# Comparing `tmp/pywry-0.5.1.tar.gz` & `tmp/pywry-0.5.2.tar.gz`

## Comparing `pywry-0.5.1.tar` & `pywry-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 pywry-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 pywry-0.5.1/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2678 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/websocket.rs
--rw-r--r--   0     1001      123    21600 2023-05-04 04:52:53.000000 pywry-0.5.1/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    61106 2023-05-04 04:52:53.000000 pywry-0.5.1/Cargo.lock
--rw-r--r--   0     1001      123      985 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/py.typed
--rw-r--r--   0     1001      123      370 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123    11147 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/core.py
--rw-r--r--   0     1001      123      180 2023-05-04 04:52:53.000000 pywry-0.5.1/python/pywry/__init__.py
--rw-r--r--   0     1001      123      792 2023-05-04 04:52:53.000000 pywry-0.5.1/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-05-04 04:52:53.000000 pywry-0.5.1/src/constants.rs
--rw-r--r--   0     1001      123     1301 2023-05-04 04:52:53.000000 pywry-0.5.1/src/lib.rs
--rw-r--r--   0     1001      123      334 2023-05-04 04:52:53.000000 pywry-0.5.1/src/ports.rs
--rw-r--r--   0     1001      123     2896 2023-05-04 04:52:53.000000 pywry-0.5.1/src/structs.rs
--rw-r--r--   0     1001      123     2507 2023-05-04 04:52:53.000000 pywry-0.5.1/src/websocket.rs
--rw-r--r--   0     1001      123    21600 2023-05-04 04:52:53.000000 pywry-0.5.1/src/window.rs
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 pywry-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.2/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     2678 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1223 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123     1085 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     4737 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123    22038 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    60354 2023-05-07 21:47:45.000000 pywry-0.5.2/Cargo.lock
+-rw-r--r--   0     1001      123      985 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/py.typed
+-rw-r--r--   0     1001      123      154 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123    12959 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/core.py
+-rw-r--r--   0     1001      123      180 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/__init__.py
+-rw-r--r--   0     1001      123      733 2023-05-07 21:47:45.000000 pywry-0.5.2/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-05-07 21:47:45.000000 pywry-0.5.2/src/constants.rs
+-rw-r--r--   0     1001      123     1223 2023-05-07 21:47:45.000000 pywry-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      123     1085 2023-05-07 21:47:45.000000 pywry-0.5.2/src/pipe.rs
+-rw-r--r--   0     1001      123     4737 2023-05-07 21:47:45.000000 pywry-0.5.2/src/structs.rs
+-rw-r--r--   0     1001      123    22038 2023-05-07 21:47:45.000000 pywry-0.5.2/src/window.rs
+-rw-r--r--   0        0        0     3280 1970-01-01 00:00:00.000000 pywry-0.5.2/PKG-INFO
```

### Comparing `pywry-0.5.1/rust_src/pywry/Cargo.toml` & `pywry-0.5.2/rust_src/pywry/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.1"
+version = "0.5.2"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -15,15 +15,13 @@
 [dependencies]
 pyo3 = { version = "0.18.0", features = [
     "extension-module",
     "generate-import-lib",
 ] }
 wry = { version = "^0.28", features = ["devtools"] }
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
-tokio-tungstenite = "^0.18"
-tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread"] }
-futures-util = { version = "^0.3.25" }
+tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread", "full"] }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
 urlencoding = "^2.1.2"
 open = "^4.0"
```

### Comparing `pywry-0.5.1/rust_src/pywry/LICENSE` & `pywry-0.5.2/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.1/rust_src/pywry/README.md` & `pywry-0.5.2/rust_src/pywry/README.md`

 * *Files identical despite different names*

### Comparing `pywry-0.5.1/rust_src/pywry/src/constants.rs` & `pywry-0.5.2/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.1/rust_src/pywry/src/lib.rs` & `pywry-0.5.2/rust_src/pywry/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 #![warn(clippy::all, clippy::pedantic, clippy::nursery)]
 #![allow(clippy::missing_errors_doc, clippy::must_use_candidate)]
 
-use ports::get_available_port;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use std::sync::mpsc;
 use window::start_wry;
 
 pub mod constants;
-pub mod ports;
+pub mod pipe;
 pub mod structs;
