# Comparing `tmp/llm_rs-0.1.0.tar.gz` & `tmp/llm_rs-0.1.1.tar.gz`

## Comparing `llm_rs-0.1.0.tar` & `llm_rs-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 llm_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2810 2023-05-03 15:18:04.000000 llm_rs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3455 2023-05-03 15:18:04.000000 llm_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-03 15:18:04.000000 llm_rs-0.1.0/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-03 15:18:04.000000 llm_rs-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1913 2023-05-03 15:18:04.000000 llm_rs-0.1.0/README.md
--rw-r--r--   0     1001      123      221 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/__init__.py
--rw-r--r--   0     1001      123     1201 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/config.pyi
--rw-r--r--   0     1001      123        0 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123     1250 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/py.typed
--rw-r--r--   0     1001      123      697 2023-05-03 15:18:04.000000 llm_rs-0.1.0/llm_rs/results.pyi
--rw-r--r--   0     1001      123      709 2023-05-03 15:18:04.000000 llm_rs-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     4127 2023-05-03 15:18:04.000000 llm_rs-0.1.0/src/configs.rs
--rw-r--r--   0     1001      123     1502 2023-05-03 15:18:04.000000 llm_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     6498 2023-05-03 15:18:04.000000 llm_rs-0.1.0/src/model_base.rs
--rw-r--r--   0     1001      123      253 2023-05-03 15:18:04.000000 llm_rs-0.1.0/src/models.rs
--rw-r--r--   0     1001      123     1263 2023-05-03 15:18:04.000000 llm_rs-0.1.0/src/results.rs
--rw-r--r--   0     1001      123    20399 2023-05-03 15:19:10.000000 llm_rs-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 llm_rs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 llm_rs-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2810 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3455 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-08 14:10:49.000000 llm_rs-0.1.1/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-08 14:10:49.000000 llm_rs-0.1.1/LICENSE
+-rw-r--r--   0     1001      123     1913 2023-05-08 14:10:49.000000 llm_rs-0.1.1/README.md
+-rw-r--r--   0     1001      123      221 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/__init__.py
+-rw-r--r--   0     1001      123     1201 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/config.pyi
+-rw-r--r--   0     1001      123        0 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123     1528 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/py.typed
+-rw-r--r--   0     1001      123      697 2023-05-08 14:10:49.000000 llm_rs-0.1.1/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      709 2023-05-08 14:10:49.000000 llm_rs-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     4127 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/configs.rs
+-rw-r--r--   0     1001      123     1502 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     8693 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/model_base.rs
+-rw-r--r--   0     1001      123      253 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/models.rs
+-rw-r--r--   0     1001      123     1263 2023-05-08 14:10:49.000000 llm_rs-0.1.1/src/results.rs
+-rw-r--r--   0     1001      123    20390 2023-05-08 14:11:58.000000 llm_rs-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 llm_rs-0.1.1/PKG-INFO
```

### Comparing `llm_rs-0.1.0/.github/workflows/CI.yml` & `llm_rs-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/.gitignore` & `llm_rs-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/LICENSE` & `llm_rs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/README.md` & `llm_rs-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 model = Llama("path/to/model.bin")
 
 #generate
 print(model.generate("The meaning of life is"))
 ```
 
 The package also supports callbacks to get each token as it is generated.
-The callback-function also supports canceling the generation by returning a `True` value from the pytohn side.
+The callback-function also supports canceling the generation by returning a `True` value from the python side.
 
 ```python 
 from llm_rs import Llama
 import sys
 from typing import Optional
 
 #load the model
```

### Comparing `llm_rs-0.1.0/llm_rs/config.pyi` & `llm_rs-0.1.1/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/llm_rs/models.pyi` & `llm_rs-0.1.1/llm_rs/models.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable
+from typing import Optional, Callable, List
 from abc import ABC, abstractmethod
 
 from .config import GenerationConfig, SessionConfig
 from .results import GenerationResult
 
 #Theoretically this is incorrect as the 'model' doesnt actually exist, but it is a good enough approximation for now. 
 class Model(ABC):
@@ -19,14 +19,26 @@
     
     def  __init__(self,path:str,session_config:SessionConfig=SessionConfig(), verbose:bool=False) -> None: ...
     
     def generate(self,prompt:str,
                  generation_config:Optional[GenerationConfig]=None,
                  callback:Callable[[str],Optional[bool]]=None) -> GenerationResult: ...
     
+    def tokenize(self,text:str) -> List[int]:
+        """
+        Tokenizes a string into a list of tokens.
+        """
+        ...
+    
+    def decode(self,tokens:List[int]) -> str:
+        """
+        Decodes a list of tokens into a string.
+        """
+        ...
+    
 
 class Llama(Model):
     """
     Wrapper around all Llama based models.
     """
     ...
