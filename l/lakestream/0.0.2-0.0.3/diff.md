# Comparing `tmp/lakestream-0.0.2.tar.gz` & `tmp/lakestream-0.0.3.tar.gz`

## Comparing `lakestream-0.0.2.tar` & `lakestream-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,67 @@
--rw-r--r--   0        0        0     1541 1970-01-01 00:00:00.000000 lakestream-0.0.2/local_dependencies/lakestream/Cargo.toml
--rw-r--r--   0      501       20     9549 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/filters.rs
--rw-r--r--   0      501       20     8978 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/interfaces.rs
--rw-r--r--   0      501       20       37 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/base/mod.rs
--rw-r--r--   0      501       20     2585 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/ls_command.rs
--rw-r--r--   0      501       20       32 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/mod.rs
--rw-r--r--   0      501       20     2897 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/cli/parser.rs
--rw-r--r--   0      501       20       94 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/default.rs
--rw-r--r--   0      501       20      135 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/mod.rs
--rw-r--r--   0      501       20     2129 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/requests.rs
--rw-r--r--   0      501       20      472 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/http/requests_wasm32.rs
--rw-r--r--   0      501       20      368 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/lib.rs
--rw-r--r--   0      501       20     1095 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/bucket.rs
--rw-r--r--   0      501       20     2830 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/list.rs
--rw-r--r--   0      501       20       26 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/localfs/mod.rs
--rw-r--r--   0      501       20      125 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/main.rs
--rw-r--r--   0      501       20     1459 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/bucket.rs
--rw-r--r--   0      501       20     8602 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/client.rs
--rw-r--r--   0      501       20     1127 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/config.rs
--rw-r--r--   0      501       20    13869 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/list.rs
--rw-r--r--   0      501       20       50 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/s3/mod.rs
--rw-r--r--   0      501       20     1036 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/formatters.rs
--rw-r--r--   0      501       20      200 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/mod.rs
--rw-r--r--   0      501       20     1031 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time.rs
--rw-r--r--   0      501       20     1779 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse.rs
--rw-r--r--   0      501       20      689 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse_ext.rs
--rw-r--r--   0      501       20      370 2023-04-23 21:04:46.000000 lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse_ext_wasm32.rs
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 lakestream-0.0.2/Cargo.toml
--rw-r--r--   0      501       20      300 2023-04-23 21:04:46.000000 lakestream-0.0.2/Makefile
--rw-r--r--   0      501       20     3393 2023-04-23 21:04:46.000000 lakestream-0.0.2/README.rst
--rw-r--r--   0      501       20     1794 2023-04-23 21:04:46.000000 lakestream-0.0.2/lakestream/__init__.py
--rw-r--r--   0      501       20      165 2023-04-23 21:04:46.000000 lakestream-0.0.2/lakestream/__main__.py
--rw-r--r--   0      501       20      991 2023-04-23 21:04:47.000000 lakestream-0.0.2/pyproject.toml
--rw-r--r--   0      501       20     4312 2023-04-23 21:04:46.000000 lakestream-0.0.2/src/lib.rs
--rw-r--r--   0      501       20    68929 2023-04-23 21:05:49.000000 lakestream-0.0.2/Cargo.lock
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 lakestream-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/Cargo.toml
+-rw-r--r--   0      501       20        2 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/output
+-rw-r--r--   0      501       20       77 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/lib.rs
+-rw-r--r--   0      501       20      129 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/main.rs
+-rw-r--r--   0      501       20     1967 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/parser.rs
+-rw-r--r--   0      501       20      529 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/cp.rs
+-rw-r--r--   0      501       20      283 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/cp_handler.rs
+-rw-r--r--   0      501       20     1733 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/ls.rs
+-rw-r--r--   0      501       20     3820 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/ls_handler.rs
+-rw-r--r--   0      501       20       94 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/mod.rs
+-rw-r--r--   0      501       20      587 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/request.rs
+-rw-r--r--   0      501       20     1916 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/request_handler.rs
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 lakestream-0.0.3/local_dependencies/lakestream/Cargo.toml
+-rw-r--r--   0      501       20     1438 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/build.rs
+-rw-r--r--   0      501       20       30 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/api/mod.rs
+-rw-r--r--   0      501       20     5747 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/api/object_store_handler.rs
+-rw-r--r--   0      501       20     3712 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/callback_wrapper.rs
+-rw-r--r--   0      501       20      897 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/config.rs
+-rw-r--r--   0      501       20     3137 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/file_object.rs
+-rw-r--r--   0      501       20     9556 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/filters.rs
+-rw-r--r--   0      501       20      135 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/list_objects_result.rs
+-rw-r--r--   0      501       20      161 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/mod.rs
+-rw-r--r--   0      501       20     7591 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/object_store.rs
+-rw-r--r--   0      501       20     2072 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/base/object_store_helpers.rs
+-rw-r--r--   0      501       20       94 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/default.rs
+-rw-r--r--   0      501       20     2144 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/error.rs
+-rw-r--r--   0      501       20      135 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/http/mod.rs
+-rw-r--r--   0      501       20     2663 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/http/requests.rs
+-rw-r--r--   0      501       20     2542 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/http/requests_wasm32.rs
+-rw-r--r--   0      501       20      682 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/lib.rs
+-rw-r--r--   0      501       20      499 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/localfs/backend.rs
+-rw-r--r--   0      501       20     1927 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/localfs/bucket.rs
+-rw-r--r--   0      501       20      930 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/localfs/get.rs
+-rw-r--r--   0      501       20     2929 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/localfs/list.rs
+-rw-r--r--   0      501       20       85 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/localfs/mod.rs
+-rw-r--r--   0      501       20     1101 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/backend.rs
+-rw-r--r--   0      501       20     2719 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/bucket.rs
+-rw-r--r--   0      501       20     1217 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/client.rs
+-rw-r--r--   0      501       20     1173 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/client_config.rs
+-rw-r--r--   0      501       20     3189 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/client_headers.rs
+-rw-r--r--   0      501       20     1925 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/config.rs
+-rw-r--r--   0      501       20      845 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/get.rs
+-rw-r--r--   0      501       20     7003 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/list.rs
+-rw-r--r--   0      501       20      178 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/mod.rs
+-rw-r--r--   0      501       20     3713 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/parse_http_response.rs
+-rw-r--r--   0      501       20     6806 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/request_builder.rs
+-rw-r--r--   0      501       20     2244 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/s3/request_handler.rs
+-rw-r--r--   0      501       20     1895 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/backend_parse.rs
+-rw-r--r--   0      501       20     1036 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/formatters.rs
+-rw-r--r--   0      501       20      219 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/mod.rs
+-rw-r--r--   0      501       20     1031 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/time.rs
+-rw-r--r--   0      501       20     1676 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/time_parse.rs
+-rw-r--r--   0      501       20      689 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/time_parse_ext.rs
+-rw-r--r--   0      501       20      878 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/time_parse_ext_wasm32.rs
+-rw-r--r--   0      501       20     3079 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/src/utils/uri_parse.rs
+-rw-r--r--   0      501       20     1555 2023-05-07 21:33:13.000000 lakestream-0.0.3/local_dependencies/lakestream/tests/localfs_tests.rs
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 lakestream-0.0.3/Cargo.toml
+-rw-r--r--   0      501       20      300 2023-05-07 21:33:13.000000 lakestream-0.0.3/Makefile
+-rw-r--r--   0      501       20     3393 2023-05-07 21:33:13.000000 lakestream-0.0.3/README.rst
+-rw-r--r--   0      501       20     2727 2023-05-07 21:33:13.000000 lakestream-0.0.3/lakestream/__init__.py
+-rw-r--r--   0      501       20      165 2023-05-07 21:33:13.000000 lakestream-0.0.3/lakestream/__main__.py
+-rw-r--r--   0      501       20      991 2023-05-07 21:33:13.000000 lakestream-0.0.3/pyproject.toml
+-rw-r--r--   0      501       20     5696 2023-05-07 21:33:13.000000 lakestream-0.0.3/src/client.rs
+-rw-r--r--   0      501       20      396 2023-05-07 21:33:13.000000 lakestream-0.0.3/src/lib.rs
+-rw-r--r--   0      501       20     1415 2023-05-07 21:33:13.000000 lakestream-0.0.3/src/utils.rs
+-rw-r--r--   0      501       20    85069 2023-05-07 21:34:46.000000 lakestream-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 lakestream-0.0.3/PKG-INFO
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/Cargo.toml` & `lakestream-0.0.3/local_dependencies/lakestream/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 [package]
 name = "lakestream"
