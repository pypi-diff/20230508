# Comparing `tmp/pep508_rs-0.1.5.tar.gz` & `tmp/pep508_rs-0.2.0.tar.gz`

## Comparing `pep508_rs-0.1.5.tar` & `pep508_rs-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1430 1970-01-01 00:00:00.000000 pep508_rs-0.1.5/Cargo.toml
--rw-r--r--   0      501       20    10173 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/License-Apache
--rw-r--r--   0      501       20     1293 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/License-BSD
--rw-r--r--   0      501       20     3039 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/Readme.md
--rw-r--r--   0      501       20      664 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/pyproject.toml
--rw-r--r--   0      501       20    44277 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/lib.rs
--rw-r--r--   0      501       20    62829 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/marker.rs
--rw-r--r--   0      501       20    14606 2023-04-17 09:58:53.000000 pep508_rs-0.1.5/src/modern.rs
--rw-r--r--   0      501       20    16967 2023-04-17 09:59:46.000000 pep508_rs-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 pep508_rs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 pep508_rs-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20    10173 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/License-Apache
+-rw-r--r--   0      501       20     1293 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/License-BSD
+-rw-r--r--   0      501       20     3039 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/Readme.md
+-rw-r--r--   0      501       20      665 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/pyproject.toml
+-rw-r--r--   0      501       20    44290 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20    64412 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/src/marker.rs
+-rw-r--r--   0      501       20    14602 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/src/modern.rs
+-rw-r--r--   0      501       20    16971 2023-05-08 16:50:03.000000 pep508_rs-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 pep508_rs-0.2.0/PKG-INFO
```

### Comparing `pep508_rs-0.1.5/Cargo.toml` & `pep508_rs-0.2.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "pep508_rs"
-version = "0.1.5"
+version = "0.2.1-beta.2"
 description = "A library for python dependency specifiers, better known as PEP 508"
 edition = "2021"
 include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
 # Same license as pypa/packaging where the tests are from
 license = "Apache-2.0 OR BSD-2-Clause"
 readme = "Readme.md"
 repository = "https://github.com/konstin/pep508_rs"
 
 [dependencies]
 anyhow = { version = "1.0.69", optional = true }
 once_cell = "1.17.1"
-pep440_rs = "0.3.1"
+pep440_rs = "0.3.6"
 pyo3 = { version = "0.18.2", optional = true, features = ["abi3", "extension-module"] }
 pyo3-log = { version = "0.8.0", optional = true }
 regex = { version = "1.7.1", default-features = false, features = ["std"] }
 serde = { version = "1.0.150", features = ["derive"], optional = true }
 serde_json = { version = "1.0.89", optional = true }
 thiserror = "1.0.37"
 toml = { version = "0.7.2", optional = true }
@@ -24,14 +24,15 @@
 unicode-width = "0.1.10"
 url = { version = "2.3.1", features = ["serde"] }
 
 [dev-dependencies]
 indoc = "2.0.0"
 log = "0.4.17"
 testing_logger = "0.1.1"
+serde_json = "1.0.96"
 
 [features]
 pyo3 = ["dep:pyo3", "pep440_rs/pyo3", "pyo3-log"]
 serde = ["dep:serde", "pep440_rs/serde"]
 modern = ["serde", "toml", "anyhow"]
 default = []