```

### Comparing `llm_rs-0.1.0/llm_rs/results.pyi` & `llm_rs-0.1.1/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/pyproject.toml` & `llm_rs-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/src/configs.rs` & `llm_rs-0.1.1/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/src/lib.rs` & `llm_rs-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/src/model_base.rs` & `llm_rs-0.1.1/src/model_base.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,44 @@
 use pyo3::prelude::*;
 use pyo3::exceptions::PyException;
 use pyo3::types::{PyTuple};
 
-use llm::{InferenceError, TokenUtf8Buffer};
-
+use llm::{InferenceError, TokenUtf8Buffer,};
+use llm_base::{EvaluateOutputRequest};
 
 use rand_chacha::ChaCha8Rng;
 use rand::prelude::*;
 
 use crate::configs;
 use crate::results;
 
+
+pub fn _tokenize(model: & dyn llm::Model,text: &str) -> Result<Vec<i32>,InferenceError>{
+    Ok(model.vocabulary()
+        .tokenize(text,false)?
+        .iter()
+        .map(|(_, token)| *token)
+        .collect())
+}
+
+pub fn _decode(model: & dyn llm::Model,tokens: Vec<i32>) -> Result<String,std::str::Utf8Error>{
+    let vocab = model.vocabulary();
+    let characters:Vec<u8> = tokens
+    .into_iter()
+    .map(|token| vocab.id_to_token[token as usize].to_owned())
+    .flatten()
+    .collect();
+
+    match std::str::from_utf8(&characters){
+        Ok(text) => Ok(text.to_string()),
+        Err(e) => Err(e),
+    }
+}
+
+
 pub fn _generate(
         _py: Python,
         model: & dyn llm::Model,
         session_config: &configs::SessionConfig,
         prompt: String,
         generation_config: Option<&configs::GenerationConfig>,
         callback: Option<PyObject>,)->Result<results::GenerationResult,PyErr>{
@@ -41,44 +65,64 @@
                 let python_function = pytohn_object.as_ref(_py);
                 callback_function = Some(python_function);
                 assert!(python_function.is_callable(), "Callback is not callable!");
             }
     
             let feed_start_at = std::time::SystemTime::now();
             //Feed the prompt
-            session.feed_prompt(model, &generation_params, &prompt, |_| {
-                Ok::<(), InferenceError>(())
-            });
+            
+            
+            let mut output_request_feeding = EvaluateOutputRequest::default();
+            _py.allow_threads(||session.feed_prompt(model, &generation_params, &prompt, &mut output_request_feeding,|_| {
+                Ok::<(),InferenceError>(())
+            }).unwrap());
             let feed_prompt_duration = feed_start_at.elapsed().unwrap();
     
     
             //Start the inference loop
             let mut tokens_processed = 0;
             let mut token_utf8_buf = TokenUtf8Buffer::new();
     
             let mut total_generated_text = String::new();
-            let mut stop_reason = results::StopReason::EndToken;
+            let stop_reason ;
     
             let generation_start_at = std::time::SystemTime::now();
+
+       
+            let mut output_request_generation = EvaluateOutputRequest::default();   
+            let mut _generate_next_tokens= ||-> Result<Option<String>, PyErr>{
+                
+                let token = match session.infer_next_token(model, &generation_params, &mut output_request_generation,&mut rng) {
+                    Ok(token) => token,
+                    Err(InferenceError::EndOfText) => return Ok(None),
+                    Err(e) => return Err(PyException::new_err(e.to_string())),
+                };
+                Ok(token_utf8_buf.push(token))
+
+            };
+
             loop {
                 //Check if we have reached the maximum token count
                 if config_to_use.max_new_tokens.is_some() && tokens_processed >= config_to_use.max_new_tokens.unwrap() {
                     stop_reason=results::StopReason::MaxLength;
                     break;
                 }
     
                 //Infere the next token and break if the END_OF_TEXT token is reached
-                let token = match session.infer_next_token(model, &generation_params, &mut rng) {
-                    Ok(token) => token,
-                    Err(InferenceError::EndOfText) => break,
-                    Err(e) => return Err(PyException::new_err(e.to_string())),
-                };
-    
+                
+                let mut token:Option<String> = None;
+                _py.allow_threads(|| token=_generate_next_tokens().unwrap());
+               
+
+                if token.is_none() {
+                    stop_reason=results::StopReason::EndToken;
+                    break;
+                }
                 //Buffer until a valid utf8 sequence is found
-                if let Some(tokens) = token_utf8_buf.push(token) {
+                if let Some(tokens) = token {
     
                     total_generated_text.push_str(&tokens);
                     //Check if the callback function is set and call it
                     if let Some(function) = callback_function {
                         let args = PyTuple::new(_py, &[tokens]);
                         let result = function.call1(args)?;
                         //Check if the callback function returned true
@@ -90,14 +134,17 @@
                             }
                         }
                     }
                 }
     
                 tokens_processed += 1;
             }