-version = "0.0.2"
+# version is auto-updated via lakestream/build.rs
+version = "0.0.3"
 authors = ["Anthony Potappel <aprxi@lakestream.dev>"]
 edition = "2021"
 
 description = "Portable file-utility for object-stores"
 documentation = "https://docs.rs/lakestream"
 homepage = "https://lakestream.dev"
 repository = "https://github.com/serverlessnext/lakestream"
 readme = "../README.rst"
 license = "MIT"
 
-
 [lib]
 name = "lakestream"
 path = "src/lib.rs"
 
-[[bin]]
-name = "lakestream"
-path = "src/main.rs"
-
 [dependencies]
 percent-encoding = { version = "2.1", default-features = false, features = ["alloc"] }
 hex = { version = "0.4.3", default-features = false, features = ["alloc"] }
-serde = { version = "1.0", features = ["derive", "alloc"] }
+serde = { version = "1.0", features = ["derive"] }
 hmac = { version = "0.11", default-features = false }
 sha2 = { version = "0.9.9", default-features = false }
-serde_json = {version = "1.0", default-features = false, features = ["alloc"]}
-regex = { version = "1.7", default-features = false, features = ["std", "unicode"] }
-itertools = "0.10"
-serde-xml-rs = "0.6"
+regex = { version = "1.8", default-features = false, features = ["std", "unicode"] }
+futures = { version = "0.3", default-features = false }
 url = "2.3"
-clap = { version = "4.2" , default-features = false, features = ["std", "help"]}
+log = "0.4"
+serde-xml-rs = "0.6"
+async-trait = "0.1"
 
 [target.'cfg(not(target_arch = "wasm32"))'.dependencies]
 time = { version = "0.3", features = ["parsing"]}