-pub mod websocket;
 pub mod window;
 
 #[pyclass]
 struct WindowManager {
-    port: u16,
+    #[pyo3(get, set)]
+    debug: bool,
 }
 
 #[pymethods]
 impl WindowManager {
     #[new]
     fn new() -> Self {
-        let target_port = get_available_port().map_or(0, |port| port);
-        Self { port: target_port }
+        Self { debug: false }
     }
-
-    fn start(&self, debug: bool, port: Option<u16>) -> PyResult<()> {
-        let port = port.unwrap_or(self.port);
-
+    fn start(&self, debug: bool) -> PyResult<()> {
         let (sender, receiver) = mpsc::channel();
-        match start_wry(port, sender, receiver, debug) {
+        let debug_printer = structs::DebugPrinter::new(debug);
+        match start_wry(sender, receiver, debug_printer) {
             Err(error) => {
                 let error_str = format!("Error starting wry server: {}", error);
                 Err(PyValueError::new_err(error_str))
             }
             Ok(_) => Ok(()),
         }
     }
-
-    const fn get_port(&self) -> u16 {
-        self.port
-    }
 }
 
-/// A Python module implemented in Rust.
+/// # PyWry Web Viewer
+/// Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library.
 #[pymodule]
 fn pywry(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_class::<WindowManager>()?;
     Ok(())
 }
```

### Comparing `pywry-0.5.1/rust_src/pywry/src/window.rs` & `pywry-0.5.2/rust_src/pywry/src/window.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 use crate::{
     constants::{BLOBINIT_SCRIPT, DEV_TOOLS_HTML},
-    structs::Showable,
-    websocket::run_server,
+    pipe::run_listener,
+    structs::{DebugPrinter, Showable, UserEvent},
 };
 use image::ImageFormat;
 use mime_guess;
 use std::{
     collections::HashMap,
     fs::{canonicalize, read},
     path::PathBuf,
     sync::mpsc::{Receiver, Sender},
 };
 
 #[cfg(not(target_os = "macos"))]
 use std::fs::{copy, create_dir_all, remove_file};
-
-use tokio::{runtime::Runtime, task};
 use urlencoding::decode as urldecode;
 use wry::{
     application::{
         dpi::LogicalSize,
         event::{Event, WindowEvent},
         event_loop::{ControlFlow, EventLoop, EventLoopProxy, EventLoopWindowTarget},
         window::{Icon, Theme, WindowBuilder, WindowId},
     },
     http::{header::CONTENT_TYPE, Response},
     webview::{WebView, WebViewBuilder},
 };
 
-enum UserEvent {
-    #[cfg(not(target_os = "macos"))]
-    DownloadStarted(String, String),
-    #[cfg(not(target_os = "macos"))]
-    DownloadComplete(Option<PathBuf>, bool, String, String, WindowId),
-    #[cfg(not(target_os = "macos"))]
-    BlobReceived(String, WindowId),
-    BlobChunk(Option<String>),
-    CloseWindow(WindowId),
-    DevTools(WindowId),
-    NewWindowCreated(WindowId),
-    OpenFile(Option<PathBuf>),
-    #[cfg(not(target_os = "windows"))]
-    NewWindow(String, Option<Icon>),
-}
-
+/// Gets the icon from the path
+/// # Arguments
+/// * `icon` - The path to the icon
+/// # Returns
+/// * `Option<Icon>` - The icon or None
 fn get_icon(icon: &str) -> Option<Icon> {
     let icon_object = match read(icon) {
         Err(_) => None,
         Ok(bytes) => {
             let imagebuffer = match image::load_from_memory_with_format(&bytes, ImageFormat::Png) {
                 Err(_) => None,
                 Ok(loaded) => {
@@ -62,39 +49,47 @@
             };
             imagebuffer
         }
     };
     icon_object
 }
 
+/// Creates a new window and returns the window id and webview
+/// # Arguments
+/// * `to_show` - The Showable struct that contains the information to show
+/// * `event_loop` - The event loop to create the window on
+/// * `proxy` - The event loop proxy to send events to
+/// * `debug` - The DebugPrinter struct to print debug messages
+/// # Returns
+/// * `Result<(WindowId, WebView), String>` - The window id and webview or an error message
 fn create_new_window(
     mut to_show: Showable,
     event_loop: &&EventLoopWindowTarget<UserEvent>,
     proxy: &EventLoopProxy<UserEvent>,
-    debug: bool,
+    debug: DebugPrinter,
 ) -> Result<(WindowId, WebView), String> {
     if to_show.html_path.is_empty() && to_show.html_str.is_empty() {
         to_show.html_str = String::from(
             "<h1 style='color:red'>No html content to show, please provide a html_path or a html_str key</h1>",
         );
     }
     let window_icon = to_show.icon.clone();
 
-    let content = if to_show.html_path.is_empty() {
-        to_show.html_str.as_bytes().to_vec()
-    } else {
-        to_show.html_path.as_bytes().to_vec()
+    let content = match to_show.html_path.is_empty() {
+        true => to_show.html_str.as_bytes().to_vec(),
+        false => to_show.html_path.as_bytes().to_vec(),
     };
 
-    let content = if debug {
-        let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
-        dev_tools_html.extend(content);
-        dev_tools_html
-    } else {
-        content
+    let content = match debug.active {
+        true => {
+            let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
+            dev_tools_html.extend(content);
+            dev_tools_html
+        }
+        false => content,
     };
 
     let mut pre_window = WindowBuilder::new()
         .with_title(to_show.title)
         .with_window_icon(get_icon(&window_icon))
         .with_min_inner_size(LogicalSize::new(800, 450))
         .with_theme(Some(Theme::Dark));
@@ -109,49 +104,56 @@
     let window = match pre_window.build(event_loop) {
         Err(error) => return Err(error.to_string()),
         Ok(item) => item,
     };
 
     let minimized = !to_show.export_image.is_empty();
     if minimized {
-        window.set_visible(to_show.export_image.is_empty());
+        window.set_visible(false);
         window.set_maximized(false);
     } else {
         window.set_always_on_top(true);
     }
 
     let window_id = window.id();
+    let background_color = match to_show.theme {
+        Theme::Light => (255, 255, 255, 255),
+        Theme::Dark => (0, 0, 0, 255),
+        _ => (255, 255, 255, 255),
+    };
 
     let webview = match WebViewBuilder::new(window) {
         Err(error2) => return Err(error2.to_string()),
         Ok(item) => {
             let protocol = item
-                .with_background_color((0, 0, 0, 255))
+                .with_background_color(background_color)
                 .with_hotkeys_zoom(true)
                 .with_custom_protocol("wry".into(), move |request| {
                     let path = request.uri().path();
                     let clean_path = &path[1..];
                     let content = content.clone();
                     let mut mime = mime_guess::from_path("index.html");
 
                     let content = if path == "/" {
                         content.into()
                     } else {
-                        let file_path = if clean_path.starts_with("file://") {
-                            let decoded = urldecode(&clean_path).expect("UTF-8").to_string();
-                            let path = PathBuf::from(&decoded);
-                            if ":" == &decoded[9..10] {
-                                path.strip_prefix("file://").unwrap().to_path_buf()
-                            } else {
-                                let path = PathBuf::from(&decoded[6..]);
-                                path.to_path_buf()
+                        let file_path = match clean_path.starts_with("file://") {
+                            true => {
+                                let decoded = urldecode(&clean_path).expect("UTF-8").to_string();
+                                let path = PathBuf::from(&decoded);
+                                if ":" == &decoded[9..10] {
+                                    path.strip_prefix("file://").unwrap().to_path_buf()
+                                } else {
+                                    let path = PathBuf::from(&decoded[6..]);
+                                    path.to_path_buf()
+                                }
                             }
-                        } else {
-                            PathBuf::from(clean_path)
+                            false => PathBuf::from(clean_path),
                         };
+
                         let file_path = file_path.to_str().unwrap();
 
                         mime = mime_guess::from_path(file_path);
                         match read(canonicalize(file_path).unwrap_or_default()) {
                             Err(_) => content.into(),
                             Ok(bytes) => bytes.into(),
                         }
@@ -168,42 +170,32 @@
                         .body(content)
                         .map_err(Into::into)
                 });
             let export_image = to_show.export_image.clone();
             let _is_export = !export_image.is_empty();
             let download_path = to_show.download_path.clone();
 
-            let init_view = if !to_show.data.is_none() || !to_show.figure.is_none() {
-                let variable_name = if !to_show.data.is_none() {
-                    "json_data"
-                } else {
-                    "plotly_figure"
-                };
-
-                let variable_value = if !to_show.data.is_none() {
-                    serde_json::to_string(&to_show.data.unwrap()).unwrap_or_default()
-                } else {
-                    serde_json::to_string(&to_show.figure.unwrap()).unwrap_or_default()
-                };
-
-                let initialization_script = if !export_image.is_empty() {
-                    format!(
-                        "window.{} = {}; window.save_image = true; window.export_image = '{}';",
-                        variable_name, variable_value, export_image
-                    )
-                } else {
-                    format!(
-                        "window.{} = {}; window.download_path = {:?};",
-                        variable_name, variable_value, download_path
-                    )
-                };
-
-                protocol.with_initialization_script(&initialization_script)
-            } else {
-                protocol
+            let init_view = match !to_show.data.is_none() {
+                true => {
+                    let variable_value =
+                        serde_json::to_string(&to_show.data.unwrap()).unwrap_or_default();
+                    let initialization_script = match !export_image.is_empty() {
+                        true => format!(
+                            "window.json_data = {}; window.save_image = true; window.export_image = {:?};",
+                            variable_value, export_image
+                        ),
+                        false => format!(
+                            "window.json_data = {}; window.download_path = {:?};",
+                            variable_value, download_path
+                        ),
+                    };
+
+                    protocol.with_initialization_script(&initialization_script)
+                }
+                false => protocol,
             };
 
             // we add a download handler, if export_image is set it takes precedence over download_path
             let init_view = init_view
                 .with_download_started_handler({
                     let _proxy = proxy.clone();
                     move |_uri: String, default_path| {
@@ -304,15 +296,18 @@
                     }
                     #[cfg(target_os = "windows")]
                     {
                         move |_uri: String| true
                     }
                 });
 
-            match init_view.with_devtools(debug).with_url("wry://localhost") {
+            match init_view
+                .with_devtools(debug.active)
+                .with_url("wry://localhost")
+            {
                 Err(error3) => return Err(error3.to_string()),
                 Ok(subitem) => match subitem.build() {
                     Err(error4) => return Err(error4.to_string()),
                     Ok(sub2item) => {
                         if !minimized {
                             let proxy = proxy.clone();
                             let _ = proxy.send_event(UserEvent::NewWindowCreated(window_id));
@@ -323,178 +318,177 @@
             }
         }
     };
 
     Ok((window_id, webview))
 }
 
+/// Starts Main Runtime Loop and creates a new window when a message is received from Python
+/// # Arguments
+/// * `sender` - The sender to send messages from Python to Wry Event Loop
+/// * `receiver` - The receiver Wry uses to receive messages from Python
+/// * `debug` - The DebugPrinter struct to print debug messages
+///
+/// # Returns
+/// * `Result<(), String>` - An error message or nothing
 pub fn start_wry(
-    port: u16,
     sender: Sender<String>,
     receiver: Receiver<String>,
-    debug: bool,
+    debug: DebugPrinter,
 ) -> Result<(), String> {
     let event_loop: EventLoop<UserEvent> = EventLoop::with_user_event();
     let proxy = event_loop.create_proxy();
     let mut webviews = HashMap::new();
-    let rt = match Runtime::new() {
-        Err(_) => return Err("Could not start a runtime".to_string()),
-        Ok(item) => item,
-    };
 
-    rt.block_on(async { task::spawn(run_server(port, sender, debug)) });
+    std::thread::spawn(move || {
+        tokio::runtime::Builder::new_current_thread()
+            .enable_all()
+            .build()
+            .unwrap()
+            .block_on(async move { run_listener(sender.clone()).await.unwrap() })
+    });
 
     event_loop.run(move |event, event_loop, control_flow| {
         *control_flow = ControlFlow::Poll;
 
         let response = receiver.try_recv().unwrap_or_default();
 
         if !response.is_empty() {
-            if debug {
-                println!("Received response");
-            }
+            debug.print("Received response");
+
             let chart = Showable::new(&response).unwrap_or_default();
             match create_new_window(chart, &event_loop, &proxy, debug) {
                 Err(error) => println!("Window Creation Error: {}", error),
 
                 Ok(new_window) => {
                     webviews.insert(new_window.0, new_window.1);
                 }
             };
         }
 
         match event {
             // UserEvent::NewWindowCreated
             Event::UserEvent(UserEvent::NewWindowCreated(window_id)) => {
-                if debug {
-                    println!("New Window Created");
-                }
+                debug.print("New Window Created");
                 if let Some(webview) = webviews.get_mut(&window_id) {
                     webview.window().set_always_on_top(false);
                 }
             }
             // UserEvent::DownloadStarted
             #[cfg(not(target_os = "macos"))]
             Event::UserEvent(UserEvent::DownloadStarted(uri, path)) => {
-                if debug {
-                    if uri.len() < 200 {
-                        println!("\nDownload Started: {}", uri);
-                    }
-                    println!("\nPath: {}", path);
+                if uri.len() < 200 {
+                    debug.print(&format!("\nDownload Started: {}", uri));
                 }
+                debug.print(&format!("\nPath: {}", path));
             }
             // UserEvent::DownloadComplete
             #[cfg(not(target_os = "macos"))]
             Event::UserEvent(UserEvent::DownloadComplete(
                 filepath,
                 success,
                 download_path,
                 export_image,
                 window_id,
             )) => {
                 let is_export = !export_image.is_empty();
-                if debug {
-                    println!("\nDownload Complete: {}", success);
-                }
+                debug.print(&format!("\nDownload Complete: {}", success));
+
                 if let Some(filepath) = filepath {
                     let decoded = urldecode(&filepath.to_str().unwrap())
                         .expect("UTF-8")
                         .to_string();
-                    let file_path = if decoded.starts_with("file://") {
-                        if ":" == &decoded[9..10] {
-                            let path = PathBuf::from(decoded);
-                            path.strip_prefix("file://").unwrap().to_path_buf()
-                        } else {
-                            let path = PathBuf::from(&decoded[6..]);
-                            path.to_path_buf()
+
+                    let file_path = match decoded.starts_with("file://") {
+                        true => {
+                            if ":" == &decoded[9..10] {
+                                let path = PathBuf::from(&decoded);
+                                path.strip_prefix("file://").unwrap().to_path_buf()
+                            } else {
+                                let path = PathBuf::from(&decoded[6..]);
+                                path.to_path_buf()
+                            }
                         }
-                    } else {
-                        PathBuf::from(decoded)
+                        false => PathBuf::from(decoded),
                     };
-                    let new_path = if !download_path.is_empty() {
-                        if !export_image.is_empty() {
-                            let path = PathBuf::from(&export_image);
-                            path.to_path_buf()
-                        } else {
-                            let mut path = PathBuf::from(&download_path);
-                            path.push(file_path.file_name().unwrap());
-                            path.to_path_buf()
-                        }
-                    } else {
-                        file_path.to_path_buf()
+
+                    let new_path = match !download_path.is_empty() {
+                        true => match !export_image.is_empty() {
+                            true => {
+                                let path = PathBuf::from(&export_image);
+                                path.to_path_buf()
+                            }
+                            false => {
+                                let mut path = PathBuf::from(&download_path);
+                                path.push(file_path.file_name().unwrap());
+                                path.to_path_buf()
+                            }
+                        },
+                        false => file_path.to_path_buf(),
                     };
 
-                    if debug {
-                        println!("\nOriginal Path: {}", file_path.to_str().unwrap());
-                        println!("New Path: {}", new_path.to_str().unwrap());
-                    }
+                    debug.print(&format!(
+                        "\nOriginal Path: {:?}",
+                        file_path.to_str().unwrap()
+                    ));
+                    debug.print(&format!("New Path: {}", new_path.to_str().unwrap()));
+
                     let dir = new_path.parent().unwrap();
-                    if !dir.exists() {
-                        if debug {
-                            println!("\nCreating directory: {}", dir.display());
-                        }
-                        if let Err(error) = create_dir_all(dir) {
-                            println!("Error creating directory: {}", error);
+                    match !dir.exists() {
+                        true => {
+                            debug.print(&format!("\nCreating directory: {}", dir.display()));
+                            if let Err(error) = create_dir_all(dir) {
+                                println!("Error creating directory: {}", error);
+                            }
                         }
+                        false => {}
                     }
-                    if let Err(error) = copy(&file_path, &new_path) {
-                        println!("\nError copying file: {}", error);
-                    } else {
-                        if is_export {
-                            let _ = proxy.send_event(UserEvent::CloseWindow(window_id));
-                        }
-                        if let Err(error) = remove_file(&file_path) {
-                            println!("Error deleting file: {}", error);
+
+                    match copy(&file_path, &new_path) {
+                        Err(error) => println!("\nError copying file: {}", error),
+                        Ok(_) => {
+                            if is_export {
+                                let _ = proxy.send_event(UserEvent::CloseWindow(window_id));
+                            }
+                            if let Err(error) = remove_file(&file_path) {
+                                println!("Error deleting file: {}", error);
+                            }
                         }
                     }
                 }
             }
             // UserEvent::CloseWindow
             Event::UserEvent(UserEvent::CloseWindow(window_id)) => {
-                if debug {
-                    println!("Close Window");
-                }
+                debug.print("Closing Window");
                 if let Some(_) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Closing Webview");
-                    }
+                    debug.print("Closing Webview");
                     webviews.remove(&window_id);
                 }
             }
             // UserEvent::BlobChunk
             Event::UserEvent(UserEvent::BlobChunk(_)) => {
-                if debug {
-                    println!("Blob Chunk");
-                }
+                debug.print("Blob Chunk");
             }
             // WindowEvent::CloseRequested
             Event::WindowEvent {
                 event: WindowEvent::CloseRequested,
                 window_id,
                 ..
             } => {
-                if debug {
-                    println!("Close Requested");
-                }
+                debug.print("Close Requested");
                 if let Some(_) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Closing Webview");
-                    }
+                    debug.print("Closing Webview");
                     webviews.remove(&window_id);
                 }
             }
             // UserEvent::DevTools
             Event::UserEvent(UserEvent::DevTools(window_id)) => {
-                if debug {
-                    println!("DevTools");
-                }
+                debug.print("DevTools");
                 if let Some(webview) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Opening DevTools");
-                    }
+                    debug.print("Opening DevTools");
                     let _ = webview.open_devtools();
                 }
             }
             // UserEvent::OpenFile
             Event::UserEvent(UserEvent::OpenFile(filepath)) => {
                 if filepath.is_some() {
                     let decoded = urldecode(&filepath.unwrap().to_str().unwrap())
@@ -505,50 +499,47 @@
                         println!("Error opening file: {}", error);
                     }
                 }
             }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
-                if debug {
-                    println!("\nNew Window Requested: {}", uri);
-                }
-                if uri.starts_with("http://") || uri.starts_with("https://") {
-                    let pre_window = WindowBuilder::new()
-                        .with_title(uri.to_string())
-                        .with_window_icon(window_icon)
-                        .with_inner_size(LogicalSize::new(1300, 900))
-                        .with_resizable(true)
-                        .with_theme(Some(Theme::Dark));
-
-                    let window = match pre_window.build(event_loop) {
-                        Err(error) => {
-                            println!("Window Creation Error: {}", error);
-                            return;
-                        }
-                        Ok(item) => item,
-                    };
+                debug.print(&format!("\nNew Window Requested: {}", uri));
+                match uri.starts_with("http://") || uri.starts_with("https://") {
+                    true => {
+                        let pre_window = WindowBuilder::new()
+                            .with_title(uri.to_string())
+                            .with_window_icon(window_icon)
+                            .with_inner_size(LogicalSize::new(1300, 900))
+                            .with_resizable(true)
+                            .with_theme(Some(Theme::Dark));
+
+                        let window = match pre_window.build(event_loop) {
+                            Err(error) => {
+                                println!("Window Creation Error: {}", error);
+                                return;
+                            }
+                            Ok(item) => item,
+                        };
+
+                        let window_id = window.id();
 
-                    let window_id = window.id();
+                        let webview = WebViewBuilder::new(window)
+                            .unwrap()
+                            .with_url(&uri)
+                            .unwrap()
+                            .build()
+                            .unwrap();
 
-                    let webview = WebViewBuilder::new(window)
-                        .unwrap()
-                        .with_url(&uri)
-                        .unwrap()
-                        .build()
-                        .unwrap();
-
-                    webviews.insert(window_id, webview);
-
-                    if debug {
-                        println!("New Window Created");
-                    }
-                } else {
-                    if debug {
-                        println!("Invalid URI tried to open in new window: {}", uri);
+                        webviews.insert(window_id, webview);
+
+                        debug.print("New Window Created");
+                    }
+                    false => {
+                        debug.print(&format!("Invalid URI tried to open in new window: {}", uri));
                     }
                 }
             }
             _ => {}
         }
     });
 }
```

### Comparing `pywry-0.5.1/Cargo.lock` & `pywry-0.5.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -468,34 +468,27 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "futures-sink"
-version = "0.3.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
-
-[[package]]
 name = "futures-task"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
 
 [[package]]
 name = "futures-util"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
 dependencies = [
  "futures-core",
  "futures-macro",
- "futures-sink",
  "futures-task",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
@@ -814,20 +807,14 @@
 dependencies = [
  "bytes",
  "fnv",
  "itoa 1.0.6",
 ]
 
 [[package]]
-name = "httparse"
-version = "1.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
-
-[[package]]
 name = "idna"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -1494,25 +1481,23 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
- "futures-util",
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
  "tokio",
- "tokio-tungstenite",
  "urlencoding",
  "wry",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
@@ -1729,33 +1714,31 @@
 checksum = "d98238b800e0d1576d8b6e3de32827c2d74bee68bb97748dcf5071fb53965432"
 dependencies = [
  "nodrop",
  "stable_deref_trait",
 ]
 
 [[package]]
-name = "sha1"
-version = "0.10.5"
+name = "sha2"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
-name = "sha2"
-version = "0.10.6"
+name = "signal-hook-registry"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
- "cfg-if",
- "cpufeatures",
- "digest",
+ "libc",
 ]
 
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
@@ -1878,17 +1861,17 @@
  "pkg-config",
  "toml",
  "version-compare",
 ]
 
 [[package]]
 name = "tao"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "389820c5cd5279ffdde7729baa9cf4db20e9936e11b1e171a20fb74babe3a6d3"
+checksum = "746ae5d0ca57ae275a792f109f6e992e0b41a443abdf3f5c6eff179ef5b3443a"
 dependencies = [
  "bitflags",
  "cairo-rs",
  "cc",
  "cocoa",
  "core-foundation",
  "core-graphics",
@@ -2004,29 +1987,31 @@
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "memchr",
  "mio",
  "num_cpus",
+ "parking_lot",
  "pin-project-lite",
+ "signal-hook-registry",
  "socket2",
+ "tokio-macros",
  "windows-sys",
 ]
 
 [[package]]
-name = "tokio-tungstenite"
-version = "0.18.0"
+name = "tokio-macros"
+version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54319c93411147bced34cb5609a80e0a8e44c5999c93903a81cd866630ec0bfd"
+checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
 dependencies = [
- "futures-util",
- "log",
- "tokio",
- "tungstenite",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
@@ -2048,33 +2033,14 @@
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
-name = "tungstenite"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30ee6ab729cd4cf0fd55218530c4522ed30b7b6081752839b68fcec8d0960788"
-dependencies = [
- "base64",
- "byteorder",
- "bytes",
- "http",
- "httparse",
- "log",
- "rand 0.8.5",
- "sha1",
- "thiserror",
- "url",
- "utf-8",
-]
-
-[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicase"
@@ -2425,17 +2391,17 @@
 checksum = "23d020b441f92996c80d94ae9166e8501e59c7bb56121189dc9eab3bd8216966"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wry"
-version = "0.28.0"
+version = "0.28.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "073b88c1cb1be36d71b6e717237870541297ffb77d175c52a9abc1448d72e6cf"
+checksum = "7d15f9f827d537cefe6d047be3930f5d89b238dfb85e08ba6a319153217635aa"
 dependencies = [
  "base64",
  "block",
  "cocoa",
  "core-graphics",
  "crossbeam-channel",
  "dunce",
```

### Comparing `pywry-0.5.1/python/pywry/backend.py` & `pywry-0.5.2/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.1/Cargo.toml` & `pywry-0.5.2/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.1"
+version = "0.5.2"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
@@ -15,15 +15,13 @@
 [dependencies]
 pyo3 = { version = "0.18.0", features = [
     "extension-module",
     "generate-import-lib",
 ] }
 wry = { version = "^0.28", features = ["devtools"] }
 image = { version = "^0.24.5", default-features = false, features = ["png"] }
-tokio-tungstenite = "^0.18"
-tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread"] }
-futures-util = { version = "^0.3.25" }
+tokio = { version = "^1.23.0", features = ["rt", "rt-multi-thread", "full"] }
 serde = { version = "^1.0", features = ["derive"] }
 serde_json = "^1.0"
 mime_guess = "^2.0"
 urlencoding = "^2.1.2"
 open = "^4.0"
```

### Comparing `pywry-0.5.1/src/constants.rs` & `pywry-0.5.2/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.1/src/lib.rs` & `pywry-0.5.2/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 #![warn(clippy::all, clippy::pedantic, clippy::nursery)]
 #![allow(clippy::missing_errors_doc, clippy::must_use_candidate)]
 
-use ports::get_available_port;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use std::sync::mpsc;
 use window::start_wry;
 
 pub mod constants;
-pub mod ports;
+pub mod pipe;
 pub mod structs;
-pub mod websocket;
 pub mod window;
 
 #[pyclass]
 struct WindowManager {
-    port: u16,
+    #[pyo3(get, set)]
+    debug: bool,
 }
 
 #[pymethods]
 impl WindowManager {
     #[new]
     fn new() -> Self {
-        let target_port = get_available_port().map_or(0, |port| port);
-        Self { port: target_port }
+        Self { debug: false }
     }
-
-    fn start(&self, debug: bool, port: Option<u16>) -> PyResult<()> {
-        let port = port.unwrap_or(self.port);
-
+    fn start(&self, debug: bool) -> PyResult<()> {
         let (sender, receiver) = mpsc::channel();
-        match start_wry(port, sender, receiver, debug) {
+        let debug_printer = structs::DebugPrinter::new(debug);
+        match start_wry(sender, receiver, debug_printer) {
             Err(error) => {
                 let error_str = format!("Error starting wry server: {}", error);
                 Err(PyValueError::new_err(error_str))
             }
             Ok(_) => Ok(()),
         }
     }
-
-    const fn get_port(&self) -> u16 {
-        self.port
-    }
 }
 
-/// A Python module implemented in Rust.
+/// # PyWry Web Viewer
+/// Easily create HTML webviewers in python utilizing the [wry](https://github.com/tauri-apps/wry) library.
 #[pymodule]
 fn pywry(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_class::<WindowManager>()?;
     Ok(())
 }
```

### Comparing `pywry-0.5.1/src/window.rs` & `pywry-0.5.2/src/window.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 use crate::{
     constants::{BLOBINIT_SCRIPT, DEV_TOOLS_HTML},
-    structs::Showable,
-    websocket::run_server,
+    pipe::run_listener,
+    structs::{DebugPrinter, Showable, UserEvent},
 };
 use image::ImageFormat;
 use mime_guess;
 use std::{
     collections::HashMap,
     fs::{canonicalize, read},
     path::PathBuf,
     sync::mpsc::{Receiver, Sender},
 };
 
 #[cfg(not(target_os = "macos"))]
 use std::fs::{copy, create_dir_all, remove_file};
-
-use tokio::{runtime::Runtime, task};
 use urlencoding::decode as urldecode;
 use wry::{
     application::{
         dpi::LogicalSize,
         event::{Event, WindowEvent},
         event_loop::{ControlFlow, EventLoop, EventLoopProxy, EventLoopWindowTarget},
         window::{Icon, Theme, WindowBuilder, WindowId},
     },
     http::{header::CONTENT_TYPE, Response},
     webview::{WebView, WebViewBuilder},
 };
 
-enum UserEvent {
-    #[cfg(not(target_os = "macos"))]
-    DownloadStarted(String, String),
-    #[cfg(not(target_os = "macos"))]
-    DownloadComplete(Option<PathBuf>, bool, String, String, WindowId),
-    #[cfg(not(target_os = "macos"))]
-    BlobReceived(String, WindowId),
-    BlobChunk(Option<String>),
-    CloseWindow(WindowId),
-    DevTools(WindowId),
-    NewWindowCreated(WindowId),
-    OpenFile(Option<PathBuf>),
-    #[cfg(not(target_os = "windows"))]
-    NewWindow(String, Option<Icon>),
-}
-
+/// Gets the icon from the path
+/// # Arguments
+/// * `icon` - The path to the icon
+/// # Returns
+/// * `Option<Icon>` - The icon or None
 fn get_icon(icon: &str) -> Option<Icon> {
     let icon_object = match read(icon) {
         Err(_) => None,
         Ok(bytes) => {
             let imagebuffer = match image::load_from_memory_with_format(&bytes, ImageFormat::Png) {
                 Err(_) => None,
                 Ok(loaded) => {
@@ -62,39 +49,47 @@
             };
             imagebuffer
         }
     };
     icon_object
 }
 
+/// Creates a new window and returns the window id and webview
+/// # Arguments
+/// * `to_show` - The Showable struct that contains the information to show
+/// * `event_loop` - The event loop to create the window on
+/// * `proxy` - The event loop proxy to send events to
+/// * `debug` - The DebugPrinter struct to print debug messages
+/// # Returns
+/// * `Result<(WindowId, WebView), String>` - The window id and webview or an error message
 fn create_new_window(
     mut to_show: Showable,
     event_loop: &&EventLoopWindowTarget<UserEvent>,
     proxy: &EventLoopProxy<UserEvent>,
-    debug: bool,
+    debug: DebugPrinter,
 ) -> Result<(WindowId, WebView), String> {
     if to_show.html_path.is_empty() && to_show.html_str.is_empty() {
         to_show.html_str = String::from(
             "<h1 style='color:red'>No html content to show, please provide a html_path or a html_str key</h1>",
         );
     }
     let window_icon = to_show.icon.clone();
 
-    let content = if to_show.html_path.is_empty() {
-        to_show.html_str.as_bytes().to_vec()
-    } else {
-        to_show.html_path.as_bytes().to_vec()
+    let content = match to_show.html_path.is_empty() {
+        true => to_show.html_str.as_bytes().to_vec(),
+        false => to_show.html_path.as_bytes().to_vec(),
     };
 
-    let content = if debug {
-        let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
-        dev_tools_html.extend(content);
-        dev_tools_html
-    } else {
-        content
+    let content = match debug.active {
+        true => {
+            let mut dev_tools_html = DEV_TOOLS_HTML.as_bytes().to_vec();
+            dev_tools_html.extend(content);
+            dev_tools_html
+        }
+        false => content,
     };
 
     let mut pre_window = WindowBuilder::new()
         .with_title(to_show.title)
         .with_window_icon(get_icon(&window_icon))
         .with_min_inner_size(LogicalSize::new(800, 450))
         .with_theme(Some(Theme::Dark));
@@ -109,49 +104,56 @@
     let window = match pre_window.build(event_loop) {
         Err(error) => return Err(error.to_string()),
         Ok(item) => item,
     };
 
     let minimized = !to_show.export_image.is_empty();
     if minimized {
-        window.set_visible(to_show.export_image.is_empty());
+        window.set_visible(false);
         window.set_maximized(false);
     } else {
         window.set_always_on_top(true);
     }
 
     let window_id = window.id();
+    let background_color = match to_show.theme {
+        Theme::Light => (255, 255, 255, 255),
+        Theme::Dark => (0, 0, 0, 255),
+        _ => (255, 255, 255, 255),
+    };
 
     let webview = match WebViewBuilder::new(window) {
         Err(error2) => return Err(error2.to_string()),
         Ok(item) => {
             let protocol = item
-                .with_background_color((0, 0, 0, 255))
+                .with_background_color(background_color)
                 .with_hotkeys_zoom(true)
                 .with_custom_protocol("wry".into(), move |request| {
                     let path = request.uri().path();
                     let clean_path = &path[1..];
                     let content = content.clone();
                     let mut mime = mime_guess::from_path("index.html");
 
                     let content = if path == "/" {
                         content.into()
                     } else {
-                        let file_path = if clean_path.starts_with("file://") {
-                            let decoded = urldecode(&clean_path).expect("UTF-8").to_string();
-                            let path = PathBuf::from(&decoded);
-                            if ":" == &decoded[9..10] {
-                                path.strip_prefix("file://").unwrap().to_path_buf()
-                            } else {
-                                let path = PathBuf::from(&decoded[6..]);
-                                path.to_path_buf()
+                        let file_path = match clean_path.starts_with("file://") {
+                            true => {
+                                let decoded = urldecode(&clean_path).expect("UTF-8").to_string();
+                                let path = PathBuf::from(&decoded);
+                                if ":" == &decoded[9..10] {
+                                    path.strip_prefix("file://").unwrap().to_path_buf()
+                                } else {
+                                    let path = PathBuf::from(&decoded[6..]);
+                                    path.to_path_buf()
+                                }
                             }
-                        } else {
-                            PathBuf::from(clean_path)
+                            false => PathBuf::from(clean_path),
                         };
+
                         let file_path = file_path.to_str().unwrap();
 
                         mime = mime_guess::from_path(file_path);
                         match read(canonicalize(file_path).unwrap_or_default()) {
                             Err(_) => content.into(),
                             Ok(bytes) => bytes.into(),
                         }
@@ -168,42 +170,32 @@
                         .body(content)
                         .map_err(Into::into)
                 });
             let export_image = to_show.export_image.clone();
             let _is_export = !export_image.is_empty();
             let download_path = to_show.download_path.clone();
 
-            let init_view = if !to_show.data.is_none() || !to_show.figure.is_none() {
-                let variable_name = if !to_show.data.is_none() {
-                    "json_data"
-                } else {
-                    "plotly_figure"
-                };
-
-                let variable_value = if !to_show.data.is_none() {
-                    serde_json::to_string(&to_show.data.unwrap()).unwrap_or_default()
-                } else {
-                    serde_json::to_string(&to_show.figure.unwrap()).unwrap_or_default()
-                };
-
-                let initialization_script = if !export_image.is_empty() {
-                    format!(
-                        "window.{} = {}; window.save_image = true; window.export_image = '{}';",
-                        variable_name, variable_value, export_image
-                    )
-                } else {
-                    format!(
-                        "window.{} = {}; window.download_path = {:?};",
-                        variable_name, variable_value, download_path
-                    )
-                };
-
-                protocol.with_initialization_script(&initialization_script)
-            } else {
-                protocol
+            let init_view = match !to_show.data.is_none() {
+                true => {
+                    let variable_value =
+                        serde_json::to_string(&to_show.data.unwrap()).unwrap_or_default();
+                    let initialization_script = match !export_image.is_empty() {
+                        true => format!(
+                            "window.json_data = {}; window.save_image = true; window.export_image = {:?};",
+                            variable_value, export_image
+                        ),
+                        false => format!(
+                            "window.json_data = {}; window.download_path = {:?};",
+                            variable_value, download_path
+                        ),
+                    };
+
+                    protocol.with_initialization_script(&initialization_script)
+                }
+                false => protocol,
             };
 
             // we add a download handler, if export_image is set it takes precedence over download_path
             let init_view = init_view
                 .with_download_started_handler({
                     let _proxy = proxy.clone();
                     move |_uri: String, default_path| {
@@ -304,15 +296,18 @@
                     }
                     #[cfg(target_os = "windows")]
                     {
                         move |_uri: String| true
                     }
                 });
 
-            match init_view.with_devtools(debug).with_url("wry://localhost") {
+            match init_view
+                .with_devtools(debug.active)
+                .with_url("wry://localhost")
+            {
                 Err(error3) => return Err(error3.to_string()),
                 Ok(subitem) => match subitem.build() {
                     Err(error4) => return Err(error4.to_string()),
                     Ok(sub2item) => {
                         if !minimized {
                             let proxy = proxy.clone();
                             let _ = proxy.send_event(UserEvent::NewWindowCreated(window_id));
@@ -323,178 +318,177 @@
             }
         }
     };
 
     Ok((window_id, webview))
 }
 
+/// Starts Main Runtime Loop and creates a new window when a message is received from Python
+/// # Arguments
+/// * `sender` - The sender to send messages from Python to Wry Event Loop
+/// * `receiver` - The receiver Wry uses to receive messages from Python
+/// * `debug` - The DebugPrinter struct to print debug messages
+///
+/// # Returns
+/// * `Result<(), String>` - An error message or nothing
 pub fn start_wry(
-    port: u16,
     sender: Sender<String>,
     receiver: Receiver<String>,
-    debug: bool,
+    debug: DebugPrinter,
 ) -> Result<(), String> {
     let event_loop: EventLoop<UserEvent> = EventLoop::with_user_event();
     let proxy = event_loop.create_proxy();
     let mut webviews = HashMap::new();
-    let rt = match Runtime::new() {
-        Err(_) => return Err("Could not start a runtime".to_string()),
-        Ok(item) => item,
-    };
 
-    rt.block_on(async { task::spawn(run_server(port, sender, debug)) });
+    std::thread::spawn(move || {
+        tokio::runtime::Builder::new_current_thread()
+            .enable_all()
+            .build()
+            .unwrap()
+            .block_on(async move { run_listener(sender.clone()).await.unwrap() })
+    });
 
     event_loop.run(move |event, event_loop, control_flow| {
         *control_flow = ControlFlow::Poll;
 
         let response = receiver.try_recv().unwrap_or_default();
 
         if !response.is_empty() {
-            if debug {
-                println!("Received response");
-            }
+            debug.print("Received response");
+
             let chart = Showable::new(&response).unwrap_or_default();
             match create_new_window(chart, &event_loop, &proxy, debug) {
                 Err(error) => println!("Window Creation Error: {}", error),
 
                 Ok(new_window) => {
                     webviews.insert(new_window.0, new_window.1);
                 }
             };
         }
 
         match event {
             // UserEvent::NewWindowCreated
             Event::UserEvent(UserEvent::NewWindowCreated(window_id)) => {
-                if debug {
-                    println!("New Window Created");
-                }
+                debug.print("New Window Created");
                 if let Some(webview) = webviews.get_mut(&window_id) {
                     webview.window().set_always_on_top(false);
                 }
             }
             // UserEvent::DownloadStarted
             #[cfg(not(target_os = "macos"))]
             Event::UserEvent(UserEvent::DownloadStarted(uri, path)) => {
-                if debug {
-                    if uri.len() < 200 {
-                        println!("\nDownload Started: {}", uri);
-                    }
-                    println!("\nPath: {}", path);
+                if uri.len() < 200 {
+                    debug.print(&format!("\nDownload Started: {}", uri));
                 }
+                debug.print(&format!("\nPath: {}", path));
             }
             // UserEvent::DownloadComplete
             #[cfg(not(target_os = "macos"))]
             Event::UserEvent(UserEvent::DownloadComplete(
                 filepath,
                 success,
                 download_path,
                 export_image,
                 window_id,
             )) => {
                 let is_export = !export_image.is_empty();
-                if debug {
-                    println!("\nDownload Complete: {}", success);
-                }
+                debug.print(&format!("\nDownload Complete: {}", success));
+
                 if let Some(filepath) = filepath {
                     let decoded = urldecode(&filepath.to_str().unwrap())
                         .expect("UTF-8")
                         .to_string();
-                    let file_path = if decoded.starts_with("file://") {
-                        if ":" == &decoded[9..10] {
-                            let path = PathBuf::from(decoded);
-                            path.strip_prefix("file://").unwrap().to_path_buf()
-                        } else {
-                            let path = PathBuf::from(&decoded[6..]);
-                            path.to_path_buf()
+
+                    let file_path = match decoded.starts_with("file://") {
+                        true => {
+                            if ":" == &decoded[9..10] {
+                                let path = PathBuf::from(&decoded);
+                                path.strip_prefix("file://").unwrap().to_path_buf()
+                            } else {
+                                let path = PathBuf::from(&decoded[6..]);
+                                path.to_path_buf()
+                            }
                         }
-                    } else {
-                        PathBuf::from(decoded)
+                        false => PathBuf::from(decoded),
                     };
-                    let new_path = if !download_path.is_empty() {
-                        if !export_image.is_empty() {
-                            let path = PathBuf::from(&export_image);
-                            path.to_path_buf()
-                        } else {
-                            let mut path = PathBuf::from(&download_path);
-                            path.push(file_path.file_name().unwrap());
-                            path.to_path_buf()
-                        }
-                    } else {
-                        file_path.to_path_buf()
+
+                    let new_path = match !download_path.is_empty() {
+                        true => match !export_image.is_empty() {
+                            true => {
+                                let path = PathBuf::from(&export_image);
+                                path.to_path_buf()
+                            }
+                            false => {
+                                let mut path = PathBuf::from(&download_path);
+                                path.push(file_path.file_name().unwrap());
+                                path.to_path_buf()
+                            }
+                        },
+                        false => file_path.to_path_buf(),
                     };
 
-                    if debug {
-                        println!("\nOriginal Path: {}", file_path.to_str().unwrap());
-                        println!("New Path: {}", new_path.to_str().unwrap());
-                    }
+                    debug.print(&format!(
+                        "\nOriginal Path: {:?}",
+                        file_path.to_str().unwrap()
+                    ));
+                    debug.print(&format!("New Path: {}", new_path.to_str().unwrap()));
+
                     let dir = new_path.parent().unwrap();
-                    if !dir.exists() {
-                        if debug {
-                            println!("\nCreating directory: {}", dir.display());
-                        }
-                        if let Err(error) = create_dir_all(dir) {
-                            println!("Error creating directory: {}", error);
+                    match !dir.exists() {
+                        true => {
+                            debug.print(&format!("\nCreating directory: {}", dir.display()));
+                            if let Err(error) = create_dir_all(dir) {
+                                println!("Error creating directory: {}", error);
+                            }
                         }
+                        false => {}
                     }
-                    if let Err(error) = copy(&file_path, &new_path) {
-                        println!("\nError copying file: {}", error);
-                    } else {
-                        if is_export {
-                            let _ = proxy.send_event(UserEvent::CloseWindow(window_id));
-                        }
-                        if let Err(error) = remove_file(&file_path) {
-                            println!("Error deleting file: {}", error);
+
+                    match copy(&file_path, &new_path) {
+                        Err(error) => println!("\nError copying file: {}", error),
+                        Ok(_) => {
+                            if is_export {
+                                let _ = proxy.send_event(UserEvent::CloseWindow(window_id));
+                            }
+                            if let Err(error) = remove_file(&file_path) {
+                                println!("Error deleting file: {}", error);
+                            }
                         }
                     }
                 }
             }
             // UserEvent::CloseWindow
             Event::UserEvent(UserEvent::CloseWindow(window_id)) => {
-                if debug {
-                    println!("Close Window");
-                }
+                debug.print("Closing Window");
                 if let Some(_) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Closing Webview");
-                    }
+                    debug.print("Closing Webview");
                     webviews.remove(&window_id);
                 }
             }
             // UserEvent::BlobChunk
             Event::UserEvent(UserEvent::BlobChunk(_)) => {
-                if debug {
-                    println!("Blob Chunk");
-                }
+                debug.print("Blob Chunk");
             }
             // WindowEvent::CloseRequested
             Event::WindowEvent {
                 event: WindowEvent::CloseRequested,
                 window_id,
                 ..
             } => {
-                if debug {
-                    println!("Close Requested");
-                }
+                debug.print("Close Requested");
                 if let Some(_) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Closing Webview");
-                    }
+                    debug.print("Closing Webview");
                     webviews.remove(&window_id);
                 }
             }
             // UserEvent::DevTools
             Event::UserEvent(UserEvent::DevTools(window_id)) => {
-                if debug {
-                    println!("DevTools");
-                }
+                debug.print("DevTools");
                 if let Some(webview) = webviews.get(&window_id) {
-                    if debug {
-                        println!("Opening DevTools");
-                    }
+                    debug.print("Opening DevTools");
                     let _ = webview.open_devtools();
                 }
             }
             // UserEvent::OpenFile
             Event::UserEvent(UserEvent::OpenFile(filepath)) => {
                 if filepath.is_some() {
                     let decoded = urldecode(&filepath.unwrap().to_str().unwrap())
@@ -505,50 +499,47 @@
                         println!("Error opening file: {}", error);
                     }
                 }
             }
             // WindowEvent::NewWindow
             #[cfg(not(target_os = "windows"))]
             Event::UserEvent(UserEvent::NewWindow(uri, window_icon)) => {
-                if debug {
-                    println!("\nNew Window Requested: {}", uri);
-                }
-                if uri.starts_with("http://") || uri.starts_with("https://") {
-                    let pre_window = WindowBuilder::new()
-                        .with_title(uri.to_string())
-                        .with_window_icon(window_icon)
-                        .with_inner_size(LogicalSize::new(1300, 900))
-                        .with_resizable(true)
-                        .with_theme(Some(Theme::Dark));
-
-                    let window = match pre_window.build(event_loop) {
-                        Err(error) => {
-                            println!("Window Creation Error: {}", error);
-                            return;
-                        }
-                        Ok(item) => item,
-                    };
+                debug.print(&format!("\nNew Window Requested: {}", uri));
+                match uri.starts_with("http://") || uri.starts_with("https://") {
+                    true => {
+                        let pre_window = WindowBuilder::new()
+                            .with_title(uri.to_string())
+                            .with_window_icon(window_icon)
+                            .with_inner_size(LogicalSize::new(1300, 900))
+                            .with_resizable(true)
+                            .with_theme(Some(Theme::Dark));
+
+                        let window = match pre_window.build(event_loop) {
+                            Err(error) => {
+                                println!("Window Creation Error: {}", error);
+                                return;
+                            }
+                            Ok(item) => item,
+                        };
+
+                        let window_id = window.id();
 
-                    let window_id = window.id();
+                        let webview = WebViewBuilder::new(window)
+                            .unwrap()
+                            .with_url(&uri)
+                            .unwrap()
+                            .build()
+                            .unwrap();
 
-                    let webview = WebViewBuilder::new(window)
-                        .unwrap()
-                        .with_url(&uri)
-                        .unwrap()
-                        .build()
-                        .unwrap();
-
-                    webviews.insert(window_id, webview);
-
-                    if debug {
-                        println!("New Window Created");
-                    }
-                } else {
-                    if debug {
-                        println!("Invalid URI tried to open in new window: {}", uri);
+                        webviews.insert(window_id, webview);
+
+                        debug.print("New Window Created");
+                    }
+                    false => {
+                        debug.print(&format!("Invalid URI tried to open in new window: {}", uri));
                     }
                 }
             }
             _ => {}
         }
     });
 }
```

### Comparing `pywry-0.5.1/PKG-INFO` & `pywry-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.1
+Version: 0.5.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: websockets
-Requires-Dist: psutil>=5.8.0,<5.9.4
 Requires-Dist: setproctitle
 Requires-Dist: auditwheel; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

