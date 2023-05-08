# Comparing `tmp/rpycocotools-0.0.3.tar.gz` & `tmp/rpycocotools-0.0.4.tar.gz`

## Comparing `rpycocotools-0.0.3.tar` & `rpycocotools-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,52 @@
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 rpycocotools-0.0.3/local_dependencies/cocotools/Cargo.toml
--rw-r--r--   0     1001      123       30 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/.gitignore
--rw-r--r--   0     1001      123    55307 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/Cargo.lock
--rw-r--r--   0     1001      123     1310 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/README.md
--rw-r--r--   0     1001      123    17709 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/annotations/coco.rs
--rw-r--r--   0     1001      123     5364 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/annotations/coco_pyo3.rs
--rw-r--r--   0     1001      123      169 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/annotations.rs
--rw-r--r--   0     1001      123     1185 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/argparse.rs
--rw-r--r--   0     1001      123    21662 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/converters/mask.rs
--rw-r--r--   0     1001      123       72 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/converters.rs
--rw-r--r--   0     1001      123     3024 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/errors.rs
--rw-r--r--   0     1001      123     1890 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/lib.rs
--rw-r--r--   0     1001      123     1529 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/main.rs
--rw-r--r--   0     1001      123      724 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/utils.rs
--rw-r--r--   0     1001      123     2327 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/visualize/display.rs
--rw-r--r--   0     1001      123     5849 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/visualize/draw.rs
--rw-r--r--   0     1001      123      141 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/src/visualize.rs
--rw-r--r--   0     1001      123      610 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/local_dependencies/cocotools/tests/load_coco.rs
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 rpycocotools-0.0.3/Cargo.toml
--rw-r--r--   0     1001      123      119 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/.gitignore
--rw-r--r--   0     1001      123       58 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/.rustfmt.toml
--rw-r--r--   0     1001      123    45725 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/Cargo.lock
--rw-r--r--   0     1001      123     1744 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/README.md
--rw-r--r--   0     1001      123       10 2023-03-27 19:29:55.000000 rpycocotools-0.0.3/dist/rpycocotools-0.0.3.tar.gz
--rw-r--r--   0     1001      123     3076 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/pyproject.toml
--rw-r--r--   0     1001      123      499 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/requirements-build.txt
--rw-r--r--   0     1001      123      939 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/requirements-dev.txt
--rw-r--r--   0     1001      123      819 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/requirements-test.txt
--rw-r--r--   0     1001      123     3963 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/src/coco.rs
--rw-r--r--   0     1001      123     1101 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/src/errors.rs
--rw-r--r--   0     1001      123     1360 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/src/main.rs
--rw-r--r--   0     1001      123     3210 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/src/mask.rs
--rw-r--r--   0     1001      123      204 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/tests/conftest.py
--rw-r--r--   0     1001      123     3018 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/tests/test_coco.py
--rw-r--r--   0     1001      123     2280 2023-03-27 19:28:19.000000 rpycocotools-0.0.3/tests/test_mask.py
--rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 rpycocotools-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.toml
+-rw-r--r--   0     1001      123       30 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/.gitignore
+-rw-r--r--   0     1001      123    55307 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.lock
+-rw-r--r--   0     1001      123      980 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/README.md
+-rw-r--r--   0     1001      123     1186 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/argparse.rs
+-rw-r--r--   0     1001      123    18281 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/object_detection.rs
+-rw-r--r--   0     1001      123     6758 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/pyo3.rs
+-rw-r--r--   0     1001      123      181 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/coco.rs
+-rw-r--r--   0     1001      123     3024 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/errors.rs
+-rw-r--r--   0     1001      123     1901 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/lib.rs
+-rw-r--r--   0     1001      123     1510 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/main.rs
+-rw-r--r--   0     1001      123    22560 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/mask/conversions.rs
+-rw-r--r--   0     1001      123      215 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/mask.rs
+-rw-r--r--   0     1001      123      724 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/utils.rs
+-rw-r--r--   0     1001      123     2296 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/display.rs
+-rw-r--r--   0     1001      123     6037 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/draw.rs
+-rw-r--r--   0     1001      123      141 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize.rs
+-rw-r--r--   0     1001      123      610 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/local_dependencies/cocotools/tests/load_coco.rs
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      123      173 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/.gitignore
+-rw-r--r--   0     1001      123       58 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/.rustfmt.toml
+-rw-r--r--   0     1001      123    45992 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/Cargo.lock
+-rw-r--r--   0     1001      123     2033 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/README.md
+-rw-r--r--   0     1001      123       10 2023-05-08 07:08:04.000000 rpycocotools-0.0.4/dist/rpycocotools-0.0.4.tar.gz
+-rw-r--r--   0     1001      123      634 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/Makefile
+-rw-r--r--   0     1001      123        0 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/_static/.gitkeep
+-rw-r--r--   0     1001      123     1572 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/conf.py
+-rw-r--r--   0     1001      123     8574 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/dataset.rst
+-rw-r--r--   0     1001      123      631 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/examples.rst
+-rw-r--r--   0     1001      123      731 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/make.bat
+-rw-r--r--   0     1001      123      101 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/quickstart.rst
+-rw-r--r--   0     1001      123     2805 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/docs/segmentation_masks.rst
+-rw-r--r--   0     1001      123     4077 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/pyproject.toml
+-rw-r--r--   0     1001      123      157 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/python/rpycocotools/__init__.py
+-rw-r--r--   0     1001      123     2147 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/python/rpycocotools/mask.py
+-rw-r--r--   0     1001      123      872 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/README.md
+-rw-r--r--   0     1001      123     4323 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-build.txt
+-rw-r--r--   0     1001      123     6529 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-dev.txt
+-rw-r--r--   0     1001      123    19383 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-doc.txt
+-rw-r--r--   0     1001      123     7535 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-flake8.txt
+-rw-r--r--   0     1001      123     4641 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements-test.txt
+-rw-r--r--   0     1001      123     3142 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/requirements/requirements.txt
+-rw-r--r--   0     1001      123     5136 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/coco.rs
+-rw-r--r--   0     1001      123     1179 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/errors.rs
+-rw-r--r--   0     1001      123     1434 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/main.rs
+-rw-r--r--   0     1001      123     5032 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/src/mask.rs
+-rw-r--r--   0     1001      123      204 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/conftest.py
+-rw-r--r--   0     1001      123     3061 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/test_coco.py
+-rw-r--r--   0     1001      123     2289 2023-05-08 07:06:47.000000 rpycocotools-0.0.4/tests/test_mask.py
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 rpycocotools-0.0.4/PKG-INFO
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/Cargo.toml` & `rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "cocotools"
 version = "0.0.3"
 edition = "2021"
-rust-version = "1.65.0"
+rust-version = "1.64.0"
 description = "Package providing functionalities to work with COCO format datasets."
 readme = "README.md"
 categories = ["command-line-utilities"]
 authors = ["Hoel Bagard"]
 license = "MIT OR Apache-2.0"
 
 [dependencies]
@@ -18,14 +18,21 @@
 rand = "0.8.5"
 minifb = "0.23"
 anyhow = "1.0.69"
 thiserror = "1.0.38"
 ndarray = "0.15.6"
 pyo3 = { version = "0.18", features = ["extension-module"], optional = true}
 
+[dev-dependencies]
+rstest = "0.16.0"
+proptest = "1.1.0"
+rand = "0.8.5"
+# ndarray-rand = "0.14.0"
+criterion = {version = "0.4.0", features = ["html_reports"] }
+
 [features]
 default = []
 pyo3 = ["dep:pyo3"]
 
 [profile.dev]
 opt-level = 1
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/Cargo.lock` & `rpycocotools-0.0.4/local_dependencies/cocotools/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1683,17 +1683,17 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dccf47db1b41fa1573ed27ccf5e08e3ca771cb994f776668c5ebda893b248fc"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/README.md` & `rpycocotools-0.0.4/local_dependencies/cocotools/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Cocotools
 The `cocotools` crate provides tools to load, manipulate, convert and visualize COCO format datasets.
 