-ureq = { version = "2.2", default-features = false, features = ["tls"]}
-
-# [target.'cfg(target_arch = "wasm32")'.dependencies]
-# js-sys = "0.3"
-# web-sys = { version = "0.3", features = ['Request', 'RequestInit', 'RequestMode', 'Headers', 'Window', 'Response', 'console'] }
-# wasm-bindgen = "0.2.84"
-# wasm-bindgen-futures = "0.4"
-
+hyper = { version = "0.14", default-features = false, features = ["client", "http1", "http2"]}
+hyper-tls = { version = "0.5" }
+native-tls = { version = "0.2" }
+openssl-sys = { version = "0.9", features = ["vendored"] }
+tokio-native-tls = { version = "0.3" }
+
+[target.'cfg(target_arch = "wasm32")'.dependencies]
+js-sys = "0.3"
+web-sys = { version = "0.3", features = ['Request', 'RequestInit', 'RequestMode', 'Headers', 'Window', 'Response', 'console'] }
+wasm-bindgen-futures = "0.4"
+wasm-bindgen = "0.2.84"
+
+[build-dependencies]
+toml_edit = "0.2"
+
+[dev-dependencies]
+# keep tokio version+features in sync with lakestream-cli
+tokio = { version = "1.12", default-features = false, features = ["rt-multi-thread", "macros"] }
+tempfile = "3.5.0"
+
+[profile.release]
+lto = true
+opt-level = 3
+panic = "abort"
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/base/filters.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/base/filters.rs`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             .map(|(_, m)| m)
             .unwrap_or(&1u64);
 
         let min_size = min_value * multiplier1;
         let max_size = max_value * multiplier2;
 
         if min_size > max_size {
-            Err(format!("Minimum size is greater than maximum size."))
+            Err("Minimum size is greater than maximum size.".to_string())
         } else {
             Ok((Some(min_size), Some(max_size)))
         }
     } else if let Some(caps) = re.captures(size) {
         let modifier = &caps["modifier"];
         let value: u64 = caps["value"].parse().expect("Invalid numeric value");
         let unit = caps["unit"].to_ascii_lowercase();
@@ -143,15 +143,15 @@
     current_time: u64,
 ) -> Result<(Option<u64>, Option<u64>), String> {
     let is_negative = time_offset_str.starts_with('-');
     let is_positive = time_offset_str.starts_with('+');
 
     if time_offset_str
         .chars()
-        .any(|c| !c.is_digit(10) && !"+-YMWDhms".contains(c))
+        .any(|c| !c.is_ascii_digit() && !"+-YMWDhms".contains(c))
     {
         return Err(format!("Invalid time offset string: {}", time_offset_str));
     }
 
     let time_offset_str = if is_negative || is_positive {
         &time_offset_str[1..]
     } else {
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/cli/ls_command.rs` & `lakestream-0.0.3/local_dependencies/lakestream-cli/src/subcommands/ls_handler.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,88 @@
-use std::collections::HashMap;
-
-use crate::{FileObjectFilter, ListObjectsResult, ObjectStoreHandler};
-
-pub fn handle_ls(ls_matches: &clap::ArgMatches, region: Option<String>) {
-    let (uri, config, recursive, max_files, filter) =
-        prepare_handle_ls_arguments(ls_matches, region);
-
-    match ObjectStoreHandler::list_objects(
-        uri,
-        config,
-        recursive,
-        Some(max_files),
-        &filter,
-    ) {
-        ListObjectsResult::FileObjects(file_objects) => {
-            // Print file objects to stdout
-            println!("Found {} file objects:", file_objects.len());
-            for fo in file_objects {
-                let full_path = true;
-                println!("{}", fo.printable(full_path));
-            }
+use lakestream::{
+    CallbackItem, CallbackWrapper, Config, FileObjectFilter, LakestreamError,
+    ListObjectsResult, ObjectStoreHandler,
+};
+use log::info;
+
+pub async fn handle_ls(ls_matches: &clap::ArgMatches, config: &mut Config) {
+    let (uri, recursive, max_files, filter) =
+        prepare_handle_ls_arguments(ls_matches);
+
+    let handler = ObjectStoreHandler::new(None);
+
+    let callback =
+        Some(CallbackWrapper::create_async(print_callback_items_async));
+
+    match handler
+        .list_objects(
+            &uri,
+            config,
+            recursive,
+            Some(max_files),
+            &filter,
+            callback,
+        )
+        .await
+    {
+        Ok(Some(list_objects_result)) => {
+            handle_list_objects_result(list_objects_result).await;
+        }
+        Ok(None) => {
+            println!("Done");
         }
+        Err(LakestreamError::NoBucketInUri(_)) => {
+            handle_list_buckets(&uri, config).await;
+        }
+        Err(err) => {
+            eprintln!("Error: {:?}", err);
+        }
+    }
+}
+
+async fn handle_list_objects_result(list_objects_result: ListObjectsResult) {
+    match list_objects_result {
         ListObjectsResult::Buckets(buckets) => {
             // Print buckets to stdout
-            println!("Found {} buckets:", buckets.len());
+            info!("Found {} buckets:", buckets.len());
             for bucket in buckets {
                 println!("{}", bucket.name());
             }
         }
+        ListObjectsResult::FileObjects(file_objects) => {
+            // Print file objects to stdout
+            info!("Found {} file objects:", file_objects.len());
+            for fo in file_objects {
+                println!("{}", fo.println_path());
+            }
+        }
+    }
+}
+
+async fn handle_list_buckets(uri: &str, config: &Config) {
+    log::info!("Calling list_buckets");
+    let handler = ObjectStoreHandler::new(None);
+    let callback =
+        Some(CallbackWrapper::create_async(print_callback_items_async));
+    match handler.list_buckets(uri, config, callback).await {
+        Ok(Some(list_objects_result)) => {
+            handle_list_objects_result(list_objects_result).await;
+        }
+        Ok(None) => {
+            log::info!("Done");
+        }
+        Err(err) => {
+            eprintln!("Error: {:?}", err);
+        }
     }
 }
 
 fn prepare_handle_ls_arguments(
     ls_matches: &clap::ArgMatches,
-    region: Option<String>,
-) -> (
-    String,
-    HashMap<String, String>,
-    bool,
-    u32,
-    Option<FileObjectFilter>,
-) {
+) -> (String, bool, u32, Option<FileObjectFilter>) {
     let recursive = *ls_matches.get_one::<bool>("recursive").unwrap_or(&false);
     let uri = ls_matches.get_one::<String>("uri").unwrap().to_string();
 
     let filter_name = ls_matches
         .get_one::<String>("name")
         .map(ToString::to_string);
     let filter_size = ls_matches
@@ -74,14 +112,16 @@
 
     let max_files = ls_matches
         .get_one::<String>("max_files")
         .unwrap()
         .parse::<u32>()
         .expect("Invalid value for max_files");
 
-    let mut config = HashMap::new();
-    if let Some(region) = region {
-        config.insert("region".to_string(), region);
-    }
+    (uri, recursive, max_files, filter)
+}
 
-    (uri, config, recursive, max_files, filter)
+async fn print_callback_items_async<T: CallbackItem>(items: Vec<T>) {
+    info!("Found {} items:", items.len());
+    for item in &items {
+        println!("{}", item.println_path());
+    }
 }
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/http/requests.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/http/requests.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,83 @@
 use std::collections::HashMap;
 use std::error::Error;
-use std::io::Read;
+use std::str::FromStr;
 
-use ureq::{Agent, Response};
+use hyper::client::HttpConnector;
+use hyper::header::{HeaderName, HeaderValue};
+use hyper::{Body, Client, Request};
+use hyper_tls::HttpsConnector;
+use native_tls::TlsConnector as NativeTlsConnector;
+use tokio_native_tls::TlsConnector;
+use url::Url;
+
+type HttpResult =
+    Result<(String, u16, HashMap<String, String>), Box<dyn Error>>;
+type HttpResultWithoutHeaders = Result<(String, u16), Box<dyn Error>>;
 
-type ResponseData = (String, u16, HashMap<String, String>);
-type HttpResult = Result<ResponseData, Box<dyn Error>>;
-type ResponseDataWithoutHeaders = (String, u16);
-type HttpResultWithoutHeaders =
-    Result<ResponseDataWithoutHeaders, Box<dyn Error>>;
-
-pub fn http_get_request(
+pub async fn http_get_request(
     url: &str,
     headers: &HashMap<String, String>,
 ) -> HttpResultWithoutHeaders {
-    let response = perform_request(url, headers)?;
-    let status = response.status();
-
-    if !(200..300).contains(&status) {
-        return Ok((String::new(), status));
-    }
-    let mut body = String::new();
-    response.into_reader().read_to_string(&mut body)?;
+    let (body, status, _) = http_get_request_with_headers(url, headers).await?;
     Ok((body, status))
 }
 
-pub fn http_get_request_with_headers(
+pub async fn http_get_request_with_headers(
     url: &str,
     headers: &HashMap<String, String>,
 ) -> HttpResult {
-    let response = perform_request(url, headers)?;
-    let status = response.status();
+    let url_u = Url::parse(url)?;
+    let accept_invalid_certs = url_u.scheme() == "https"
+        && url_u.host_str() == Some("localhost")
+        && url_u.port().map_or(true, |port| port > 0);
+
+    let mut native_tls_connector_builder = NativeTlsConnector::builder();
+    native_tls_connector_builder
+        .danger_accept_invalid_certs(accept_invalid_certs);
+    let native_tls_connector = native_tls_connector_builder.build().unwrap();
+
+    let tls_connector = TlsConnector::from(native_tls_connector);
+
+    let mut http_connector = HttpConnector::new();
+    http_connector.enforce_http(false);
+
+    let https = HttpsConnector::from((http_connector, tls_connector));
+    let client = Client::builder().build::<_, Body>(https);
+
+    let mut request = Request::get(url).body(Body::empty())?;
+    for (key, value) in headers.iter() {
+        if let (Ok(header_name), Ok(header_value)) =
+            (HeaderName::from_str(key), HeaderValue::from_str(value))
+        {
+            request.headers_mut().append(header_name, header_value);
+        }
+    }
+
+    let response = client.request(request).await?;
+
+    let status = response.status().as_u16();
     let headers_map = parse_response_headers(&response);
 
-    if !(200..300).contains(&status) {
+    if !(200..300).contains(&(status as isize)) {
         return Ok((String::new(), status, headers_map));
     }
 
-    let mut body = String::new();
-    response.into_reader().read_to_string(&mut body)?;
-    Ok((body, status, headers_map))
-}
-
-fn perform_request(
-    url: &str,
-    headers: &HashMap<String, String>,
-) -> Result<Response, Box<dyn Error>> {
-    let agent = Agent::new();
-    let mut request_builder = agent.get(url);
-
-    // Add headers to the request
-    for (key, value) in headers {
-        request_builder = request_builder.set(key, value);
-    }
+    let body_bytes = hyper::body::to_bytes(response.into_body()).await?;
+    let body = String::from_utf8_lossy(&body_bytes).to_string();
 
-    let response = request_builder.call()?;
-    Ok(response)
+    Ok((body, status, headers_map))
 }
 
 fn parse_response_headers(
-    response: &ureq::Response,
+    response: &hyper::Response<Body>,
 ) -> HashMap<String, String> {
-    let header_names = response.headers_names();
+    let mut headers_map = HashMap::new();
 
-    // Creating a HashMap to store the headers
-    let mut headers_map: HashMap<String, String> = HashMap::new();
-
-    // Iterating through the header names and getting their values
-    for key in header_names {
-        if let Some(value) = response.header(&key) {
-            headers_map.insert(key, value.to_owned());
-        }
+    for (key, value) in response.headers() {
+        headers_map.insert(
+            key.to_string(),
+            value.to_str().unwrap_or_default().to_string(),
+        );
     }
     headers_map
 }
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/localfs/list.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/localfs/list.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,82 @@
 use std::fs;
 use std::path::Path;
 
-use crate::{FileObject, FileObjectFilter};
+use super::bucket::FileSystem;
+use crate::{FileObject, FileObjectFilter, FileObjectVec};
 
-pub fn list_files(
+pub async fn list_files(
+    fs: &dyn FileSystem,
     path: &Path,
     max_keys: Option<u32>,
     recursive: bool,
     filter: &Option<FileObjectFilter>,
-) -> Vec<FileObject> {
-    let mut file_objects = Vec::new();
-    list_files_next(path, max_keys, recursive, filter, &mut file_objects);
-    file_objects
+    file_objects: &mut FileObjectVec,
+) {
+    list_files_next(fs, path, max_keys, recursive, filter, file_objects).await;
+}
+
+async fn list_files_next(
+    fs: &dyn FileSystem,
+    path: &Path,
+    max_keys: Option<u32>,
+    recursive: bool,
+    filter: &Option<FileObjectFilter>,
+    file_objects: &mut FileObjectVec,
+) {
+    let mut directory_stack = vec![path.to_owned()];
+
+    while let Some(current_path) = directory_stack.pop() {
+        let mut temp_file_objects = Vec::new();
+
+        if let Ok(entries) = fs.read_dir(&current_path) {
+            for entry in entries.flatten() {
+                if let Some(max_keys) = max_keys {
+                    if file_objects.len() >= max_keys as usize {
+                        break;
+                    }
+                }
+
+                let metadata = match entry.metadata() {
+                    Ok(md) => md,
+                    Err(_) => continue,
+                };
+
+                if metadata.is_file() {
+                    let file_object = handle_file(&entry, filter);
+                    if let Some(file_object) = file_object {
+                        temp_file_objects.push(file_object);
+                    }
+                } else if metadata.is_dir() {
+                    let dir_name = entry.path().to_string_lossy().to_string();
+
+                    // Only add directory object when no filter is provided
+                    if filter.is_none() {
+                        let dir_object =
+                            FileObject::new(dir_name, 0, None, None);
+                        temp_file_objects.push(dir_object);
+                    }
+
+                    if recursive {
+                        directory_stack.push(entry.path());
+                    }
+                }
+            }
+        }
+        file_objects.extend_async(temp_file_objects).await;
+    }
 }
 
 fn handle_file(
     entry: &fs::DirEntry,
     filter: &Option<FileObjectFilter>,
-    file_objects: &mut Vec<FileObject>,
-) -> u32 {
+) -> Option<FileObject> {
     let metadata = match entry.metadata() {
         Ok(md) => md,
-        Err(_) => return 0,
+        Err(_) => return None,
     };
 
     let file_name = entry.path().to_string_lossy().to_string();
     let file_size = metadata.len();
     let modified = metadata.modified().ok().map(|mtime| {
         mtime
             .duration_since(std::time::UNIX_EPOCH)
@@ -34,80 +85,13 @@
     });
 
     let file_object = FileObject::new(file_name, file_size, modified, None);
 
     // Check if the file_object satisfies the filter conditions
     if let Some(ref filter) = filter {
         if !filter.matches(&file_object) {
-            return 0;
+            return None;
         }
     }
 
-    file_objects.push(file_object);
-    1
-}
-
-fn handle_directory(
-    entry: &fs::DirEntry,
-    max_keys: Option<u32>,
-    recursive: bool,
-    filter: &Option<FileObjectFilter>,
-    file_objects: &mut Vec<FileObject>,
-) -> u32 {
-    let dir_name = entry.path().to_string_lossy().to_string();
-
-    // Only add directory object when no filter is provided
-    if filter.is_none() {
-        let dir_object = FileObject::new(dir_name, 0, None, None);
-        file_objects.push(dir_object);
-    }
-
-    if !recursive {
-        return 1;
-    }
-
-    list_files_next(
-        entry.path().as_path(),
-        max_keys,
-        recursive,
-        filter,
-        file_objects,
-    ) + 1
-}
-
-fn list_files_next(
-    path: &Path,
-    max_keys: Option<u32>,
-    recursive: bool,
-    filter: &Option<FileObjectFilter>,
-    file_objects: &mut Vec<FileObject>,
-) -> u32 {
-    let mut count = 0;
-
-    if let Ok(entries) = fs::read_dir(path) {
-        for entry in entries.flatten() {
-            if let Some(max_keys) = max_keys {
-                if file_objects.len() >= max_keys as usize {
-                    break;
-                }
-            }
-
-            let metadata = match entry.metadata() {
-                Ok(md) => md,
-                Err(_) => continue,
-            };
-
-            if metadata.is_file() {
-                count += handle_file(&entry, filter, file_objects);
-            } else if metadata.is_dir() {
-                count += handle_directory(
-                    &entry,
-                    max_keys,
-                    recursive,
-                    filter,
-                    file_objects,
-                );
-            }
-        }
-    }
-    count
+    Some(file_object)
 }
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/s3/client.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/s3/request_builder.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,100 @@
 use std::collections::HashMap;
 
 use hmac::{Hmac, Mac, NewMac};
-use itertools::Itertools;
 use percent_encoding::{utf8_percent_encode, CONTROLS};
 use sha2::{Digest, Sha256};
 use url::{form_urlencoded, Url};
 
-use super::bucket::S3Credentials;
+use super::client::S3ClientConfig;
 use crate::utils::time::UtcTimeNow;
-use crate::AWS_MAX_LIST_OBJECTS;
+use crate::LakestreamError;
 
-fn sign(key: &[u8], msg: &[u8]) -> Vec<u8> {
-    let mut hmac = Hmac::<Sha256>::new_from_slice(key)
-        .expect("HMAC can take key of any size");
-    hmac.update(msg);
-    let result = hmac.finalize();
-    result.into_bytes().as_slice().to_vec()
+pub struct RequestBuilder {
+    url: String,
 }
 
-pub struct S3Client {
-    resource: String,
-    region: String,
-    credentials: S3Credentials,
-    endpoint_url: String,
-    utc_now: UtcTimeNow,
-    query_string: Option<String>,
-}
+impl RequestBuilder {
+    pub fn new(url: &str) -> Self {
+        let url = url.to_string();
+        Self { url }
+    }
 
-impl S3Client {
-    pub fn new(
-        endpoint_url: String,
-        region: String,
-        credentials: S3Credentials,
-    ) -> S3Client {
-        let resource = "".to_string();
+    pub fn generate_headers(
+        &self,
+        config: &S3ClientConfig,
+        method: &str,
+        resource: Option<&str>,
+        query_string: Option<&str>,
+        payload_hash: Option<&str>,
+    ) -> Result<HashMap<String, String>, LakestreamError> {
         let utc_now = UtcTimeNow::new();
+        let date_stamp = utc_now.date_stamp();
+        let x_amz_date = utc_now.x_amz_date();
 
-        S3Client {
-            resource,
-            region,
-            credentials,
-            endpoint_url,
-            utc_now,
-            query_string: None,
-        }
-    }
+        let credential_scope =
+            format!("{}/{}/s3/aws4_request", date_stamp, config.region());
+        let mut headers = self.initiate_headers(&x_amz_date, payload_hash);
 
-    pub fn url(&self) -> String {
-        format!(
-            "{}/{}?{}",
-            &self.endpoint_url,
-            &self.resource,
-            self.query_string.as_ref().unwrap_or(&"".to_string())
-        )
+        let url = Url::parse(&self.url)?;
+        let host = url.host_str().ok_or("Missing host")?.to_owned();
+        let host = match url.port() {
+            Some(port) => format!("{}:{}", host, port),
+            None => host,
+        };
+
+        headers.insert("host".to_string(), host);
+
+        let canonical_uri = self.get_canonical_uri(&url, resource);
+
+        let canonical_headers = self.get_canonical_headers(&headers);
+
+        let mut signed_headers: Vec<String> =
+            headers.keys().map(|key| key.to_lowercase()).collect();
+
+        signed_headers.sort();
+
+        let signed_headers_str = signed_headers.join(";");
+
+        let canonical_query_string =
+            self.get_canonical_query_string(query_string)?;
+
+        let canonical_request = format!(
+            "{}\n/{}\n{}\n{}\n{}\n{}",
+            method,
+            canonical_uri,
+            canonical_query_string,
+            canonical_headers,
+            signed_headers_str,
+            payload_hash.unwrap_or("UNSIGNED-PAYLOAD")
+        );
+
+        let string_to_sign = format!(
+            "AWS4-HMAC-SHA256\n{}\n{}\n{:x}",
+            x_amz_date,
+            credential_scope,
+            Sha256::digest(canonical_request.as_bytes())
+        );
+        let signing_key = self.generate_signing_key(
+            &date_stamp,
+            config.credentials().secret_key(),
+            config.region(),
+        );
+        let signature = sign(&signing_key, string_to_sign.as_bytes());
+
+        let authorization_header = format!(
+            "AWS4-HMAC-SHA256 Credential={}/{}, SignedHeaders={}, Signature={}",
+            config.credentials().access_key(),
+            credential_scope,
+            signed_headers_str,
+            hex::encode(signature)
+        );
+
+        headers.insert("Authorization".to_string(), authorization_header);
+        Ok(headers)
     }
 
     fn get_canonical_headers(
         &self,
         headers: &HashMap<String, String>,
     ) -> String {
         let mut canonical_headers = String::new();
@@ -75,42 +113,50 @@
                     &format!("{}:{}\n", header_name, header_value.trim());
             }
         }
 
         canonical_headers
     }
 
-    fn generate_signing_key(&self) -> Vec<u8> {
+    fn generate_signing_key(
+        &self,
+        date_stamp: &str,
+        secret_key: &str,
+        region: &str,
+    ) -> Vec<u8> {
         let k_date = sign(
-            format!("AWS4{}", self.credentials.secret_key()).as_bytes(),
-            self.utc_now.date_stamp().as_bytes(),
+            format!("AWS4{}", secret_key).as_bytes(),
+            date_stamp.as_bytes(),
         );
-        let k_region = sign(&k_date, self.region.as_bytes());
+        let k_region = sign(&k_date, region.as_bytes());
         let k_service = sign(&k_region, b"s3");
         sign(&k_service, b"aws4_request")
     }
 
     fn initiate_headers(
         &self,
-        headers: Option<HashMap<String, String>>,
         x_amz_date: &str,
         payload_hash: Option<&str>,
-    ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
-        let mut headers = headers.unwrap_or_default();
+    ) -> HashMap<String, String> {
+        let mut headers = HashMap::new();
         headers.insert("x-amz-date".to_string(), x_amz_date.to_string());
         headers.insert(
             "x-amz-content-sha256".to_string(),
             payload_hash.unwrap_or("UNSIGNED-PAYLOAD").to_string(),
         );
-        Ok(headers)
+        headers
     }
 
-    fn get_canonical_uri(&self, url: &Url, resource: &str) -> String {
+    fn get_canonical_uri(&self, url: &Url, resource: Option<&str>) -> String {
         let canonical_resource = form_urlencoded::byte_serialize(
-            resource.trim_end_matches('/').as_bytes(),
+            resource
+                .unwrap_or_default()
+                .trim_start_matches('/')
+                .trim_end_matches('/')
+                .as_bytes(),
         )
         .collect::<String>();
         let endpoint_path =
             url.path().trim_start_matches('/').trim_end_matches('/');
 
         if endpoint_path.is_empty() {
             canonical_resource
@@ -122,145 +168,48 @@
                 canonical_resource
             )
         }
     }
 
     fn get_canonical_query_string(
         &self,
-    ) -> Result<String, Box<dyn std::error::Error>> {
-        if self.query_string.as_ref().map_or(true, |s| s.is_empty()) {
+        query_string: Option<&str>,
+    ) -> Result<String, LakestreamError> {
+        if query_string.as_ref().map_or(true, |s| s.is_empty()) {
             Ok(String::new())
         } else {
-            let mut parts: Vec<(String, String)> =
-                match self.query_string.as_ref() {
-                    Some(query) => query
-                        .split('&')
-                        .filter_map(|p| {
-                            let mut split = p.splitn(2, '=');
-                            match (split.next(), split.next()) {
-                                (Some(k), Some(v)) => {
-                                    Some((k.to_string(), v.to_string()))
-                                }
-                                _ => None,
+            let mut parts: Vec<(String, String)> = match query_string.as_ref() {
+                Some(query) => query
+                    .split('&')
+                    .filter_map(|p| {
+                        let mut split = p.splitn(2, '=');
+                        match (split.next(), split.next()) {
+                            (Some(k), Some(v)) => {
+                                Some((k.to_string(), v.to_string()))
                             }
-                        })
-                        .collect(),
-                    None => Vec::new(),
-                };
+                            _ => None,
+                        }
+                    })
+                    .collect(),
+                None => Vec::new(),
+            };
             parts.sort();
 
             let encoded_parts: Vec<String> = parts
                 .into_iter()
                 .map(|(k, v)| {
                     format!("{}={}", k, utf8_percent_encode(&v, CONTROLS))
                 })
                 .collect();
 
             Ok(encoded_parts.join("&"))
         }
     }
+}
 
-    pub fn generate_list_buckets_headers(
-        &mut self,
-    ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
-        let method = "GET";
-
-        self.generate_headers(method, None, None)
-    }
-
-    pub fn generate_list_objects_headers(
-        &mut self,
-        prefix: Option<&str>,
-        max_keys: Option<u32>,
-        continuation_token: Option<&str>,
-    ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
-        let method = "GET";
-
-        // Ensure max_keys does not exceed AWS_MAX_LIST_OBJECTS
-        let max_keys = max_keys
-            .map(|keys| std::cmp::min(keys, AWS_MAX_LIST_OBJECTS))
-            .unwrap_or(AWS_MAX_LIST_OBJECTS);
-
-        let mut query_parts = form_urlencoded::Serializer::new(String::new());
-        query_parts.append_pair("list-type", "2");
-        query_parts.append_pair("max-keys", &max_keys.to_string());
-        query_parts.append_pair("delimiter", "/");
-        query_parts.append_pair("encoding-type", "url");
-
-        if let Some(p) = prefix {
-            query_parts.append_pair("prefix", p);
-        }
-        if let Some(token) = continuation_token {
-            query_parts.append_pair("continuation-token", token);
-        }
-
-        self.query_string = Some(query_parts.finish());
-
-        self.generate_headers(method, None, None)
-    }
-
-    fn generate_headers(
-        &mut self,
-        method: &str,
-        headers: Option<HashMap<String, String>>,
-        payload_hash: Option<&str>,
-    ) -> Result<HashMap<String, String>, Box<dyn std::error::Error>> {
-        let date_stamp = self.utc_now.date_stamp();
-        let x_amz_date = self.utc_now.x_amz_date();
-
-        let credential_scope =
-            format!("{}/{}/s3/aws4_request", date_stamp, self.region);
-        let mut headers =
-            self.initiate_headers(headers, &x_amz_date, payload_hash)?;
-
-        let url = Url::parse(&self.endpoint_url)?;
-        let host = url.host_str().ok_or("Missing host")?.to_owned();
-        let host = match url.port() {
-            Some(port) => host.replace(&format!(":{}", port), ""),
-            None => host,
-        };
-        headers.insert("host".to_string(), host);
-
-        let canonical_uri = self.get_canonical_uri(&url, &self.resource);
-
-        let canonical_headers = self.get_canonical_headers(&headers);
-        let signed_headers = headers
-            .keys()
-            .map(|key| key.to_lowercase())
-            .sorted()
-            .collect::<Vec<String>>()
-            .join(";");
-
-        let canonical_query_string = self.get_canonical_query_string()?;
-
-        let canonical_request = format!(
-            "{}\n/{}\n{}\n{}\n{}\n{}",
-            method,
-            canonical_uri,
-            canonical_query_string,
-            canonical_headers,
-            signed_headers,
-            payload_hash.unwrap_or("UNSIGNED-PAYLOAD")
-        );
-
-        let string_to_sign = format!(
-            "AWS4-HMAC-SHA256\n{}\n{}\n{:x}",
-            x_amz_date,
-            credential_scope,
-            Sha256::digest(canonical_request.as_bytes())
-        );
-
-        let signing_key = self.generate_signing_key();
-        let signature = sign(&signing_key, string_to_sign.as_bytes());
-
-        let authorization_header = format!(
-            "AWS4-HMAC-SHA256 Credential={}/{}, SignedHeaders={}, Signature={}",
-            self.credentials.access_key(),
-            credential_scope,
-            signed_headers,
-            hex::encode(signature)
-        );
-
-        headers.insert("Authorization".to_string(), authorization_header);
-        Ok(headers)
-    }
+fn sign(key: &[u8], msg: &[u8]) -> Vec<u8> {
+    let mut hmac = Hmac::<Sha256>::new_from_slice(key)
+        .expect("HMAC can take key of any size");
+    hmac.update(msg);
+    let result = hmac.finalize();
+    result.into_bytes().as_slice().to_vec()
 }
```

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/utils/formatters.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/utils/formatters.rs`

 * *Files identical despite different names*

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/utils/time.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/utils/time.rs`

 * *Files identical despite different names*