+            
+           
+
             let generation_duration = generation_start_at.elapsed().unwrap();
     
             let result = results::GenerationResult{
                 text:total_generated_text,
                 times: results::GenerationTimes{
                     total:generation_duration.as_millis()+feed_prompt_duration.as_millis(),
                     generation:generation_duration.as_millis(),
@@ -134,19 +181,22 @@
                 let should_log = verbose.unwrap_or(false);
 
                 //Build the correct session parameters
                 let default_config = crate::configs::SessionConfig::default();
                 let config_to_use = session_config.unwrap_or(default_config);
             
                 let path = std::path::Path::new(&path);
-                
+                let model_params =  llm_base::ModelParameters{
+                    n_context_tokens: config_to_use.context_length,
+                    prefer_mmap: config_to_use.prefer_mmap,
+                    ..Default::default()
+                };
                 let llm_model: $llm_model = llm_base::load(
                     &path,
-                    config_to_use.prefer_mmap,
-                    config_to_use.context_length,
+                    model_params,
                     |load_progress| {
                     if should_log{
                         llm_base::load_progress_callback_stdout(load_progress)
                     }
                 }).unwrap();
 
                 
@@ -159,14 +209,28 @@
                 prompt: String,
                 generation_config: Option<&crate::configs::GenerationConfig>,
                 callback: Option<PyObject>,
             ) -> PyResult<crate::results::GenerationResult> {
 
                 return crate::model_base::_generate(_py,self.llm_model.as_ref(),&self.config,prompt, generation_config, callback);
             }
+
+            fn tokenize(&self,text:String)-> PyResult<Vec<i32>>{
+                match crate::model_base::_tokenize(self.llm_model.as_ref(),&text){
+                    Ok(tokens) => Ok(tokens),
+                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string()))
+                }
+            }
+
+            fn decode(&self,tokens:Vec<i32>)-> PyResult<String>{
+                match crate::model_base::_decode(self.llm_model.as_ref(),tokens){
+                    Ok(tokens) => Ok(tokens),
+                    Err(e) => Err(pyo3::exceptions::PyException::new_err(e.to_string()))
+                }
+            }
         }
 
 
         };
 }
```

### Comparing `llm_rs-0.1.0/src/results.rs` & `llm_rs-0.1.1/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.1.0/Cargo.lock` & `llm_rs-0.1.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -132,25 +132,25 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "ggml-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
@@ -204,106 +204,101 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "llm"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
  "llm-llama",
  "llm-neox",
 ]
 
 [[package]]
 name = "llm-base"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
  "serde",
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-bloom"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
- "ggml",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
- "ggml",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
- "ggml",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-llama"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
- "ggml",
  "llm-base",
  "protobuf",
  "rand",
  "rust_tokenizers",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-neox"
-version = "0.1.0"
-source = "git+https://github.com/rustformers/llm.git#9fbe79fbbf9dd1be20c6f035c4fae4fa99527844"
+version = "0.1.0-rc3"
+source = "git+https://github.com/rustformers/llm.git#d4ec956cb17ee035e78d5af8867e016ce502c8bf"
 dependencies = [
  "bytemuck",
- "ggml",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
@@ -594,17 +589,17 @@
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
 name = "serde_bytes"
 version = "0.11.9"
@@ -612,17 +607,17 @@
 checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
 dependencies = [
  "serde",
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
```

### Comparing `llm_rs-0.1.0/PKG-INFO` & `llm_rs-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llm-rs
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Summary: Unofficial python bindings for llm-rs. 🐍❤️🦀
 Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/LLukas22/llm-rs-python
 Project-URL: Bug Tracker, https://github.com/LLukas22/llm-rs-python/issues
+Project-URL: Homepage, https://github.com/LLukas22/llm-rs-python
 
 # llm-rs-python
 Unofficial python bindings for the rust [llm](https://github.com/rustformers/llm) library created with [PyO3](https://github.com/PyO3/pyo3). 🐍❤️🦀
 
 This package allows you to run multiple different Large Language Models (LLMs) like LLama or GPT-NeoX on your CPU.
 
 All supported architectures are listed on the [llm](https://github.com/rustformers/llm) project page.
@@ -39,15 +39,15 @@
 model = Llama("path/to/model.bin")
 
 #generate
 print(model.generate("The meaning of life is"))
 ```
 
 The package also supports callbacks to get each token as it is generated.
-The callback-function also supports canceling the generation by returning a `True` value from the pytohn side.
+The callback-function also supports canceling the generation by returning a `True` value from the python side.
 
 ```python 
 from llm_rs import Llama
 import sys
 from typing import Optional
 
 #load the model
```