-This crate aims to provide similar functionalities to the [python pycocotools package](https://pypi.org/project/pycocotools/) / [cocoapi](https://github.com/cocodataset/cocoapi) with additionnal utilities such as conversion between dataset formats. It also aims to have a better documentation and a more readable implementation.
-
 ## API Usage example
 ```
 use std::path::PathBuf;
 use cocotools::COCO;
 
 let annotations_file_path = PathBuf::from("../data_samples/coco_25k/annotations.json");
 let dataset = COCO::try_from(&annotations_file_path)?;
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/annotations/coco.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/object_detection.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 pub struct Dataset {
     pub images: Vec<Image>,
     pub annotations: Vec<Annotation>,
     pub categories: Vec<Category>,
 }
 
 /// Stores information relating to one image.
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
 #[derive(Clone, Debug, PartialEq, Eq, Deserialize, Serialize)]
 pub struct Image {
     pub id: u32,
     pub width: u32,
     pub height: u32,
     pub file_name: String,
     // "license": int,
@@ -37,105 +37,114 @@
 
 /// Object instance annotation for object detection.\
 ///
 /// Each object instance annotation contains a series of fields, including the category id and segmentation mask of the object.\
 /// In [the original COCO dataset](https://cocodataset.org/#home), the segmentation format depends on whether the instance represents a single object (`iscrowd=0` in which case polygons are used) or a collection of objects (`iscrowd=1` in which case RLE is used). Note that a single object (iscrowd=0) may require multiple polygons, for example if occluded.\
 /// Crowd annotations (`iscrowd=1`) are used to label large groups of objects (e.g. a crowd of people). In addition, an enclosing bounding box is provided for each object (box coordinates are measured from the top left image corner and are 0-indexed).\
 /// Finally, the categories field of the annotation structure stores the mapping of category id to category and supercategory names.
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct Annotation {
     pub id: u32,
     pub image_id: u32,
     pub category_id: u32,
-    /// Segmentation in the annotation file can be a polygon, RLE or encoded RLE.\
+    /// Segmentation in the annotation file can be a polygon, RLE or COCO RLE.\
     /// Examples of what each segmentation should look like in the JSON file:
     /// - [`Polygons`]: `"segmentation": [[510.66, 423.01, 511.72, 420.03, ..., 510.45, 423.01]]`
     /// - [`Rle`]: `"segmentation": {"size": [40, 40], "counts": [245, 5, 35, 5, ..., 5, 35, 5, 1190]}`
-    /// - [`EncodedRle`]: `"segmentation": {"size": [480, 640], "counts": "aUh2b0X...BgRU4"}`
+    /// - [`CocoRle`]: `"segmentation": {"size": [480, 640], "counts": "aUh2b0X...BgRU4"}`
     pub segmentation: Segmentation,
     pub area: f64,
     /// The COCO bounding box format is `[top left x position, top left y position, width, height]`.\
     /// Example: "bbox": `[473.07, 395.93, 38.65, 28.67]`
     pub bbox: Bbox,
     /// Either 1 or 0
     pub iscrowd: u32,
 }
 
 // #[cfg_attr(feature = "pyo3", pyclass)]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 #[serde(untagged)]
 pub enum Segmentation {
     Rle(Rle),
-    EncodedRle(EncodedRle),
+    CocoRle(CocoRle),
     Polygons(Polygons),
     #[serde(skip)]
     PolygonsRS(PolygonsRS),
 }
 
 /// Polygon(s) representing a segmentation mask.
 ///
 /// A Segmentation mask might require multiple polygons if the mask is in multiple parts (in case of partial occlusion for example).
 ///
 /// Each `Vec<f64>` represents an enclosed area belonging to the segmentation mask.
 /// The length of each vector must be even. Every 2*n value represents the x coordinates of the nth point, while the 2*n+1 represents its y coordinates.
 ///
 /// # Example:
 /// ```rust
-/// # use cocotools::annotations::coco::Polygons;
+/// # use cocotools::coco::object_detection::Polygons;
 /// let poly: Polygons = vec![vec![510.66, 423.01, 511.72, 420.03, 510.45, 423.01], vec![10.0, 10.0, 15.0, 15.0, 10.0, 15.0]];
 /// assert_eq!(poly.len(), 2);
 /// assert_eq!(poly[0].len() % 2, 0);
 /// ```
 pub type Polygons = Vec<Vec<f64>>;
 
 /// Internal type used to represent polygons.
 ///
 /// It contains the width and height of the image for easier handling, notably when using traits.
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
 #[derive(Clone, Debug, Deserialize, Serialize)]
 pub struct PolygonsRS {
     /// Vector with two elements, the width and height of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     /// See [`Polygons`].
     pub counts: Vec<Vec<f64>>,
 }
 
 /// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(get_all, name = "RLE", module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
 pub struct Rle {
     /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     pub counts: Vec<u32>,
 }
 
-/// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding) and then encoded into a string.
+/// Segmentation mask compressed as a [Run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding) and then further compressed into a string.
 ///
 /// For the encoding process, see [here](https://github.com/cocodataset/cocoapi/blob/master/common/maskApi.c#L204).
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(get_all, name = "COCO_RLE", module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
-pub struct EncodedRle {
+pub struct CocoRle {
     /// Vector with two elements, the height and width of the image corresponding to the segmentation mask.
     pub size: Vec<u32>,
     pub counts: String,
 }
 
 /// Bounding box enclosing an object.
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(
+    feature = "pyo3",
+    pyclass(sequence, get_all, name = "BBox", module = "rpycocotools.anns")
+)]
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 pub struct Bbox {
     pub left: f64,
     pub top: f64,
     pub width: f64,
     pub height: f64,
 }
 
 /// Category of an annotation.
-#[cfg_attr(feature = "pyo3", pyclass(get_all))]
+#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "rpycocotools.anns"))]
 #[derive(Clone, Debug, Eq, PartialEq, Deserialize, Serialize)]
 pub struct Category {
     pub id: u32,
     pub name: String,
     pub supercategory: String,
 }
 
@@ -172,20 +181,26 @@
             .categories
             .into_iter()
             .map(|category| (category.id, category))
             .collect();
 
         let imgs: HashMap<u32, Image> = dataset
             .images
+            .clone()
             .into_iter()
             .map(|image| (image.id, image))
             .collect();
 
         let mut anns: HashMap<u32, Annotation> = HashMap::new();
-        let mut img_to_anns: HashMap<u32, HashSet<u32>> = HashMap::new();
+        // Have (at least) an empty set for each image to avoid getting an error in the case where an image does not have any annotation.
+        let mut img_to_anns: HashMap<u32, HashSet<u32>> = dataset
+            .images
+            .into_iter()
+            .map(|image| (image.id, HashSet::new()))
+            .collect();
 
         for mut annotation in dataset.annotations {
             let ann_id = annotation.id;
             let img_id = annotation.image_id;
 
             // The polygon format from COCO is annoying to deal with as it does not contain the size of the image,
             // it is therefore transformed into a more complete format.
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/annotations/coco_pyo3.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/coco/pyo3.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use pyo3::class::basic::CompareOp;
 use pyo3::prelude::*;
 
-use crate::annotations::coco::*;
+use crate::coco::object_detection::*;
 
 #[pymethods]
 impl Annotation {
     fn __repr__(&self) -> String {
         format!(
             "Annotation(id={}, image_id={}, category_id={}, segmentation={}, area={}, bbox={}, iscrowd={})",
             self.id, self.image_id, self.category_id, &self.segmentation.__repr__(), self.area, &self.bbox.__repr__(), self.iscrowd
@@ -93,33 +93,44 @@
         slf
     }
 
     fn __next__(mut slf: PyRefMut<'_, Self>) -> Option<f64> {
         slf.inner.next()
     }
 }
+
 #[pymethods]
 impl Bbox {
     #[new]
     fn new(left: f64, top: f64, width: f64, height: f64) -> Self {
         Self {
             left,
             top,
             width,
             height,
         }
     }
 
     fn __repr__(&self) -> String {
         format!(
-            "Bbox(left={}, top={}, width={}, height={})",
+            "BBox(left={}, top={}, width={}, height={})",
             self.left, self.top, self.width, self.height
         )
     }
 
+    fn __len__(&self) -> usize {
+        4
+    }
+
+    fn __getitem__(&self, idx: usize) -> f64 {
+        // https://pyo3.rs/main/doc/pyo3/types/struct.pysequence
+        // https://docs.rs/pyo3/0.14.3/pyo3/class/sequence/trait.PySequenceProtocol.html
+        [self.left, self.top, self.width, self.height][idx]
+    }
+
     fn __iter__(slf: PyRef<'_, Self>) -> PyResult<Py<BboxIter>> {
         let iter = BboxIter {
             inner: vec![slf.left, slf.top, slf.width, slf.height].into_iter(),
         };
         Py::new(slf.py(), iter)
     }
 
@@ -144,56 +155,80 @@
 impl Rle {
     #[new]
     fn new(size: Vec<u32>, counts: Vec<u32>) -> Self {
         Self { size, counts }
     }
 
     fn __repr__(&self) -> String {
-        format!("RLE(counts={:?}, size={:?})", self.counts, self.size)
+        format!("RLE(size={:?}, counts={:?})", self.size, self.counts)
+    }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+        match op {
+            CompareOp::Eq => (self.size == other.size && self.counts == other.counts).into_py(py),
+            CompareOp::Ne => (self.size != other.size || self.counts != other.counts).into_py(py),
+            _ => py.NotImplemented(),
+        }
     }
 }
 
 #[pymethods]
-impl EncodedRle {
+impl CocoRle {
     #[new]
     fn new(size: Vec<u32>, counts: String) -> Self {
         Self { size, counts }
     }
 
     fn __repr__(&self) -> String {
-        format!("EncodedRLE(counts={:?}, size={:?})", self.counts, self.size)
+        format!("COCO_RLE(size={:?}, counts={:?})", self.size, self.counts)
+    }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+        match op {
+            CompareOp::Eq => (self.size == other.size && self.counts == other.counts).into_py(py),
+            CompareOp::Ne => (self.size != other.size || self.counts != other.counts).into_py(py),
+            _ => py.NotImplemented(),
+        }
     }
 }
 
 #[pymethods]
 impl PolygonsRS {
     #[new]
     fn new(size: Vec<u32>, counts: Vec<Vec<f64>>) -> Self {
         Self { size, counts }
     }
 
     fn __repr__(&self) -> String {
-        format!("PolygonsRS(counts={:?})", self.counts)
+        format!("PolygonsRS(size={:?}, counts={:?})", self.size, self.counts)
+    }
+
+    fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+        match op {
+            CompareOp::Eq => (self.size == other.size && self.counts == other.counts).into_py(py),
+            CompareOp::Ne => (self.size != other.size || self.counts != other.counts).into_py(py),
+            _ => py.NotImplemented(),
+        }
     }
 }
 
 impl Segmentation {
     fn __repr__(&self) -> String {
         match self {
             Segmentation::Rle(rle) => rle.__repr__(),
-            Segmentation::EncodedRle(encoded_rle) => encoded_rle.__repr__(),
+            Segmentation::CocoRle(coco_rle) => coco_rle.__repr__(),
             Segmentation::Polygons(poly) => format!("Polygons(counts={:?})", poly),
             Segmentation::PolygonsRS(poly) => poly.__repr__(),
         }
     }
 }
 
 impl IntoPy<PyObject> for Segmentation {
     fn into_py(self, py: Python<'_>) -> PyObject {
         match self {
             Segmentation::Rle(rle) => rle.into_py(py),
-            Segmentation::EncodedRle(encoded_rle) => encoded_rle.into_py(py),
+            Segmentation::CocoRle(coco_rle) => coco_rle.into_py(py),
             Segmentation::Polygons(poly) => poly.into_py(py),
             Segmentation::PolygonsRS(poly) => poly.into_py(py),
         }
     }
 }
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/argparse.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/argparse.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::path::PathBuf;
 
 use clap::{Parser, Subcommand};
 
-use crate::converters::mask::Segmentation;
+use crate::mask::conversions::Segmentation;
 
 #[derive(Parser)]
 #[command(author, version, about)]
 pub struct Cli {
     #[command(subcommand)]
     pub command: Commands,
 }
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/converters/mask.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/mask/conversions.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,126 @@
 use clap::ValueEnum;
 use image;
 use imageproc::contours;
 use imageproc::drawing;
-use ndarray::{s, Array2, ArrayViewMut, ShapeBuilder};
+use ndarray::{s, ArrayViewMut, ShapeBuilder};
 
-use crate::annotations::coco;
+use super::Mask;
+use crate::coco::object_detection;
 use crate::errors::MaskError;
 
-/// A boolean mask indicating for each pixel whether it belongs to the object or not.
-pub type Mask = Array2<u8>;
-
 /// Segmentation types.
 #[derive(Copy, Clone, PartialEq, Eq, PartialOrd, Ord, ValueEnum)]
 pub enum Segmentation {
     Polygons,
     Rle,
-    EncodedRle,
+    CocoRle,
 }
 
 /// Converts all the segmentation masks in the dataset to the desired type.
 ///
 /// # Errors
 ///
 /// Will return `Err` if the conversion failed.
 pub fn convert_coco_segmentation(
-    dataset: &mut coco::HashmapDataset,
+    dataset: &mut object_detection::HashmapDataset,
     target_segmentation: Segmentation,
 ) -> Result<(), MaskError> {
+    use object_detection::Segmentation::{CocoRle, Polygons, PolygonsRS, Rle};
+    use Segmentation as S;
     for ann in dataset.anns.values_mut() {
         let converted_segmentation = match &ann.segmentation {
-            coco::Segmentation::Rle(rle) => match target_segmentation {
-                Segmentation::Rle => coco::Segmentation::Rle(rle.clone()),
-                Segmentation::EncodedRle => {
-                    coco::Segmentation::EncodedRle(coco::EncodedRle::try_from(rle)?)
-                }
-                Segmentation::Polygons => coco::Segmentation::Polygons(coco::Polygons::from(rle)),
+            Rle(rle) => match target_segmentation {
+                S::Rle => Rle(rle.clone()),
+                S::CocoRle => CocoRle(object_detection::CocoRle::try_from(rle)?),
+                S::Polygons => Polygons(object_detection::Polygons::from(rle)),
             },
-            coco::Segmentation::EncodedRle(encoded_rle) => match target_segmentation {
-                Segmentation::Rle => coco::Segmentation::Rle(coco::Rle::from(encoded_rle)),
-                Segmentation::EncodedRle => coco::Segmentation::EncodedRle(encoded_rle.clone()),
-                Segmentation::Polygons => coco::Segmentation::Polygons(coco::Polygons::from(
-                    &coco::Rle::from(encoded_rle),
+            CocoRle(coco_rle) => match target_segmentation {
+                S::Rle => Rle(object_detection::Rle::from(coco_rle)),
+                S::CocoRle => CocoRle(coco_rle.clone()),
+                S::Polygons => Polygons(object_detection::Polygons::from(
+                    &object_detection::Rle::from(coco_rle),
                 )),
             },
-            coco::Segmentation::PolygonsRS(poly) => match target_segmentation {
-                Segmentation::Rle => coco::Segmentation::Rle(coco::Rle::try_from(poly)?),
-                Segmentation::EncodedRle => coco::Segmentation::EncodedRle(
-                    coco::EncodedRle::try_from(&coco::Rle::from(&Mask::try_from(poly)?))?,
-                ),
-                Segmentation::Polygons => coco::Segmentation::Polygons(poly.counts.clone()),
+            PolygonsRS(poly) => match target_segmentation {
+                S::Rle => Rle(object_detection::Rle::try_from(poly)?),
+                S::CocoRle => CocoRle(object_detection::CocoRle::try_from(poly)?),
+                S::Polygons => Polygons(poly.counts.clone()),
             },
-            coco::Segmentation::Polygons(_) => unimplemented!(),
+            Polygons(_) => unimplemented!(),
         };
         ann.segmentation = converted_segmentation;
     }
     Ok(())
 }
 
-#[allow(clippy::expect_used)]
-impl From<&coco::Rle> for coco::Polygons {
-    fn from(rle: &coco::Rle) -> Self {
-        let mask = Mask::from(rle);
-        let mask_img = mask
-            .as_slice_memory_order()
-            .map(|slice| {
-                image::GrayImage::from_raw(rle.size[1], rle.size[0], slice.to_owned()).expect(
-                    "Buffer already contains a mask created using the rle sizes and is threfore big enough."
-                )
-            })
-            .expect("The mask is created just above and should therefore be continuous in memory.");
-
-        let contours = contours::find_contours::<u32>(&mask_img);
-
-        // find_contours returns all the points defining the contours, the following for loop removes all the points formings lines as they are not needed.
-        let mut counts: Self = Self::new();
-        let mut prev_prev_x: u32;
-        let mut prev_prev_y: u32;
-        let mut prev_x: u32;
-        let mut prev_y: u32;
-        for (i, contour) in contours.iter().enumerate() {
-            // Valid polygons must have at least 3 points.
-            // The case of having less than 3 points is not expected to occur on real data, hence the silent failt if it occurs.
-            if contour.points.len() > 3 {
-                counts.push(Vec::with_capacity(2 * contour.points.len()));
-
-                counts[i].push(f64::from(contour.points[0].y));
-                counts[i].push(f64::from(contour.points[0].x));
-                prev_prev_x = contour.points[0].x;
-                prev_prev_y = contour.points[0].y;
-                prev_x = contour.points[1].x;
-                prev_y = contour.points[1].y;
-                for point in &contour.points {
-                    if !((prev_prev_x == prev_x && prev_x == point.x)
-                        || (prev_prev_y == prev_y && prev_y == point.y))
-                    {
-                        counts[i].push(f64::from(prev_y));
-                        counts[i].push(f64::from(prev_x));
-                    }
-                    prev_prev_x = prev_x;
-                    prev_prev_y = prev_y;
-                    prev_x = point.x;
-                    prev_y = point.y;
-                }
-
-                if !((prev_prev_x == prev_x && prev_x == contour.points[0].x)
-                    || (prev_prev_y == prev_y && prev_y == contour.points[0].y))
-                {
-                    counts[i].push(f64::from(prev_y));
-                    counts[i].push(f64::from(prev_x));
-                }
-            }
-        }
-        counts
-    }
-}
-
-impl TryFrom<&coco::PolygonsRS> for coco::Rle {
+impl TryFrom<&object_detection::PolygonsRS> for object_detection::Rle {
     type Error = MaskError;
     // It might be more efficient to do it like this: https://github.com/cocodataset/cocoapi/blob/master/common/maskApi.c#L162
     // It would also avoid having slightly different results from the reference implementation.
-    fn try_from(poly: &coco::PolygonsRS) -> Result<Self, Self::Error> {
+    fn try_from(poly: &object_detection::PolygonsRS) -> Result<Self, Self::Error> {
         Ok(Self::from(&Mask::try_from(poly)?))
     }
 }
 
-/// Decode encoded rle segmentation information into a rle.
+/// Convert a mask into its RLE form.
+///
+/// ## Args:
+/// - mask: A binary mask indicating for each pixel whether it belongs to the object or not.
+///
+/// ## Returns:
+/// - The RLE corresponding to the mask.
+// The implementation makes a clone of the mask, which is expensive. This could be avoided by taking a mutable reference and reversing the axes again after the for loop.
+// However asking for a mutable reference might be confusing.
+#[allow(clippy::cast_possible_truncation)]
+impl From<&Mask> for object_detection::Rle {
+    fn from(mask: &Mask) -> Self {
+        let mut previous_value = 0;
+        let mut count = 0;
+        let mut counts = Vec::new();
+        for value in mask.clone().reversed_axes().iter() {
+            if *value != previous_value {
+                counts.push(count);
+                previous_value = *value;
+                count = 0;
+            }
+            count += 1;
+        }
+        counts.push(count);
+
+        Self {
+            size: vec![mask.nrows() as u32, mask.ncols() as u32],
+            counts,
+        }
+    }
+}
+
+/// Decode COCO RLE segmentation information into RLE.
 
 /// See the (hard to read) implementation:
 /// <https://github.com/cocodataset/cocoapi/blob/master/common/maskApi.c#L218>
 /// <https://github.com/cocodataset/cocoapi/blob/8c9bcc3cf640524c4c20a9c40e89cb6a2f2fa0e9/PythonAPI/pycocotools/_mask.pyx#L145>
 
 /// [LEB128 wikipedia article](https://en.wikipedia.org/wiki/LEB128#Decode_signed_integer)
 /// It is similar to LEB128, but here shift is incremented by 5 instead of 7 because the implementation uses
 /// 6 bits per byte instead of 8. (no idea why, I guess it's more efficient for the COCO dataset?)
 #[allow(clippy::cast_sign_loss, clippy::cast_possible_wrap)]
-impl From<&coco::EncodedRle> for coco::Rle {
+impl From<&object_detection::CocoRle> for object_detection::Rle {
     /// Converts a compressed RLE to its uncompressed version.
-    fn from(encoded_rle: &coco::EncodedRle) -> Self {
+    fn from(coco_rle: &object_detection::CocoRle) -> Self {
         assert!(
-            encoded_rle.counts.is_ascii(),
-            "Encoded RLE is not in valid ascii."
+            coco_rle.counts.is_ascii(),
+            "COCO RLE is not in valid ascii."
         );
 
-        let bytes_rle = encoded_rle.counts.as_bytes();
+        let bytes_rle = coco_rle.counts.as_bytes();
 
         let mut current_count_idx: usize = 0;
         let mut current_byte_idx: usize = 0;
-        let mut counts: Vec<u32> = vec![0; encoded_rle.counts.len()];
+        let mut counts: Vec<u32> = vec![0; coco_rle.counts.len()];
         while current_byte_idx < bytes_rle.len() {
             let mut continuous_pixels: i32 = 0;
             let mut shift = 0;
             let mut high_order_bit = 1;
 
             // When the high order bit of a byte becomes 0, we have decoded the integer and can move on to the next one.
             while high_order_bit != 0 {
@@ -186,28 +156,28 @@
                 counts.pop();
             } else {
                 break;
             }
         }
 
         Self {
-            size: encoded_rle.size.clone(),
+            size: coco_rle.size.clone(),
             counts,
         }
     }
 }
 
-impl TryFrom<&coco::Rle> for coco::EncodedRle {
+impl TryFrom<&object_detection::Rle> for object_detection::CocoRle {
     type Error = MaskError;
 
-    // Get compressed string representation of encoded mask.
-    fn try_from(rle: &coco::Rle) -> Result<Self, Self::Error> {
+    // Get COCO compressed string representation of RLE.
+    fn try_from(rle: &object_detection::Rle) -> Result<Self, Self::Error> {
         let mut high_order_bit: bool;
         let mut byte: u8;
-        let mut encoded_counts: Vec<u8> = Vec::new();
+        let mut coco_counts: Vec<u8> = Vec::new();
 
         for i in 0..rle.counts.len() {
             let mut continuous_pixels = i64::from(rle.counts[i]);
             if i > 2 {
                 continuous_pixels -= i64::from(rle.counts[i - 2]);
             }
             high_order_bit = true;
@@ -220,31 +190,114 @@
                 } else {
                     continuous_pixels != -1
                 };
                 if high_order_bit {
                     byte |= 0x20;
                 };
                 byte += 48;
-                encoded_counts.push(byte);
+                coco_counts.push(byte);
             }
         }
         Ok(Self {
             size: rle.size.clone(),
-            counts: std::str::from_utf8(&encoded_counts)
-                .map_err(|err| MaskError::StrConversion(err, encoded_counts.clone()))?
+            counts: std::str::from_utf8(&coco_counts)
+                .map_err(|err| MaskError::StrConversion(err, coco_counts.clone()))?
                 .to_string(),
         })
     }
 }
 
+impl TryFrom<&object_detection::PolygonsRS> for object_detection::CocoRle {
+    type Error = MaskError;
+    fn try_from(poly: &object_detection::PolygonsRS) -> Result<Self, Self::Error> {
+        Self::try_from(&object_detection::Rle::from(&Mask::try_from(poly)?))
+    }
+}
+
+#[allow(clippy::cast_possible_truncation)]
+impl TryFrom<&Mask> for object_detection::CocoRle {
+    type Error = MaskError;
+    fn try_from(mask: &Mask) -> Result<Self, Self::Error> {
+        Self::try_from(&object_detection::Rle::from(mask))
+    }
+}
+
 #[allow(clippy::expect_used)]
-impl From<&coco::Rle> for Mask {
+impl From<&object_detection::Rle> for object_detection::Polygons {
+    fn from(rle: &object_detection::Rle) -> Self {
+        let mask = Mask::from(rle);
+        let mask_img = mask
+            .as_slice_memory_order()
+            .map(|slice| {
+                image::GrayImage::from_raw(rle.size[1], rle.size[0], slice.to_owned()).expect(
+                    "Buffer already contains a mask created using the rle sizes and is threfore big enough."
+                )
+            })
+            .expect("The mask is created just above and should therefore be continuous in memory.");
+
+        let contours = contours::find_contours::<u32>(&mask_img);
+
+        // find_contours returns all the points defining the contours, the following for loop removes all the points formings lines as they are not needed.
+        let mut counts: Self = Self::new();
+        let mut prev_prev_x: u32;
+        let mut prev_prev_y: u32;
+        let mut prev_x: u32;
+        let mut prev_y: u32;
+        for (i, contour) in contours.iter().enumerate() {
+            // Valid polygons must have at least 3 points.
+            // The case of having less than 3 points is not expected to occur on real data, hence the silent failt if it occurs.
+            if contour.points.len() > 3 {
+                counts.push(Vec::with_capacity(2 * contour.points.len()));
+
+                counts[i].push(f64::from(contour.points[0].y));
+                counts[i].push(f64::from(contour.points[0].x));
+                prev_prev_x = contour.points[0].x;
+                prev_prev_y = contour.points[0].y;
+                prev_x = contour.points[1].x;
+                prev_y = contour.points[1].y;
+                for point in &contour.points {
+                    if !((prev_prev_x == prev_x && prev_x == point.x)
+                        || (prev_prev_y == prev_y && prev_y == point.y))
+                    {
+                        counts[i].push(f64::from(prev_y));
+                        counts[i].push(f64::from(prev_x));
+                    }
+                    prev_prev_x = prev_x;
+                    prev_prev_y = prev_y;
+                    prev_x = point.x;
+                    prev_y = point.y;
+                }
+
+                if !((prev_prev_x == prev_x && prev_x == contour.points[0].x)
+                    || (prev_prev_y == prev_y && prev_y == contour.points[0].y))
+                {
+                    counts[i].push(f64::from(prev_y));
+                    counts[i].push(f64::from(prev_x));
+                }
+            }
+        }
+        counts
+    }
+}
+
+#[allow(clippy::cast_possible_truncation)]
+impl From<&Mask> for object_detection::PolygonsRS {
+    fn from(mask: &Mask) -> Self {
+        Self {
+            size: vec![mask.shape()[0] as u32, mask.shape()[1] as u32],
+            counts: object_detection::Polygons::from(&object_detection::Rle::from(mask)),
+        }
+    }
+}
+
+#[allow(clippy::expect_used)]
+impl From<&object_detection::Rle> for Mask {
     /// Converts a RLE to its uncompressed mask.
     #[allow(clippy::cast_possible_truncation)]
-    fn from(rle: &coco::Rle) -> Self {
+    fn from(rle: &object_detection::Rle) -> Self {
         let width = rle.size[1] as usize;
         let height = rle.size[0] as usize;
 
         let mut mask: Self = Self::zeros((height, width).f());
         let mut mask_1d = ArrayViewMut::from_shape(
             (height * width).f(),
             mask.as_slice_memory_order_mut().expect("The mask array is created just above, there shouldn't be any error when creating a view of it"),
@@ -260,70 +313,38 @@
             current_value = u8::from(current_value == 0);
             current_position += *nb_pixels as usize;
         }
         mask
     }
 }
 
-/// Convert a mask into its RLE form.
-///
-/// ## Args:
-/// - mask: A binary mask indicating for each pixel whether it belongs to the object or not.
-///
-/// ## Returns:
-/// - The RLE corresponding to the mask.
-// The implementation makes a clone of the mask, which is expensive. This could be avoided by taking a mutable reference and reversing the axes again after the for loop.
-// However asking for a mutable reference might be confusing.
-#[allow(clippy::cast_possible_truncation)]
-impl From<&Mask> for coco::Rle {
-    fn from(mask: &Mask) -> Self {
-        let mut previous_value = 0;
-        let mut count = 0;
-        let mut counts = Vec::new();
-        for value in mask.clone().reversed_axes().iter() {
-            if *value != previous_value {
-                counts.push(count);
-                previous_value = *value;
-                count = 0;
-            }
-            count += 1;
-        }
-        counts.push(count);
-
-        Self {
-            size: vec![mask.nrows() as u32, mask.ncols() as u32],
-            counts,
-        }
-    }
-}
-
-impl TryFrom<&coco::Segmentation> for Mask {
+impl TryFrom<&object_detection::Segmentation> for Mask {
     type Error = MaskError;
 
-    fn try_from(coco_segmentation: &coco::Segmentation) -> Result<Self, Self::Error> {
+    fn try_from(coco_segmentation: &object_detection::Segmentation) -> Result<Self, Self::Error> {
         let mask = match coco_segmentation {
-            coco::Segmentation::Rle(rle) => Self::from(rle),
-            coco::Segmentation::EncodedRle(encoded_rle) => {
-                Self::from(&coco::Rle::from(encoded_rle))
+            object_detection::Segmentation::Rle(rle) => Self::from(rle),
+            object_detection::Segmentation::CocoRle(coco_rle) => {
+                Self::from(&object_detection::Rle::from(coco_rle))
             }
-            coco::Segmentation::PolygonsRS(poly) => Self::try_from(poly)?,
-            coco::Segmentation::Polygons(_) => {
+            object_detection::Segmentation::PolygonsRS(poly) => Self::try_from(poly)?,
+            object_detection::Segmentation::Polygons(_) => {
                 unimplemented!("Use the 'mask_from_poly' function.")
             }
         };
         Ok(mask)
     }
 }
 
 #[allow(clippy::cast_possible_truncation)]
-impl TryFrom<&coco::PolygonsRS> for Mask {
+impl TryFrom<&object_detection::PolygonsRS> for Mask {
     type Error = MaskError;
 
     /// Create a mask from a compressed polygon representation.
-    fn try_from(poly_ann: &coco::PolygonsRS) -> Result<Self, Self::Error> {
+    fn try_from(poly_ann: &object_detection::PolygonsRS) -> Result<Self, Self::Error> {
         let mut mask = image::GrayImage::new(poly_ann.size[1], poly_ann.size[0]);
 
         for poly in &poly_ann.counts {
             let mut points_poly: Vec<imageproc::point::Point<i32>> = Vec::new();
             for i in (0..poly.len()).step_by(2) {
                 points_poly.push(imageproc::point::Point::new(
                     poly[i] as i32,
@@ -356,33 +377,43 @@
 ///
 /// ## Errors
 /// Will return `Err` if the internal conversion from `ImageBuffer` to Mask (ndarray) fails.
 ///
 /// ## Returns:
 /// - The decompressed mask.
 #[allow(clippy::cast_possible_truncation, clippy::module_name_repetitions)]
-pub fn mask_from_poly(poly: &coco::Polygons, width: u32, height: u32) -> Result<Mask, MaskError> {
+pub fn mask_from_poly(
+    poly: &object_detection::Polygons,
+    width: u32,
+    height: u32,
+) -> Result<Mask, MaskError> {
     let mut points_poly: Vec<imageproc::point::Point<i32>> = Vec::new();
     for i in (0..poly[0].len()).step_by(2) {
         points_poly.push(imageproc::point::Point::new(
             poly[0][i] as i32,
             poly[0][i + 1] as i32,
         ));
     }
     let mut mask = image::GrayImage::new(width, height);
     drawing::draw_polygon_mut(&mut mask, &points_poly, image::Luma([1u8]));
 
     Mask::from_shape_vec((height as usize, width as usize), mask.into_raw())
         .map_err(MaskError::ImageToNDArrayConversion)
 }
 
+#[allow(clippy::cast_possible_truncation, clippy::module_name_repetitions)]
+#[must_use]
+pub fn poly_from_mask(mask: &Mask) -> object_detection::Polygons {
+    object_detection::Polygons::from(&object_detection::Rle::from(mask))
+}
+
 #[cfg(test)]
 #[allow(clippy::unwrap_used)]
 mod tests {
-    use super::coco::{EncodedRle, Polygons, PolygonsRS, Rle};
+    use super::object_detection::{CocoRle, Polygons, PolygonsRS, Rle};
     use super::*;
     use ndarray::array;
     use proptest::prelude::*;
     use rstest::rstest;
 
     prop_compose! {
         #[allow(clippy::unwrap_used)]
@@ -408,16 +439,16 @@
                 Mask::from_shape_vec((nrows, ncols), mask_data).unwrap()
             }
     }
 
     proptest! {
         #[test]
         fn rle_decode_inverts_encode(rle in generate_rle(50, 20)){
-            let encoded_rle = EncodedRle::try_from(&rle).unwrap();
-            let decoded_rle = Rle::from(&encoded_rle);
+            let coco_rle = CocoRle::try_from(&rle).unwrap();
+            let decoded_rle = Rle::from(&coco_rle);
             prop_assert_eq!(decoded_rle, rle);
         }
     }
 
     proptest! {
         #[test]
         fn mask_to_rle_to_mask(mask in generate_mask(100, 100)){
@@ -525,19 +556,19 @@
         let mask = Mask::from(rle);
         assert_eq!(&mask, expected_mask);
     }
 
     #[rstest]
     #[case::square(
         &Rle {size: vec![4, 4], counts: vec![5, 2, 2, 2, 5]},
-        &EncodedRle { size: vec![4, 4], counts: "52203".to_string() })]
+        &CocoRle { size: vec![4, 4], counts: "52203".to_string() })]
     #[case::square2(
         &Rle {counts: vec![6, 1, 40, 4, 5, 4, 5, 4, 21], size: vec![9, 10]},
-        &EncodedRle {size: vec![9, 10], counts: "61X13mN000`0".to_string()})]
+        &CocoRle {size: vec![9, 10], counts: "61X13mN000`0".to_string()})]
     #[case::test1(
         &Rle {counts: vec![245, 5, 35, 5, 35, 5, 35, 5, 35, 5, 1190], size: vec![40, 40]},
-        &EncodedRle {size: vec![40, 40], counts: "e75S10000000ST1".to_string()})]
-    fn encode_rle(#[case] rle: &Rle, #[case] expected_encoded_rle: &EncodedRle) {
-        let encoded_rle = EncodedRle::try_from(rle).unwrap();
-        assert_eq!(&encoded_rle, expected_encoded_rle);
+        &CocoRle {size: vec![40, 40], counts: "e75S10000000ST1".to_string()})]
+    fn encode_rle(#[case] rle: &Rle, #[case] expected_coco_rle: &CocoRle) {
+        let coco_rle = CocoRle::try_from(rle).unwrap();
+        assert_eq!(&coco_rle, expected_coco_rle);
     }
 }
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/errors.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/errors.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/lib.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 //! ```
 //!
 //! ### Loading a segmentation mask
 //!
 //! ```
 //! # use std::path::PathBuf;
 //! use cocotools::COCO;
-//! use cocotools::converters::mask;
-//! use cocotools::annotations::coco;
+//! use cocotools::mask;
+//! use cocotools::mask::conversions;
+//! use cocotools::coco::object_detection;
 //!
 //! let annotations_file_path = PathBuf::from("../data_samples/coco_25k/annotations.json");
 //! let image_folder_path = PathBuf::from("../data_samples/coco_25k/images");
 //! let coco_dataset = COCO::new(&annotations_file_path, &image_folder_path)?;
 //! let anns = coco_dataset.get_img_anns(174482)?;
 //! let mask = mask::Mask::try_from(&anns[0].segmentation)?;
 //! assert_eq!(mask.ncols(), 388);
 //! assert_eq!(mask.nrows(), 640);
 //! # Ok::<(), Box<dyn std::error::Error>>(())
 //! ```
 
-pub mod annotations;
-pub mod converters;
+pub mod coco;
 pub mod errors;
+pub mod mask;
 pub(crate) mod utils;
 pub mod visualize;
 
 // #[doc(hidden)]
-pub use crate::annotations::COCO;
+pub use crate::coco::COCO;
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/main.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/main.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use std::error;
 use std::path::PathBuf;
 
 use clap::Parser;
 
-mod annotations;
 mod argparse;
-mod converters;
+mod coco;
 mod errors;
+mod mask;
 mod utils;
 mod visualize;
-use crate::annotations::COCO;
 use crate::argparse::{Cli, Commands};
+use crate::coco::COCO;
 use crate::visualize::display;
 
 fn main() -> Result<(), Box<dyn error::Error>> {
     let cli = Cli::parse();
 
     match &cli.command {
         Commands::Visualize {
@@ -35,15 +35,15 @@
         }
         Commands::ConvertSegmentation {
             annotations_path,
             target_segmentation,
             output_path,
         } => {
             let mut dataset = COCO::new(annotations_path, &PathBuf::from("N/A"))?;
-            converters::mask::convert_coco_segmentation(&mut dataset, *target_segmentation)?;
+            mask::conversions::convert_coco_segmentation(&mut dataset, *target_segmentation)?;
             let output_path = output_path
                 .as_ref()
                 .map_or_else(|| annotations_path, |output_path| output_path);
             dataset.save_to(output_path)?;
         }
     }
     Ok(())
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/utils.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/utils.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/visualize/display.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/display.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-use std::path::{Path, PathBuf};
+use std::path::PathBuf;
 
 extern crate image;
 extern crate minifb;
 use minifb::{Key, Window, WindowOptions};
 
 use super::draw::{self, ToBuffer};
-use crate::annotations::coco::{Annotation, HashmapDataset};
+use crate::coco::object_detection::{Annotation, HashmapDataset};
 use crate::utils;
 
 /// Visualize the annotations for the given image id.
 ///
 /// # Errors
 ///
 /// Will return `Err` if `img_id` is not present in the dataset.
-pub fn img_anns(
-    dataset: &HashmapDataset,
-    image_folder: &Path,
-    img_id: u32,
-) -> Result<(), Box<dyn std::error::Error>> {
+pub fn img_anns(dataset: &HashmapDataset, img_id: u32) -> Result<(), Box<dyn std::error::Error>> {
     let anns = dataset.get_img_anns(img_id)?;
     let img_name = &dataset.get_img(img_id)?.file_name;
-    let img_path = image_folder.join(img_name);
+    let img_path = dataset.image_folder.join(img_name);
 
     self::anns(&img_path, &anns, true)?;
 
     Ok(())
 }
 
 /// Display the given image in a window.
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/src/visualize/draw.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/src/visualize/draw.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 use std::iter::zip;
 
 use image;
 use imageproc::{drawing::draw_hollow_rect_mut, rect::Rect};
 use rand::Rng;
 
-use crate::annotations::coco;
-use crate::converters::mask;
+use crate::coco::object_detection;
 use crate::errors::MaskError;
+use crate::mask;
 
 /// Draw the bounding box on the image.
 ///
 /// ## Args
 /// - `img`: The image to draw on.
 /// - `bbox`: The bounding box to draw.
 /// - `color`: The color to use for drawing the bounding box.
 ///
 /// ## Example
 ///
 /// ```rust
 /// # use image::RgbImage;
-/// # use cocotools::annotations::coco::Bbox;
+/// # use cocotools::coco::object_detection::Bbox;
 /// use cocotools::visualize::draw;
 /// let mut img = RgbImage::new(60, 60);
 /// let bbox = Bbox{left: 40.0, top: 40.0, width: 10.0, height: 10.0};
 /// let color = image::Rgb([255, 0, 0]);
 /// draw::bbox(&mut img, &bbox, color);
 /// ```
 #[allow(clippy::cast_sign_loss, clippy::cast_possible_truncation)]
-pub fn bbox(img: &mut image::RgbImage, bbox: &coco::Bbox, color: image::Rgb<u8>) {
-    let rect =
-        Rect::at(bbox.left as i32, bbox.top as i32).of_size(bbox.width as u32, bbox.height as u32);
+pub fn bbox(img: &mut image::RgbImage, bbox: &object_detection::Bbox, color: image::Rgb<u8>) {
+    if bbox.width > 0.0 && bbox.height > 0.0 {
+        let rect = Rect::at(bbox.left as i32, bbox.top as i32)
+            .of_size(bbox.width as u32, bbox.height as u32);
 
-    draw_hollow_rect_mut(img, rect, color);
+        draw_hollow_rect_mut(img, rect, color);
+    }
 }
 
 /// Draw the max on the image.
 ///
 /// ## Args
 /// - `img`: The image to draw on.
 /// - `mask`: The mask to draw.
 /// - `color`: The color to use for drawing the mask.
 ///
 /// ## Example
 ///
 /// ```rust
 /// # use image::RgbImage;
 /// # use ndarray::array;
-/// # use cocotools::annotations::coco::Bbox;
+/// # use cocotools::coco::object_detection::Bbox;
 /// use cocotools::visualize::draw;
 /// let mask = &array![[0, 0, 0, 0, 0, 0, 0],
 ///                    [0, 0, 1, 1, 1, 0, 0],
 ///                    [0, 0, 1, 1, 1, 0, 0],
 ///                    [0, 0, 1, 1, 1, 0, 0],
 ///                    [0, 0, 1, 1, 1, 0, 0],
 ///                    [0, 0, 1, 1, 1, 0, 0],
@@ -78,47 +80,47 @@
 /// - `img`: The image to draw on.
 /// - `anns`: The annotations to draw. They are assumed to correspong to the image, or to an image of the same size as `img`.
 /// - `draw_bbox`: If true, then also the bounding boxes.
 ///
 /// # Example
 ///
 /// ```rust
-/// # use cocotools::annotations::coco;
+/// # use cocotools::coco::object_detection;
 /// # use image::RgbImage;
 /// use cocotools::visualize::draw;
 /// let mut img = RgbImage::new(40, 40);
 /// let anns = vec![
-///     coco::Annotation {
+///     object_detection::Annotation {
 ///         id: 1,
 ///         image_id: 1,
 ///         category_id: 1,
-///         segmentation: coco::Segmentation::EncodedRle(coco::EncodedRle {
+///         segmentation: object_detection::Segmentation::CocoRle(object_detection::CocoRle {
 ///             size: vec![40, 40],
 ///             counts: "e75S10000000ST1".to_string(),
 ///         }),
 ///         // # the bounding box here does not correspond to the segmentation.
 ///         area: 1.0,
-///         bbox: coco::Bbox {
+///         bbox: object_detection::Bbox {
 ///             left: 10.0,
 ///             top: 10.0,
 ///             width: 20.0,
 ///             height: 20.0,
 ///         },
 ///         iscrowd: 0,
 ///     },
-///     coco::Annotation {
+///     object_detection::Annotation {
 ///         id: 2,
 ///         image_id: 1,
 ///         category_id: 2,
-///         segmentation: coco::Segmentation::PolygonsRS(coco::PolygonsRS {
+///         segmentation: object_detection::Segmentation::PolygonsRS(object_detection::PolygonsRS {
 ///             size: vec![40, 40],
 ///             counts: vec![vec![4.0, 4.0, 24.0, 4.0, 24.0, 24.0, 4.0, 24.0]],
 ///         }),
 ///         area: 400.0,
-///         bbox: coco::Bbox {
+///         bbox: object_detection::Bbox {
 ///             left: 4.0,
 ///             top: 4.0,
 ///             width: 24.0,
 ///             height: 24.0,
 ///         },
 ///         iscrowd: 0,
 ///     },
@@ -127,15 +129,15 @@
 /// ```
 ///
 /// ## Errors
 ///
 /// Will return `Err` if the segmentation annotations could not be decompressed.
 pub fn anns(
     img: &mut image::ImageBuffer<image::Rgb<u8>, Vec<u8>>,
-    anns: &Vec<&coco::Annotation>,
+    anns: &Vec<&object_detection::Annotation>,
     draw_bbox: bool,
 ) -> Result<(), MaskError> {
     let mut rng = rand::thread_rng();
     for ann in anns {
         let color = image::Rgb([rng.gen::<u8>(), rng.gen::<u8>(), rng.gen::<u8>()]);
         if draw_bbox {
             self::bbox(img, &ann.bbox, color);
```

### Comparing `rpycocotools-0.0.3/local_dependencies/cocotools/tests/load_coco.rs` & `rpycocotools-0.0.4/local_dependencies/cocotools/tests/load_coco.rs`

 * *Files identical despite different names*

### Comparing `rpycocotools-0.0.3/Cargo.lock` & `rpycocotools-0.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -763,14 +763,25 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "nshare"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4447657cd40e3107416ec4f2ac3e61a18781b00061789e3b8f4bbcbccb26c4c6"
+dependencies = [
+ "image",
+ "nalgebra",
+ "ndarray",
+]
+
+[[package]]
 name = "num"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
 dependencies = [
  "num-bigint",
  "num-complex",
@@ -1238,14 +1249,16 @@
 
 [[package]]
 name = "rpycocotools"
 version = "0.0.3"
 dependencies = [
  "anyhow",
  "cocotools",
+ "ndarray",
+ "nshare",
  "numpy",
  "pyo3",
  "serde",
  "serde_json",
 ]
 
 [[package]]
@@ -1393,17 +1406,17 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
-version = "0.9.4"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6002a767bff9e83f8eeecf883ecb8011875a21ae8da43bffb817a57e78cc09"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
```

### Comparing `rpycocotools-0.0.3/README.md` & `rpycocotools-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-# Rpycocotools
+# rpycocotools
 
 [![PyPI](https://img.shields.io/pypi/v/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rpycocotools?style=flat)](https://pypi.org/project/rpycocotools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rpycocotools?style=flat-square)](https://pypistats.org/packages/rpycocotools)
 [![PyPI - License](https://img.shields.io/pypi/l/rpycocotools?style=flat)](https://opensource.org/licenses/MIT)
 
-Tool to handle COCO-like data in python. This repo is very much a wip.
+The `rpycocotools` package provides tools to load, manipulate, convert and visualize COCO format datasets.
 
+### Installation
 
-### Build
+You can install the package through pip:
+```
+pip install rpycocotools
+```
 
-Build and install into local virtualenv with `maturin develop`.
+You can also build and install it into a virtualenv with `pip install .` (do not use `maturin develop`, the imports will not work).
 
 ### Usage example
 
 Visualize image with a given `id`:
 ```python
 import rpycocotools
 coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
@@ -27,19 +31,18 @@
 </p>
 
 ```python
 import rpycocotools
 coco_dataset = rpycocotools.COCO("../data_samples/coco_25k/annotations.json", "../data_samples/coco_25k/images")
 anns = coco_dataset.get_img_anns(174482)
 mask = rpycocotools.mask.decode_poly_rs(anns[0].segmentation)
-mask = 255 * mask
 ```
 The mask is a numpy array and can be visualized (for example with opencv):
 
 <p align="center">
   <img alt="bike_segmentation" src="https://user-images.githubusercontent.com/34478245/226691842-8a11cde1-905d-434e-b287-0c3c685e01d1.png">
 </p>
 
-### Run the tests
-```
-python -m pytest . -vv
-```
+
+## TODO list:
+- Make it possible to get the dataset as a json (in order to be able to save/print it).
+- Make it possible to get the visualization image as a numpy array.
```

### Comparing `rpycocotools-0.0.3/pyproject.toml` & `rpycocotools-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "rpycocotools"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{name="Bagard Hoel"}]
 description = "Package providing utilities to load, manipulate, convert and visualize COCO format datasets."
 keywords = ["COCO", "COCO dataset"]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -19,40 +19,57 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 license = {text="MIT"}
-dependencies = ["numpy", "rpycocotools-stubs==0.0.3"]
+dependencies = ["numpy", "rpycocotools-stubs==0.0.4"]
 requires-python = ">=3.8"
 
 [project.urls]
 "Source Code" = "https://github.com/hoel-bagard/rust_coco_tools"
 
 [tool.maturin]
 sdist-include = ["LICENSE", "README.md"]
+python-source = "python"
+module-name = "rpycocotools._rpycocotools"
 # bindings = "cffi"
 # compatibility = "linux"
 
 [project.optional-dependencies]
 build = ["maturin"]
 test = ["pytest", "hypothesis"]
 dev = ["pip-tools", "ruff", "pyright"]
+doc = ["sphinx", "sphinx-rtd-theme", "sphinx-hoverxref", "sphinx-codeautolink"]
+flake8 = [
+    "flake8>=5.0.4,<6.0",
+    "flake8-bugbear>=23.3.12,<24.0",
+    "flake8-builtins>=2.1.0,<3.0",
+    "flake8-comprehensions>=3.12.0,<4.0",
+    "flake8-docstrings>=1.7.0,<2.0",
+    "flake8-quotes>=3.3.2,<4",
+    "pep8-naming>=0.13.3",
+    "flake8-import-order>=0.18.2",
+    "flake8-noqa>=1.3.1,<2",
+    "flake8-broken-line>=0.6.0",
+    "flake8-commas>=2.1.0,<3.0",
+    "Flake8-pyproject>=1.2.3,<2"
+]
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/7.1.x/explanation/goodpractices.html
 addopts = [
     "--import-mode=importlib",
     "--strict-markers",
 ]
 
 [tool.ruff]
-select = ["A", "B", "C4", "D", "E", "F", "N", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM", "ARG", "PTH", "PL", "TRY", "NPY", "RUF", "W"]
-ignore = ["D1", "D401", "D204", "D203", "D213", "S101", "PLR2004"]
+select = ["ALL"]
+exclude = ["docs/conf.py"]
 line-length = 120
 
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
@@ -61,22 +78,25 @@
 max-args = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
+"tests/**/*.py" = ["D1", "INP001", "PLR2004", "S101"]
 
 [tool.pyright]
 include = ["tests"]
+ignore = ["python"]
+pythonVersion = "3.11"
+pythonPlatform = "Linux"
 
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
-
 reportMissingModuleSource = false
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportUnusedImport = true
 reportUnusedClass = "warning"
 reportUnusedFunction = "warning"
 reportUnusedVariable = "warning"
@@ -97,9 +117,29 @@
 reportUnnecessaryComparison = "warning"
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
 
-pythonVersion = "3.10"
-pythonPlatform = "Linux"
+[tool.flake8]
+application_import_names = "rpycocotools"
+exclude = ["env", "venv", "docs"]
+max-line-length = 120
+docstring-convention = "google"
+import-order-style = "smarkets"
+inline-quotes = "double"
+# D1: Missing docstring
+# I100: Import statements are in the wrong order.
+# I201: Missing newline between import groups.
+# F401: imported but unused
+per-file-ignores = [
+    "tests/*.py:D1,I201,I100",
+    "python/rpycocotools/__init__.py:F401"
+]
+
+[tool.pylint.messages_control]
+max-line-length = 120
+disable = [
+    "import-error",
+    "no-name-in-module",
+]
```

### Comparing `rpycocotools-0.0.3/src/coco.rs` & `rpycocotools-0.0.4/src/coco.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 use std::path::PathBuf;
 
-use cocotools::annotations::coco;
+use cocotools::coco::object_detection;
 use cocotools::errors::CocoError;
 use cocotools::visualize::display;
 use cocotools::COCO;
+use nshare::ToNdarray3;
+use numpy::IntoPyArray;
+use numpy::PyArray3;
 use pyo3::exceptions::{PyKeyError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyUnicode;
 
 use crate::errors::{PyLoadingError, PyMissingIdError};
 
 #[pyclass(name = "COCO", module = "rpycocotools")]
@@ -25,70 +28,78 @@
         let annotations_path = PathBuf::from(annotations_path.to_str()?);
         let image_folder_path = PathBuf::from(image_folder_path.to_str()?);
         let dataset =
             COCO::new(annotations_path, image_folder_path).map_err(PyLoadingError::from)?;
         Ok(Self(dataset))
     }
 
-    fn get_img(&self, py: Python<'_>, img_id: u32) -> PyResult<Py<coco::Image>> {
+    fn __len__(&self) -> usize {
+        self.0.get_imgs().len()
+    }
+
+    fn get_img(&self, py: Python<'_>, img_id: u32) -> PyResult<Py<object_detection::Image>> {
         Py::new(
             py,
             self.0
                 .get_img(img_id)
                 .map_err(PyMissingIdError::from)?
                 .clone(),
         )
     }
 
-    fn get_ann(&self, py: Python<'_>, ann_id: u32) -> PyResult<Py<coco::Annotation>> {
+    fn get_ann(&self, py: Python<'_>, ann_id: u32) -> PyResult<Py<object_detection::Annotation>> {
         Py::new(
             py,
             self.0
                 .get_ann(ann_id)
                 .map_err(PyMissingIdError::from)?
                 .clone(),
         )
     }
 
-    fn get_cat(&self, py: Python<'_>, cat_id: u32) -> PyResult<Py<coco::Category>> {
+    fn get_cat(&self, py: Python<'_>, cat_id: u32) -> PyResult<Py<object_detection::Category>> {
         Py::new(
             py,
             self.0
                 .get_cat(cat_id)
                 .map_err(PyMissingIdError::from)?
                 .clone(),
         )
     }
 
     /// Order is non-deterministic
-    fn get_imgs(&self, py: Python<'_>) -> PyResult<Vec<Py<coco::Image>>> {
+    fn get_imgs(&self, py: Python<'_>) -> PyResult<Vec<Py<object_detection::Image>>> {
         self.0
             .get_imgs()
             .into_iter()
             .map(|img| Py::new(py, img.clone()))
             .collect()
     }
 
-    fn get_anns(&self, py: Python<'_>) -> PyResult<Vec<Py<coco::Annotation>>> {
+    fn get_anns(&self, py: Python<'_>) -> PyResult<Vec<Py<object_detection::Annotation>>> {
         self.0
             .get_anns()
             .into_iter()
             .map(|ann| Py::new(py, ann.clone()))
             .collect()
     }
 
-    fn get_cats(&self, py: Python<'_>) -> PyResult<Vec<Py<coco::Category>>> {
+    fn get_cats(&self, py: Python<'_>) -> PyResult<Vec<Py<object_detection::Category>>> {
         self.0
             .get_cats()
             .into_iter()
             .map(|cat| Py::new(py, cat.clone()))
             .collect()
     }
 
-    fn get_img_anns(&self, img_id: u32, py: Python<'_>) -> PyResult<Vec<Py<coco::Annotation>>> {
+    fn get_img_anns(
+        &self,
+        img_id: u32,
+        py: Python<'_>,
+    ) -> PyResult<Vec<Py<object_detection::Annotation>>> {
         self.0
             .get_img_anns(img_id)
             .map_err(PyMissingIdError::from)?
             .into_iter()
             .map(|ann| Py::new(py, ann.clone()))
             .collect()
     }
@@ -114,19 +125,46 @@
             .map_err(PyMissingIdError::from)?
             .file_name;
 
         display::img(&img, file_name)
             .map_err(|err| PyValueError::new_err(format!("Failed to display the image: {err}")))?;
         Ok(())
     }
+
+    /// Draw the annotations on the image and returns it as a (RGB) numpy array.
+    ///
+    /// ## Errors
+    ///
+    /// Will return `Err` if the image cannot be drawn (potentially due to it not being in the dataset).
+    pub fn draw_anns<'a>(
+        &self,
+        py: Python<'a>,
+        img_id: u32,
+        draw_bboxes: bool,
+    ) -> PyResult<&'a PyArray3<u8>> {
+        let img = self
+            .0
+            .draw_img_anns(img_id, draw_bboxes)
+            .map_err(|err| match err {
+                CocoError::MissingId(err) => PyKeyError::new_err(err.to_string()),
+                CocoError::Mask(err) => PyValueError::new_err(err.to_string()),
+                CocoError::Loading(err) => PyValueError::new_err(err.to_string()),
+            })?;
+
+        let img = img
+            .into_ndarray3()
+            .permuted_axes([1, 2, 0])
+            .into_pyarray(py);
+        Ok(img)
+    }
 }
 
 #[pyclass(name = "Polygons", module = "rpycocotools.anns")]
 #[derive(Debug)]
-pub struct PyPolygons(cocotools::annotations::coco::Polygons);
+pub struct PyPolygons(pub cocotools::coco::object_detection::Polygons);
 
 #[pymethods]
 impl PyPolygons {
     #[new]
     fn new(counts: Vec<Vec<f64>>) -> Self {
         Self(counts)
     }
```

### Comparing `rpycocotools-0.0.3/src/errors.rs` & `rpycocotools-0.0.4/src/errors.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 // TODO: Try to do a macro to avoid all the boiler plate.
+// TODO: Expose the errors to the python api ? https://pyo3.rs/main/exception
 use pyo3::exceptions::{PyKeyError, PyValueError};
 use pyo3::prelude::*;
 
 use crate::cocotools::errors::{LoadingError, MaskError, MissingIdError};
 
 pub struct PyLoadingError(LoadingError);
```

### Comparing `rpycocotools-0.0.3/src/lib.rs` & `rpycocotools-0.0.4/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+#![allow(clippy::redundant_pub_crate)]
 extern crate cocotools;
 use pyo3::types::PyDict;
 use pyo3::{prelude::*, wrap_pymodule};
 
 pub mod coco;
 pub mod errors;
 pub mod mask;
 
 #[pymodule]
 fn anns(_py: Python<'_>, module: &PyModule) -> PyResult<()> {
-    module.add_class::<cocotools::annotations::coco::Annotation>()?;
-    module.add_class::<cocotools::annotations::coco::Bbox>()?;
-    module.add_class::<cocotools::annotations::coco::Category>()?;
+    module.add_class::<cocotools::coco::object_detection::Annotation>()?;
+    module.add_class::<cocotools::coco::object_detection::Bbox>()?;
+    module.add_class::<cocotools::coco::object_detection::Category>()?;
     module.add_class::<coco::PyPolygons>()?;
-    module.add_class::<cocotools::annotations::coco::PolygonsRS>()?;
-    module.add_class::<cocotools::annotations::coco::Rle>()?;
-    module.add_class::<cocotools::annotations::coco::EncodedRle>()?;
-    module.add_class::<cocotools::annotations::coco::Image>()?;
+    module.add_class::<cocotools::coco::object_detection::PolygonsRS>()?;
+    module.add_class::<cocotools::coco::object_detection::Rle>()?;
+    module.add_class::<cocotools::coco::object_detection::CocoRle>()?;
+    module.add_class::<cocotools::coco::object_detection::Image>()?;
     Ok(())
 }
 
 #[pymodule]
-fn rpycocotools(py: Python<'_>, module: &PyModule) -> PyResult<()> {
+fn _rpycocotools(py: Python<'_>, module: &PyModule) -> PyResult<()> {
     module.add_class::<coco::PyCOCO>()?;
     module.add_wrapped(wrap_pymodule!(anns))?;
     module.add_wrapped(wrap_pymodule!(mask::py_mask))?;
 
     // Inserting to sys.modules allows importing submodules nicely from Python
     // e.g. from rpycocotools.mask import decode_rle
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
-    sys_modules.set_item("rpycocotools.mask", module.getattr("mask")?)?;
-    sys_modules.set_item("rpycocotools.anns", module.getattr("anns")?)?;
+    sys_modules.set_item("_rpycocotools.mask", module.getattr("mask")?)?;
+    sys_modules.set_item("_rpycocotools.anns", module.getattr("anns")?)?;
 
     Ok(())
 }
```

### Comparing `rpycocotools-0.0.3/tests/test_coco.py` & `rpycocotools-0.0.4/tests/test_coco.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import rpycocotools
 from hypothesis import given
 from hypothesis import strategies as st
 
 u32_max = 4_294_967_295
-u32_st =  st.integers(min_value=0, max_value=u32_max)
+u32_st = st.integers(min_value=0, max_value=u32_max)
 
 
 def test_access_cats(coco_dataset: rpycocotools.COCO) -> None:
     cats = coco_dataset.get_cats()
     assert len(cats) == 80
 
 
@@ -24,18 +24,19 @@
     assert len(anns) == 45
 
 
 def test_access_ann(coco_dataset: rpycocotools.COCO) -> None:
     ann = coco_dataset.get_ann(1348739)
     assert ann.id == 1348739
     assert isinstance(ann.segmentation, rpycocotools.anns.PolygonsRS)
-    assert str(ann) == ("Annotation(id=1348739, image_id=174482, category_id=3, segmentation=PolygonsRS(counts="
-                        "[[81.28, 87.23, 82.91, 83.96, 84.0, 76.33, 99.48, 76.22, 105.91, 84.5, 108.09, 93.98, 98.17, "
-                        "93.44, 90.33, 94.2, 85.97, 94.53, 84.0, 94.31]]), area=390.6123, "
-                        "bbox=Bbox(left=81.28, top=76.22, width=26.81, height=18.31), iscrowd=0)")
+    assert str(ann) == ("Annotation(id=1348739, image_id=174482, category_id=3, segmentation=PolygonsRS("
+                        "size=[388, 640], "
+                        "counts=[[81.28, 87.23, 82.91, 83.96, 84.0, 76.33, 99.48, 76.22, 105.91, 84.5, 108.09, "
+                        "93.98, 98.17, 93.44, 90.33, 94.2, 85.97, 94.53, 84.0, 94.31]]), "
+                        "area=390.6123, bbox=BBox(left=81.28, top=76.22, width=26.81, height=18.31), iscrowd=0)")
 
 
 def test_access_imgs(coco_dataset: rpycocotools.COCO) -> None:
     imgs = coco_dataset.get_imgs()
     assert len(imgs) == 4
 
 
@@ -49,30 +50,30 @@
     anns = coco_dataset.get_img_anns(480985)
     assert len(anns) == 13
     assert all(ann.image_id == 480985 for ann in anns)
 
 
 @given(u32_st, u32_st, u32_st, u32_st)
 def test_bbox_create(left: int, top: int, width: int, height: int) -> None:
-    bbox = rpycocotools.anns.Bbox(left, top, width, height)
-    assert isinstance(bbox, rpycocotools.anns.Bbox)
+    bbox = rpycocotools.anns.BBox(left, top, width, height)
+    assert isinstance(bbox, rpycocotools.anns.BBox)
 
 
 @given(u32_st, u32_st, u32_st, u32_st)
 def test_bbox_equality(left: int, top: int, width: int, height: int) -> None:
-    bbox1 = rpycocotools.anns.Bbox(left, top, width, height)
-    bbox2 = rpycocotools.anns.Bbox(left, top, width, height)
+    bbox1 = rpycocotools.anns.BBox(left, top, width, height)
+    bbox2 = rpycocotools.anns.BBox(left, top, width, height)
     assert bbox1 == bbox2
 
 
 @given(st.tuples(st.tuples(u32_st, u32_st, u32_st, u32_st),
                  st.tuples(u32_st, u32_st, u32_st, u32_st)).filter(lambda x: x[0] != x[1]))
 def test_bbox_inequality(coords: tuple[tuple[int, int, int, int], tuple[int, int, int, int]]) -> None:
-    bbox1 = rpycocotools.anns.Bbox(*coords[0])
-    bbox2 = rpycocotools.anns.Bbox(*coords[1])
+    bbox1 = rpycocotools.anns.BBox(*coords[0])
+    bbox2 = rpycocotools.anns.BBox(*coords[1])
     assert bbox1 != bbox2
 
 
 @given(u32_st, u32_st, u32_st, u32_st)
 def test_bbox_repr(left: int, top: int, width: int, height: int) -> None:
-    bbox = rpycocotools.anns.Bbox(left, top, width, height)
-    assert str(bbox) == f"Bbox(left={left}, top={top}, width={width}, height={height})"
+    bbox = rpycocotools.anns.BBox(left, top, width, height)
+    assert str(bbox) == f"BBox(left={left}, top={top}, width={width}, height={height})"
```

### Comparing `rpycocotools-0.0.3/tests/test_mask.py` & `rpycocotools-0.0.4/tests/test_mask.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,51 +2,52 @@
 import numpy.typing as npt
 import pytest
 import rpycocotools
 from hypothesis import strategies as st
 from rpycocotools import mask
 
 u32_max = 4_294_967_295
-u32_st =  st.integers(min_value=0, max_value=u32_max)
+u32_st = st.integers(min_value=0, max_value=u32_max)
 
 
 def test_access_mask(coco_dataset: rpycocotools.COCO) -> None:
     ann = coco_dataset.get_ann(1348739)
     assert isinstance(ann.segmentation, rpycocotools.anns.PolygonsRS)
-    mask = rpycocotools.mask.decode_poly_rs(ann.segmentation)
+    mask = rpycocotools.mask.decode(ann.segmentation)
     assert np.sum(mask) == 423
 
 
 def test_create_mask() -> None:
-    rpycocotools.anns.Rle(size=[4,4], counts=[5, 2, 2, 2, 5])
-    rpycocotools.anns.EncodedRle(size=[4,4], counts="52203")
+    rpycocotools.anns.RLE(size=[4, 4], counts=[5, 2, 2, 2, 5])
+    rpycocotools.anns.COCO_RLE(size=[4, 4], counts="52203")
     rpycocotools.anns.PolygonsRS(size=[7, 7], counts=[[2.0, 1.0, 2.0, 5.0, 4.0, 5.0, 4.0, 1.0]])
     rpycocotools.anns.Polygons([[2.0, 1.0, 2.0, 5.0, 4.0, 5.0, 4.0, 1.0]])
 
 
-@pytest.mark.xfail(reason="Not implemented")
-@pytest.mark.parametrize(("rle", "expected_encoded_rle"),
-                         [(rpycocotools.anns.Rle(size=[4,4], counts=[5, 2, 2, 2, 5]),
-                           rpycocotools.anns.EncodedRle(size=[4,4], counts="52203")),
+# @pytest.mark.xfail(reason="Not implemented")
+@pytest.mark.parametrize(("rle", "expected_coco_rle"),
+                         [(rpycocotools.anns.RLE(size=[4, 4], counts=[5, 2, 2, 2, 5]),
+                           rpycocotools.anns.COCO_RLE(size=[4, 4], counts="52203")),
                           ])
-def test_convert_mask(rle: rpycocotools.anns.Rle, expected_encoded_rle: rpycocotools.anns.EncodedRle) -> None:
-    encoded_rle = rle.to_encoded_rle()  # pyright: ignore
-    assert encoded_rle == expected_encoded_rle
+def test_convert_mask(rle: rpycocotools.anns.RLE, expected_coco_rle: rpycocotools.anns.COCO_RLE) -> None:
+    decoded_mask = mask.decode(rle)
+    coco_rle = mask.encode(decoded_mask, target="coco_rle")
+    assert coco_rle == expected_coco_rle
 
 
 @pytest.mark.parametrize(("rle", "expected_mask"),
-                         [(rpycocotools.anns.Rle(size=[7, 7], counts=[15, 5, 2, 5, 2, 5, 15]),
+                         [(rpycocotools.anns.RLE(size=[7, 7], counts=[15, 5, 2, 5, 2, 5, 15]),
                            np.asarray([[0, 0, 0, 0, 0, 0, 0],
                                        [0, 0, 1, 1, 1, 0, 0],
                                        [0, 0, 1, 1, 1, 0, 0],
                                        [0, 0, 1, 1, 1, 0, 0],
                                        [0, 0, 1, 1, 1, 0, 0],
                                        [0, 0, 1, 1, 1, 0, 0],
                                        [0, 0, 0, 0, 0, 0, 0]])),
                           ])
-def test_decode_rle(rle: rpycocotools.anns.Rle, expected_mask: npt.NDArray[np.uint8]) -> None:
-    decoded_mask = mask.decode_rle(rle)
+def test_decode_rle(rle: rpycocotools.anns.RLE, expected_mask: npt.NDArray[np.uint8]) -> None:
+    decoded_mask = mask.decode(rle)
     assert np.all(decoded_mask == expected_mask)
 
 
 def test_import() -> None:
-    from rpycocotools.mask import decode_encoded_rle  # noqa: F401 # pyright: ignore[reportUnusedImport]
+    from rpycocotools.mask import decode, encode  # noqa: F401 # pyright: ignore[reportUnusedImport]
```