### Comparing `lakestream-0.0.2/local_dependencies/lakestream/src/utils/time_parse_ext.rs` & `lakestream-0.0.3/local_dependencies/lakestream/src/utils/time_parse_ext.rs`

 * *Files identical despite different names*

### Comparing `lakestream-0.0.2/README.rst` & `lakestream-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `lakestream-0.0.2/pyproject.toml` & `lakestream-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "lakestream"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python interface for Lakestream"
 readme = "README.rst"
 requires-python = ">=3.7"
 url = "https://lakestream.dev"
 documentation = "https://lakestream.dev/python_api"
 repository = "https://github.com/serverlessnext/lakestream"
 keywords = ["serverless", "data", "api"]
```

### Comparing `lakestream-0.0.2/Cargo.lock` & `lakestream-0.0.3/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anstream"
-version = "0.3.0"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e579a7752471abc2a8268df8b20005e3eadd975f585398f17efcfd8d4927371"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -83,27 +92,38 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcd8291a340dd8ac70e18878bc4501dd7b4ff970cfa21c207d36ece51ea88fd"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
+name = "async-trait"
+version = "0.1.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
@@ -124,15 +144,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
- "miniz_oxide",
+ "miniz_oxide 0.6.2",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
 version = "0.13.1"
@@ -229,15 +249,15 @@
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae6b4de23c7d39c0631fd3cc952d87951c86c75a13812d7247cb7a896e7b3551"
 dependencies = [
  "byteorder",
  "flate2",
  "lzxd",
- "time",
+ "time 0.3.21",
 ]
 
 [[package]]
 name = "camino"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