```

### Comparing `pep508_rs-0.1.5/License-Apache` & `pep508_rs-0.2.0/License-Apache`

 * *Files identical despite different names*

### Comparing `pep508_rs-0.1.5/License-BSD` & `pep508_rs-0.2.0/License-BSD`

 * *Files identical despite different names*

### Comparing `pep508_rs-0.1.5/Readme.md` & `pep508_rs-0.2.0/Readme.md`

 * *Files identical despite different names*

### Comparing `pep508_rs-0.1.5/src/lib.rs` & `pep508_rs-0.2.0/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 mod marker;
 #[cfg(feature = "modern")]
 pub mod modern;
 
 pub use marker::{
     MarkerEnvironment, MarkerExpression, MarkerOperator, MarkerTree, MarkerValue,
-    MarkerValueString, MarkerValueVersion, MarkerWarningKind,
+    MarkerValueString, MarkerValueVersion, MarkerWarningKind, StringVersion,
 };
 #[cfg(feature = "pyo3")]
 use pep440_rs::PyVersion;
 use pep440_rs::{Version, VersionSpecifier, VersionSpecifiers};
 #[cfg(feature = "pyo3")]
 use pyo3::{
     basic::CompareOp, create_exception, exceptions::PyNotImplementedError, pyclass, pymethods,
@@ -898,15 +898,15 @@
                     ^"
             },
         );
     }
 
     #[test]
     fn basic_examples() {
-        let input = r#"requests[security,tests] >= 2.8.1, == 2.8.* ; python_version < '2.7'"#;
+        let input = r#"requests[security,tests] >=2.8.1, ==2.8.* ; python_version < '2.7'"#;
         let requests = Requirement::from_str(input).unwrap();
         assert_eq!(input, requests.to_string());
         let expected = Requirement {
             name: "requests".to_string(),
             extras: Some(vec!["security".to_string(), "tests".to_string()]),
             version_or_url: Some(VersionOrUrl::VersionSpecifier(
                 [
```

### Comparing `pep508_rs-0.1.5/src/marker.rs` & `pep508_rs-0.2.0/src/marker.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 
 use crate::{CharIter, Pep508Error, Pep508ErrorSource};
 use pep440_rs::{Version, VersionSpecifier};
 #[cfg(feature = "pyo3")]
 use pyo3::{
     basic::CompareOp, exceptions::PyValueError, pyclass, pymethods, PyAny, PyResult, Python,
 };
+#[cfg(feature = "serde")]
+use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
 use std::collections::HashSet;
 use std::fmt::{Display, Formatter};
+use std::ops::Deref;
 use std::str::FromStr;
 use tracing::warn;
 
 /// Ways in which marker evaluation can fail
 #[cfg_attr(feature = "pyo3", pyclass(module = "pep508"))]
 #[derive(Debug, Eq, Hash, Ord, PartialOrd, PartialEq, Clone, Copy)]
 pub enum MarkerWarningKind {
@@ -282,44 +285,94 @@
             Self::TildeEqual => "~=",
             Self::In => "in",
             Self::NotIn => "not in",
         })
     }
 }
 
+/// Helper type with a [Version] and its original text
+#[cfg_attr(feature = "pyo3", pyclass(get_all, module = "pep508"))]
+#[derive(Clone, Debug, Eq, Hash, PartialEq)]
+pub struct StringVersion {
+    /// Original unchanged string
+    pub string: String,
+    /// Parsed version
+    pub version: Version,
+}
+
+impl FromStr for StringVersion {
+    type Err = String;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        Ok(Self {
+            string: s.to_string(),
+            version: Version::from_str(s)?,
+        })
+    }
+}
+
+#[cfg(feature = "serde")]
+impl Serialize for StringVersion {
+    fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
+    where
+        S: Serializer,
+    {
+        serializer.serialize_str(&self.string)
+    }
+}
+
+#[cfg(feature = "serde")]
+impl<'de> Deserialize<'de> for StringVersion {
+    fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
+    where
+        D: Deserializer<'de>,
+    {
+        let string = String::deserialize(deserializer)?;
+        Self::from_str(&string).map_err(de::Error::custom)
+    }
+}
+
+impl Deref for StringVersion {
+    type Target = Version;
+
+    fn deref(&self) -> &Self::Target {
+        &self.version
+    }
+}
+
 /// The marker values for a python interpreter, normally the current one
 ///
 /// <https://packaging.python.org/en/latest/specifications/dependency-specifiers/#environment-markers>
 ///
 /// Some are `(String, Version)` because we have to support version comparison
 #[allow(missing_docs)]
-#[cfg_attr(feature = "serde", derive(serde::Deserialize))]
+#[cfg_attr(feature = "serde", derive(serde::Deserialize, serde::Serialize))]
 #[cfg_attr(feature = "pyo3", pyclass(get_all, module = "pep508"))]
 #[derive(Clone, Debug, Eq, Hash, PartialEq)]
 pub struct MarkerEnvironment {
     pub implementation_name: String,
-    pub implementation_version: (String, Version),
+    pub implementation_version: StringVersion,
     pub os_name: String,
     pub platform_machine: String,
     pub platform_python_implementation: String,
     pub platform_release: String,
     pub platform_system: String,
     pub platform_version: String,
-    pub python_full_version: (String, Version),
-    pub python_version: (String, Version),
+    pub python_full_version: StringVersion,
+    pub python_version: StringVersion,
     pub sys_platform: String,
 }
 
 impl MarkerEnvironment {
     /// Returns of the PEP 440 version typed value of the key in the current environment
     fn get_version(&self, key: &MarkerValueVersion) -> &Version {
         match key {
-            MarkerValueVersion::ImplementationVersion => &self.implementation_version.1,
-            MarkerValueVersion::PythonFullVersion => &self.python_full_version.1,
-            MarkerValueVersion::PythonVersion => &self.python_version.1,
+            MarkerValueVersion::ImplementationVersion => &self.implementation_version.version,
+            MarkerValueVersion::PythonFullVersion => &self.python_full_version.version,
+            MarkerValueVersion::PythonVersion => &self.python_version.version,
         }
     }
 
     /// Returns of the stringly typed value of the key in the current environment
     fn get_string(&self, key: &MarkerValueString) -> &str {
         match key {
             MarkerValueString::ImplementationName => &self.implementation_name,
@@ -371,47 +424,44 @@
         platform_release: &str,
         platform_system: &str,
         platform_version: &str,
         python_full_version: &str,
         python_version: &str,
         sys_platform: &str,
     ) -> PyResult<Self> {
-        let implementation_version_pep440 =
-            Version::from_str(implementation_version).map_err(|err| {
+        let implementation_version =
+            StringVersion::from_str(implementation_version).map_err(|err| {
                 PyValueError::new_err(format!(
                     "implementation_version is not a valid PEP440 version: {}",
                     err
                 ))
             })?;
-        let python_full_version_pep440 = Version::from_str(python_full_version).map_err(|err| {
+        let python_full_version = StringVersion::from_str(python_full_version).map_err(|err| {
             PyValueError::new_err(format!(
                 "python_full_version is not a valid PEP440 version: {}",
                 err
             ))
         })?;
-        let python_version_pep440 = Version::from_str(python_version).map_err(|err| {
+        let python_version = StringVersion::from_str(python_version).map_err(|err| {
             PyValueError::new_err(format!(
                 "python_version is not a valid PEP440 version: {}",
                 err
             ))
         })?;
         Ok(Self {
             implementation_name: implementation_name.to_string(),
-            implementation_version: (
-                implementation_version.to_string(),
-                implementation_version_pep440,
-            ),
+            implementation_version,
             os_name: os_name.to_string(),
             platform_machine: platform_machine.to_string(),
             platform_python_implementation: platform_python_implementation.to_string(),
             platform_release: platform_release.to_string(),
             platform_system: platform_system.to_string(),
             platform_version: platform_version.to_string(),
-            python_full_version: (python_full_version.to_string(), python_full_version_pep440),
-            python_version: (python_version.to_string(), python_version_pep440),
+            python_full_version,
+            python_version,
             sys_platform: sys_platform.to_string(),
         })
     }
 
     /// Query the current python interpreter to get the correct marker value
     #[staticmethod]
     fn current(py: Python<'_>) -> PyResult<Self> {
@@ -443,53 +493,53 @@
                 "".to_string()
             }
         );
         let python_full_version: String = platform.getattr("python_version")?.call0()?.extract()?;
         let python_version = format!("{}.{}", python_version_tuple.0, python_version_tuple.1);
 
         // This is not written down in PEP 508, but it's the only reasonable assumption to make
-        let implementation_version_pep440 =
-            Version::from_str(&implementation_version).map_err(|err| {
+        let implementation_version =
+            StringVersion::from_str(&implementation_version).map_err(|err| {
                 PyValueError::new_err(format!(
                     "Broken python implementation, implementation_version is not a valid PEP440 version: {}",
                     err
                 ))
             })?;
-        let python_full_version_pep440 = Version::from_str(&python_full_version).map_err(|err| {
+        let python_full_version = StringVersion::from_str(&python_full_version).map_err(|err| {
             PyValueError::new_err(format!(
                 "Broken python implementation, python_full_version is not a valid PEP440 version: {}",
                 err
             ))
         })?;
-        let python_version_pep440 = Version::from_str(&python_version).map_err(|err| {
+        let python_version = StringVersion::from_str(&python_version).map_err(|err| {
             PyValueError::new_err(format!(
                 "Broken python implementation, python_version is not a valid PEP440 version: {}",
                 err
             ))
         })?;
         Ok(Self {
             implementation_name: format!(
                 "{}.{}.{}{}",
                 py.version_info().major,
                 py.version_info().minor,
                 py.version_info().patch,
                 py.version_info().suffix.unwrap_or_default()
             ),
-            implementation_version: (implementation_version, implementation_version_pep440),
+            implementation_version,
             os_name: os.getattr("name")?.extract()?,
             platform_machine: platform.getattr("machine")?.call0()?.extract()?,
             platform_python_implementation: platform
                 .getattr("python_implementation")?
                 .call0()?
                 .extract()?,
             platform_release: platform.getattr("release")?.call0()?.extract()?,
             platform_system: platform.getattr("system")?.call0()?.extract()?,
             platform_version: platform.getattr("version")?.call0()?.extract()?,
-            python_full_version: (python_full_version, python_full_version_pep440),
-            python_version: (python_version, python_version_pep440),
+            python_full_version,
+            python_version,
             sys_platform: sys.getattr("platform")?.extract()?,
         })
     }
 }
 
 /// Represents one clause such as `python_version > "3.8"` in the form
 /// ```text
@@ -1279,39 +1329,38 @@
 fn parse_markers(markers: &str) -> Result<MarkerTree, Pep508Error> {
     let mut chars = CharIter::new(markers);
     parse_markers_impl(&mut chars)
 }
 
 #[cfg(test)]
 mod test {
-    use crate::marker::MarkerEnvironment;
+    use crate::marker::{MarkerEnvironment, StringVersion};
     use crate::{MarkerExpression, MarkerOperator, MarkerTree, MarkerValue, MarkerValueString};
     use indoc::indoc;
     use log::Level;
-    use pep440_rs::Version;
     use std::str::FromStr;
 
     fn assert_err(input: &str, error: &str) {
         assert_eq!(MarkerTree::from_str(input).unwrap_err().to_string(), error);
     }
 
     fn env37() -> MarkerEnvironment {
-        let v37 = Version::from_str("3.7").unwrap();
+        let v37 = StringVersion::from_str("3.7").unwrap();
 
         MarkerEnvironment {
             implementation_name: "".to_string(),
-            implementation_version: ("3.7".to_string(), v37.clone()),
+            implementation_version: v37.clone(),
             os_name: "linux".to_string(),
             platform_machine: "".to_string(),
             platform_python_implementation: "".to_string(),
             platform_release: "".to_string(),
             platform_system: "".to_string(),
             platform_version: "".to_string(),
-            python_full_version: ("3.7".to_string(), v37.clone()),
-            python_version: ("3.7".to_string(), v37),
+            python_full_version: v37.clone(),
+            python_version: v37,
             sys_platform: "linux".to_string(),
         }
     }
 
     /// Copied from <https://github.com/pypa/packaging/blob/85ff971a250dc01db188ef9775499c15553a8c95/tests/test_markers.py#L175-L221>
     #[test]
     fn test_marker_equivalence() {
@@ -1349,26 +1398,26 @@
                 b
             );
         }
     }
 
     #[test]
     fn test_marker_evaluation() {
-        let v27 = Version::from_str("2.7").unwrap();
+        let v27 = StringVersion::from_str("2.7").unwrap();
         let env27 = MarkerEnvironment {
             implementation_name: "".to_string(),
-            implementation_version: ("2.7".to_string(), v27.clone()),
+            implementation_version: v27.clone(),
             os_name: "linux".to_string(),
             platform_machine: "".to_string(),
             platform_python_implementation: "".to_string(),
             platform_release: "".to_string(),
             platform_system: "".to_string(),
             platform_version: "".to_string(),
-            python_full_version: ("2.7".to_string(), v27.clone()),
-            python_version: ("2.7".to_string(), v27),
+            python_full_version: v27.clone(),
+            python_version: v27,
             sys_platform: "linux".to_string(),
         };
         let env37 = env37();
         let marker1 = MarkerTree::from_str("python_version == '2.7'").unwrap();
         let marker2 = MarkerTree::from_str(
             "os_name == \"linux\" or python_version == \"3.7\" and sys_platform == \"win32\"",
         )
@@ -1510,8 +1559,29 @@
             indoc! {r#"
                 Unexpected character 'a', expected end of input
                 os_name == "nt" and python_version >= "3.8"
                                 ^^^^^^^^^^^^^^^^^^^^^^^^^^"#
             },
         );
     }
+
+    #[cfg(feature = "serde")]
+    #[test]
+    fn test_marker_environment_from_json() {
+        let _env: MarkerEnvironment = serde_json::from_str(
+            r##"{
+                "implementation_name": "cpython", 
+                "implementation_version": "3.7.13",
+                "os_name": "posix",
+                "platform_machine": "x86_64",
+                "platform_python_implementation": "CPython",
+                "platform_release": "5.4.188+",
+                "platform_system": "Linux",
+                "platform_version": "#1 SMP Sun Apr 24 10:03:06 PDT 2022",
+                "python_full_version": "3.7.13",
+                "python_version": "3.7",
+                "sys_platform": "linux"
+            }"##,
+        )
+        .unwrap();
+    }
 }
```

### Comparing `pep508_rs-0.1.5/src/modern.rs` & `pep508_rs-0.2.0/src/modern.rs`

 * *Files 2% similar despite different names*

```diff
@@ -323,16 +323,16 @@
             modern_dependencies: BTreeMap<String, RequirementModern>,
             extras: HashMap<String, Vec<String>>,
         }
 
         let pyproject_toml = indoc! {r#"
             [modern-dependencies]
             pydantic = "1.10.5"
-            numpy = ">=1.24.2,<2.0.0"
-            pandas = { version = ">=1.5.3,<2.0.0" }
+            numpy = ">=1.24.2, <2.0.0"
+            pandas = { version = ">=1.5.3, <2.0.0" }
             flask = { version = "2.2.3 ", extras = ["dotenv"], optional = true }
             tqdm = { git = "https://github.com/tqdm/tqdm", rev = "0bb91857eca0d4aea08f66cf1c8949abe0cd6b7a" }
             jax = { url = "https://storage.googleapis.com/jax-releases/cuda112/jaxlib-0.1.64+cuda112-cp39-none-manylinux2010_x86_64.whl" }
             zstandard = { file = "/home/ferris/wheels/zstandard/zstandard-0.20.0.tar.gz" }
             h5py = { path = "/home/ferris/wheels/h5py/" }
 
             [extras]
@@ -344,19 +344,19 @@
 
         let actual: Vec<String> = deps
             .modern_dependencies
             .iter()
             .map(|(name, spec)| spec.to_pep508(name, &deps.extras).unwrap().to_string())
             .collect();
         let expected: Vec<String> = vec![
-            "flask[dotenv] == 2.2.3 ; extra == 'internet'".to_string(),
+            "flask[dotenv] ==2.2.3 ; extra == 'internet'".to_string(),
             "h5py @ file:///home/ferris/wheels/h5py/".to_string(),
             "jax @ https://storage.googleapis.com/jax-releases/cuda112/jaxlib-0.1.64+cuda112-cp39-none-manylinux2010_x86_64.whl".to_string(),
-            "numpy >= 1.24.2, < 2.0.0".to_string(),
-            "pandas >= 1.5.3, < 2.0.0".to_string(),
-            "pydantic == 1.10.5".to_string(),
+            "numpy >=1.24.2, <2.0.0".to_string(),
+            "pandas >=1.5.3, <2.0.0".to_string(),
+            "pydantic ==1.10.5".to_string(),
             "tqdm @ git+https://github.com/tqdm/tqdm@0bb91857eca0d4aea08f66cf1c8949abe0cd6b7a".to_string(),
             "zstandard @ file:///home/ferris/wheels/zstandard/zstandard-0.20.0.tar.gz".to_string()
         ];
         assert_eq!(actual, expected)
     }
 }
```

### Comparing `pep508_rs-0.1.5/Cargo.lock` & `pep508_rs-0.2.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
@@ -98,17 +98,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -167,29 +167,29 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.5"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aac177a025c60a4dd25d638bf33e746d1ead5f7123f6650f35b4394c7ce1a104"
+checksum = "4b962c30be0b372ef828da212d99a1f18b6726ef312b022ddbc6970ed1876c16"
 dependencies = [
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
  "unicode-width",
 ]
 
 [[package]]
 name = "pep508_rs"
-version = "0.1.5"
+version = "0.2.1-beta.2"
 dependencies = [
  "anyhow",
  "indoc 2.0.1",
  "log",
  "once_cell",
  "pep440_rs",
  "pyo3",
@@ -295,17 +295,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -313,28 +313,28 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
@@ -342,26 +342,26 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.162"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
@@ -410,17 +410,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "testing_logger"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d92b727cb45d33ae956f7f46b966b25f1bc712092aeef9dba5ac798fc89f720"
 dependencies = [
@@ -507,21 +507,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
@@ -638,13 +638,13 @@
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
```

### Comparing `pep508_rs-0.1.5/PKG-INFO` & `pep508_rs-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pep508_rs
-Version: 0.1.5
+Version: 0.2.0
 Summary: A library for python dependency specifiers, better known as PEP 508
 License: Apache-2.0 OR BSD-2-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/konstin/pep508_rs
 
 # Dependency specifiers (PEP 508) in Rust
```