@@ -247,15 +267,15 @@
 
 [[package]]
 name = "cargo-options"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68dacdf12b405b432ddcb94aa5edef0766daf8cb781f484e56b518305afd45ba"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.25",
 ]
 
 [[package]]
 name = "cargo-platform"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cbdb825da8a5df079a43676dbe042702f1707b1109f713a01420fbb4cc71fa27"
@@ -267,15 +287,15 @@
 name = "cargo-xwin"
 version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb40f2f01bc8ff52fbb570b4b7f8ec823ba21ce1a64352492868eab29f39b9fc"
 dependencies = [
  "anyhow",
  "cargo-options",
- "clap 3.2.23",
+ "clap 3.2.25",
  "dirs",
  "fs-err",
  "indicatif",
  "path-slash",
  "which",
  "xwin",
 ]
@@ -285,15 +305,15 @@
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed951e06c76e4580db0fec84aad5a0266f876f82c3190e323b4c09875edf5750"
 dependencies = [
  "anyhow",
  "cargo-options",
  "cargo_metadata",
- "clap 3.2.23",
+ "clap 3.2.25",
  "dirs",
  "fs-err",
  "path-slash",
  "rustc_version",
  "semver",
  "serde",
  "serde_json",
@@ -361,57 +381,72 @@
 checksum = "18e9079d1a12a2cc2bffb5db039c43661836ead4082120d5844f02555aca2d46"
 dependencies = [
  "base64 0.13.1",
  "encoding_rs",
 ]
 
 [[package]]
+name = "chrono"
+version = "0.4.24"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+dependencies = [
+ "iana-time-zone",
+ "js-sys",
+ "num-integer",
+ "num-traits",
+ "time 0.1.45",
+ "wasm-bindgen",
+ "winapi",
+]
+
+[[package]]
 name = "chumsky"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23170228b96236b5a7299057ac284a321457700bc8c41a4476052f0f4ba5349d"
 dependencies = [
  "hashbrown",
  "stacker",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags",
- "clap_derive 3.2.18",
+ "clap_derive 3.2.25",
  "clap_lex 0.2.4",
  "indexmap",
  "once_cell",
  "strsim",
  "termcolor",
  "terminal_size",
  "textwrap 0.16.0",
 ]
 
 [[package]]
 name = "clap"
-version = "4.2.4"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
+checksum = "34d21f9bf1b425d2968943631ec91202fe5e837264063503708b83013f8fc938"
 dependencies = [
  "clap_builder",
  "clap_derive 4.2.0",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.4"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
+checksum = "914c8c79fb560f238ef6429439a30023c862f7a28e688c58f7203f12b29970bd"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex 0.4.1",
  "strsim",
  "terminal_size",
@@ -419,32 +454,32 @@
 
 [[package]]
 name = "clap_complete"
 version = "3.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f7a2e0a962c45ce25afce14220bc24f9dade0a1787f185cecf96bfba7847cd8"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.25",
 ]
 
 [[package]]
 name = "clap_complete_fig"
 version = "3.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed37b4c0c1214673eba6ad8ea31666626bf72be98ffb323067d973c48b4964b9"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.25",
  "clap_complete",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.18"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
+checksum = "ae6371b8bdc8b7d3959e9cf7b22d4435ef3e79e138688421ec654acf8c81b008"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
@@ -483,14 +518,24 @@
 checksum = "adfbb116d9e2c4be7011360d0c0bee565712c11e969c9609b25b619366dc379d"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "codespan-reporting"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
+dependencies = [
+ "termcolor",
+ "unicode-width",
+]
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "combine"
@@ -518,14 +563,30 @@
  "lazy_static",
  "libc",
  "unicode-width",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
+name = "core-foundation"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
+name = "core-foundation-sys"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+
+[[package]]
 name = "cpufeatures"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
@@ -599,14 +660,58 @@
 checksum = "b1d1a86f49236c215f271d40892d5fc950490551400b02ef360692c29815c714"
 dependencies = [
  "generic-array",
  "subtle",
 ]
 
 [[package]]
+name = "cxx"
+version = "1.0.94"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
+dependencies = [
+ "cc",
+ "cxxbridge-flags",
+ "cxxbridge-macro",
+ "link-cplusplus",
+]
+
+[[package]]
+name = "cxx-build"
+version = "1.0.94"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
+dependencies = [
+ "cc",
+ "codespan-reporting",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "scratch",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "cxxbridge-flags"
+version = "1.0.94"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
+
+[[package]]
+name = "cxxbridge-macro"
+version = "1.0.94"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
 name = "data-encoding"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
 
 [[package]]
 name = "dialoguer"
@@ -687,15 +792,28 @@
 [[package]]
 name = "env_logger"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44533bbbb3bb3c1fa17d9f2e4e38bbbaf8396ba82193c4cb1b6445d711445d36"
 dependencies = [
  "atty",
- "humantime",
+ "humantime 1.3.0",
+ "log",
+ "regex",
+ "termcolor",
+]
+
+[[package]]
+name = "env_logger"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a12e6657c4c97ebab115a42dcee77225f7f482cdd841cf7088c657a42e9e00e7"
+dependencies = [
+ "atty",
+ "humantime 2.1.0",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
@@ -746,29 +864,44 @@
  "libc",
  "redox_syscall 0.2.16",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
- "miniz_oxide",
+ "miniz_oxide 0.7.1",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "foreign-types"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
+dependencies = [
+ "foreign-types-shared",
+]
+
+[[package]]
+name = "foreign-types-shared"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
@@ -776,14 +909,75 @@
 [[package]]
 name = "fs-err"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0845fa252299212f0389d64ba26f34fa32cfe41588355f21ed507c59a0f64541"
 
 [[package]]
+name = "futures"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
+name = "futures-channel"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+]
+
+[[package]]
+name = "futures-core"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
+
+[[package]]
+name = "futures-io"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
+
+[[package]]
+name = "futures-sink"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+
+[[package]]
+name = "futures-task"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
+
+[[package]]
+name = "futures-util"
+version = "0.3.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+ "futures-task",
+ "pin-project-lite",
+ "pin-utils",
+]
+
+[[package]]
 name = "generic-array"
 version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
@@ -793,15 +987,15 @@
 name = "getrandom"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
@@ -844,14 +1038,33 @@
 dependencies = [
  "log",
  "plain",
  "scroll",
 ]
 
 [[package]]
+name = "h2"
+version = "0.3.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash",
 ]
@@ -899,14 +1112,48 @@
 checksum = "2a2a2320eb7ec0ebe8da8f744d7812d9fc4cb4d09344ac01898dbcb6a20ae69b"
 dependencies = [
  "crypto-mac",
  "digest 0.9.0",
 ]
 
 [[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+
+[[package]]
 name = "human-panic"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c16465f6227e18e5a64eba488245d7b2974d4db0c4404ca5a69b550defa18d0a"
 dependencies = [
  "anstream",
  "anstyle",
@@ -924,14 +1171,81 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
 dependencies = [
  "quick-error",
 ]
 
 [[package]]
+name = "humantime"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
+
+[[package]]
+name = "hyper"
+version = "0.14.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "hyper-tls"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+dependencies = [
+ "bytes",
+ "hyper",
+ "native-tls",
+ "tokio",
+ "tokio-native-tls",
+]
+
+[[package]]
+name = "iana-time-zone"
+version = "0.1.56"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+dependencies = [
+ "cxx",
+ "cxx-build",
+]
+
+[[package]]
 name = "idna"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -968,15 +1282,15 @@
 name = "indicatif"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cef509aa9bc73864d6756f0d34d35504af3cf0844373afe9b8669a5b8005a729"
 dependencies = [
  "console",
  "number_prefix",
- "portable-atomic",
+ "portable-atomic 0.3.20",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1036,38 +1350,61 @@
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lakestream"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
- "clap 4.2.4",
+ "async-trait",
+ "futures",
  "hex",
  "hmac",
- "itertools",
+ "hyper",
+ "hyper-tls",
+ "js-sys",
+ "log",
+ "native-tls",
+ "openssl-sys",
  "percent-encoding",
  "regex",
  "serde",
  "serde-xml-rs",
- "serde_json",
  "sha2 0.9.9",
- "time",
- "ureq",
+ "time 0.3.21",
+ "tokio-native-tls",
+ "toml_edit 0.2.1",
  "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
+name = "lakestream-cli"
+version = "0.0.3"
+dependencies = [
+ "clap 4.2.7",
+ "env_logger 0.9.3",
+ "futures",
+ "lakestream",
+ "log",
+ "tokio",
 ]
 
 [[package]]
 name = "lakestream_py"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "lakestream",
+ "lakestream-cli",
  "maturin",
  "pyo3",
+ "tokio",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
@@ -1081,23 +1418,38 @@
  "fs-err",
  "glob",
  "goblin 0.5.4",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.143"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
+
+[[package]]
+name = "link-cplusplus"
+version = "1.0.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "linked-hash-map"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.4"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
+checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1150,15 +1502,15 @@
  "base64 0.13.1",
  "bytesize",
  "cargo-xwin",
  "cargo-zigbuild",
  "cargo_metadata",
  "cbindgen",
  "cc",
- "clap 3.2.23",
+ "clap 3.2.25",
  "clap_complete",
  "clap_complete_fig",
  "configparser",
  "console",
  "dialoguer",
  "dirs",
  "dunce",
@@ -1247,14 +1599,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
+name = "mio"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+dependencies = [
+ "libc",
+ "log",
+ "wasi 0.11.0+wasi-snapshot-preview1",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
 name = "msi"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eaa7bfcd0ffc3b4dc4a555e5ada4d302b4b6b5ce8d6bc07a6ea703ea63aff149"
 dependencies = [
  "byteorder",
  "cfb",
@@ -1272,24 +1645,61 @@
  "mime",
  "mime_guess",
  "rand",
  "tempfile",
 ]
 
 [[package]]
+name = "native-tls"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
+dependencies = [
+ "lazy_static",
+ "libc",
+ "log",
+ "openssl",
+ "openssl-probe",
+ "openssl-sys",
+ "schannel",
+ "security-framework",
+ "security-framework-sys",
+ "tempfile",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
@@ -1319,14 +1729,68 @@
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
+name = "openssl"
+version = "0.10.52"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
+dependencies = [
+ "bitflags",
+ "cfg-if",
+ "foreign-types",
+ "libc",
+ "once_cell",
+ "openssl-macros",
+ "openssl-sys",
+]
+
+[[package]]
+name = "openssl-macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "openssl-probe"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
+
+[[package]]
+name = "openssl-src"
+version = "111.25.3+1.1.1t"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "openssl-sys"
+version = "0.9.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
+dependencies = [
+ "cc",
+ "libc",
+ "openssl-src",
+ "pkg-config",
+ "vcpkg",
+]
+
+[[package]]
 name = "os_info"
 version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "006e42d5b888366f1880eda20371fedde764ed2213dc8496f49622fa0c99cd5e"
 dependencies = [
  "log",
  "serde",
@@ -1377,18 +1841,24 @@
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
+name = "pin-utils"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
+
+[[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plain"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4596b6d070b27117e987119b4dac604f3c58cfb0b191112e24771b2faeac1a6"
 
@@ -1400,31 +1870,40 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "portable-atomic"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26f6a7b87c2e435a3241addceeeff740ff8b7e76b74c13bf9acb17fa454ea00b"
+checksum = "e30165d31df606f5726b090ec7592c308a0eaf61721ff64c9a3018e344a8753e"
+dependencies = [
+ "portable-atomic 1.3.1",
+]
+
+[[package]]
+name = "portable-atomic"
+version = "1.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bbda379e6e462c97ea6afe9f6233619b202bbc4968d7caa6917788d2070a044"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "pretty_env_logger"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "926d36b9553851b8b0005f1275891b392ee4d2d833852c417ed025477350fb9d"
 dependencies = [
- "env_logger",
+ "env_logger 0.7.1",
  "log",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1564,17 +2043,17 @@
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "quoted_printable"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a24039f627d8285853cc90dcddf8c1ebfaa91f834566948872b225b9a28ed1b6"
+checksum = "5a3866219251662ec3b26fc217e3e05bf9c4f84325234dfb96bf0bf840889e49"
 
 [[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
@@ -1739,17 +2218,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.14"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1779,20 +2258,35 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "schannel"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+dependencies = [
+ "windows-sys 0.42.0",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "scratch"
+version = "1.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
+
+[[package]]
 name = "scroll"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04c565b551bafbef4157586fa379538366e4385d42082f255bfd96e4fe8519da"
 dependencies = [
  "scroll_derive",
 ]
@@ -1815,27 +2309,50 @@
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
+name = "security-framework"
+version = "2.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+dependencies = [
+ "bitflags",
+ "core-foundation",
+ "core-foundation-sys",
+ "libc",
+ "security-framework-sys",
+]
+
+[[package]]
+name = "security-framework-sys"
+version = "2.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
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
 name = "serde-xml-rs"
 version = "0.6.0"
@@ -1846,17 +2363,17 @@
  "serde",
  "thiserror",
  "xml-rs",
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
@@ -1921,26 +2438,45 @@
 [[package]]
 name = "shlex"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
 
 [[package]]
+name = "slab"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "smawk"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f67ad224767faa3c7d8b6d91985b78e70a1324408abcb1cfcc2be4c06bc06043"
 
 [[package]]
+name = "socket2"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "socks"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0c3dbbd9ae980613c6dd8e28a9407b50509d3803b57624d5dfe8315218cd58b"
 dependencies = [
  "byteorder",
  "libc",
@@ -2015,17 +2551,17 @@
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
@@ -2103,34 +2639,45 @@
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
+dependencies = [
+ "libc",
+ "wasi 0.10.0+wasi-snapshot-preview1",
+ "winapi",
+]
+
+[[package]]
+name = "time"
+version = "0.3.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -2143,14 +2690,66 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
+name = "tokio"
+version = "1.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
+dependencies = [
+ "autocfg",
+ "bytes",
+ "libc",
+ "mio",
+ "num_cpus",
+ "pin-project-lite",
+ "socket2",
+ "tokio-macros",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "tokio-macros"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "tokio-native-tls"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
+dependencies = [
+ "native-tls",
+ "tokio",
+]
+
+[[package]]
+name = "tokio-util"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
@@ -2174,14 +2773,25 @@
 checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dbbdcf4f749dd33b1f1ea19b547bf789d87442ec40767d6015e5e2d39158d69a"
+dependencies = [
+ "chrono",
+ "combine",
+ "linked-hash-map",
+]
+
+[[package]]
+name = "toml_edit"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5376256e44f2443f8896ac012507c19a012df0fe8758b55246ae51a2279db51f"
 dependencies = [
  "combine",
  "indexmap",
  "itertools",
@@ -2198,34 +2808,40 @@
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
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
@@ -2259,14 +2875,20 @@
  "thread_local",
  "tracing",
  "tracing-core",
  "tracing-serde",
 ]
 
 [[package]]
+name = "try-lock"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+
+[[package]]
 name = "twox-hash"
 version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if",
  "rand",
@@ -2369,28 +2991,34 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.1"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
+checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
+name = "vcpkg"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "versions"
@@ -2409,14 +3037,30 @@
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
+name = "want"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+dependencies = [
+ "log",
+ "try-lock",
+]
+
+[[package]]
+name = "wasi"
+version = "0.10.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -2440,14 +3084,26 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
@@ -2540,14 +3196,23 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -2688,17 +3353,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
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
 
 [[package]]
 name = "xattr"
 version = "0.2.3"
@@ -2706,29 +3371,29 @@
 checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "xml-rs"
-version = "0.8.4"
+version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2d7d3948613f75c98fd9328cfdcc45acc4d360655289d0a7d4ec931392200a3"
+checksum = "699d0104bcdd7e7af6d093d6c6e2d0c479b8a129ee0d1023b31d2e0c71bfdda2"
 
 [[package]]
 name = "xwin"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f5f72397389fd26dd36b01f23e19c0608db8e764f7bb65fdc5b1e7e2aa02550"
 dependencies = [
  "anyhow",
  "bytes",
  "cab",
  "camino",
- "clap 4.2.4",
+ "clap 4.2.7",
  "cli-table",
  "flate2",
  "indicatif",
  "msi",
  "parking_lot",
  "rayon",
  "regex",
@@ -2742,18 +3407,18 @@
  "ureq",
  "versions",
  "zip",
 ]
 
 [[package]]
 name = "zip"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0445d0fbc924bb93539b4316c11afb121ea39296f99a3c4c9edad09e3658cdef"
+checksum = "7e92305c174683d78035cbf1b70e18db6329cc0f1b9cae0a52ca90bf5bfe7125"
 dependencies = [
  "byteorder",
  "bzip2",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
- "time",
+ "time 0.3.21",
 ]
```

### Comparing `lakestream-0.0.2/PKG-INFO` & `lakestream-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakestream
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

