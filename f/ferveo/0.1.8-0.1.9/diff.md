# Comparing `tmp/ferveo-0.1.8.tar.gz` & `tmp/ferveo-0.1.9.tar.gz`

## Comparing `ferveo-0.1.8.tar` & `ferveo-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/subproductdomain/Cargo.toml
--rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/subproductdomain/src/lib.rs
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/Cargo.toml
--rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/BENCHMARK.md
--rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/README.md
--rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
--rw-rw-r--   0     1000     1000    19154 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/tpke.rs
--rw-rw-r--   0     1000     1000     1259 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/api.rs
--rw-rw-r--   0     1000     1000     7780 2023-04-28 12:33:25.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
--rw-rw-r--   0     1000     1000     5498 2023-04-26 08:55:27.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/combine.rs
--rw-rw-r--   0     1000     1000     3429 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/context.rs
--rw-rw-r--   0     1000     1000    11504 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/decryption.rs
--rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
--rw-rw-r--   0     1000     1000     2183 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/key_share.rs
--rw-rw-r--   0     1000     1000    28735 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/lib.rs
--rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/refresh.rs
--rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/ferveo/Cargo.toml
--rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/Cargo.lock
--rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.8/local_dependencies/ferveo/README.md
--rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/bench_main.rs
--rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
--rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/mod.rs
--rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pairing.rs
--rw-rw-r--   0     1000     1000     3478 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
--rw-rw-r--   0     1000     1000     3257 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
--rw-rw-r--   0     1000     1000     2897 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/ferveo/examples/bench_ark_sizes.rs
--rw-rw-r--   0     1000     1000     4336 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/examples/bench_primitives_size.rs
--rw-rw-r--   0     1000     1000    18555 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/api.rs
--rw-rw-r--   0     1000     1000    24426 2023-04-26 12:06:08.000000 ferveo-0.1.8/local_dependencies/ferveo/src/dkg/pv.rs
--rw-rw-r--   0     1000     1000    24978 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/dkg.rs
--rw-rw-r--   0     1000     1000    17470 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/lib.rs
--rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/src/primitives.rs
--rw-rw-r--   0     1000     1000    21326 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/pvss.rs
--rw-rw-r--   0     1000     1000     1976 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/validator.rs
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/ferveo-common/Cargo.toml
--rw-rw-r--   0     1000     1000     6907 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/keypair.rs
--rw-rw-r--   0     1000     1000      120 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/lib.rs
--rw-rw-r--   0     1000     1000     4000 2023-04-26 12:06:08.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/serialization.rs
--rw-rw-r--   0     1000     1000      406 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/utils.rs
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 ferveo-0.1.8/Cargo.toml
--rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.8/.gitignore
--rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.8/LICENSE
--rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.8/MANIFEST.in
--rw-rw-r--   0     1000     1000      226 2023-05-03 13:35:12.000000 ferveo-0.1.8/README.md
--rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.8/build.rs
--rw-rw-r--   0     1000     1000     3007 2023-05-03 13:21:11.000000 ferveo-0.1.8/examples/server_api_precomputed.py
--rw-rw-r--   0     1000     1000     3128 2023-05-03 13:21:11.000000 ferveo-0.1.8/examples/server_api_simple.py
--rw-rw-r--   0     1000     1000      383 2023-04-26 12:06:08.000000 ferveo-0.1.8/ferveo/__init__.py
--rw-rw-r--   0     1000     1000     3691 2023-04-26 12:06:08.000000 ferveo-0.1.8/ferveo/__init__.pyi
--rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.8/ferveo/py.typed
--rw-rw-r--   0     1000     1000      316 2023-04-14 08:59:50.000000 ferveo-0.1.8/pyproject.toml
--rw-rw-r--   0     1000     1000     1444 2023-05-03 13:28:52.000000 ferveo-0.1.8/setup.py
--rw-rw-r--   0     1000     1000    20357 2023-05-03 13:21:11.000000 ferveo-0.1.8/src/lib.rs
--rw-rw-r--   0     1000     1000     3494 2023-05-03 13:21:11.000000 ferveo-0.1.8/test/test_ferveo.py
--rw-rw-r--   0     1000     1000     1507 2023-05-03 13:21:11.000000 ferveo-0.1.8/test/test_serialization.py
--rw-rw-r--   0     1000     1000    55603 2023-05-03 13:29:17.000000 ferveo-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 ferveo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 ferveo-0.1.9/local_dependencies/ferveo-common/Cargo.toml
+-rw-rw-r--   0     1000     1000     6907 2023-05-05 09:07:06.000000 ferveo-0.1.9/local_dependencies/ferveo-common/src/keypair.rs
+-rw-rw-r--   0     1000     1000      120 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/ferveo-common/src/lib.rs
+-rw-rw-r--   0     1000     1000     4000 2023-04-26 12:06:08.000000 ferveo-0.1.9/local_dependencies/ferveo-common/src/serialization.rs
+-rw-rw-r--   0     1000     1000      406 2023-04-25 07:31:20.000000 ferveo-0.1.9/local_dependencies/ferveo-common/src/utils.rs
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/Cargo.toml
+-rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/BENCHMARK.md
+-rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/README.md
+-rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
+-rw-rw-r--   0     1000     1000    19154 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/benches/tpke.rs
+-rw-rw-r--   0     1000     1000     1259 2023-04-25 07:31:20.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/api.rs
+-rw-rw-r--   0     1000     1000     7780 2023-04-28 12:33:25.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
+-rw-rw-r--   0     1000     1000     5498 2023-04-26 08:55:27.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/combine.rs
+-rw-rw-r--   0     1000     1000     3429 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/context.rs
+-rw-rw-r--   0     1000     1000    11504 2023-05-05 13:45:09.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/decryption.rs
+-rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
+-rw-rw-r--   0     1000     1000     2183 2023-04-25 07:31:20.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/key_share.rs
+-rw-rw-r--   0     1000     1000    29312 2023-05-05 14:11:07.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/lib.rs
+-rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/refresh.rs
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 ferveo-0.1.9/local_dependencies/ferveo/Cargo.toml
+-rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/ferveo/Cargo.lock
+-rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.9/local_dependencies/ferveo/README.md
+-rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/bench_main.rs
+-rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
+-rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/mod.rs
+-rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/pairing.rs
+-rw-rw-r--   0     1000     1000     3478 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
+-rw-rw-r--   0     1000     1000     3257 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
+-rw-rw-r--   0     1000     1000     2897 2023-04-25 07:31:20.000000 ferveo-0.1.9/local_dependencies/ferveo/examples/bench_ark_sizes.rs
+-rw-rw-r--   0     1000     1000     4336 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/ferveo/examples/bench_primitives_size.rs
+-rw-rw-r--   0     1000     1000    19003 2023-05-05 14:22:48.000000 ferveo-0.1.9/local_dependencies/ferveo/src/api.rs
+-rw-rw-r--   0     1000     1000    24426 2023-05-05 09:07:06.000000 ferveo-0.1.9/local_dependencies/ferveo/src/dkg/pv.rs
+-rw-rw-r--   0     1000     1000    24978 2023-05-05 09:07:06.000000 ferveo-0.1.9/local_dependencies/ferveo/src/dkg.rs
+-rw-rw-r--   0     1000     1000    17470 2023-05-05 14:12:16.000000 ferveo-0.1.9/local_dependencies/ferveo/src/lib.rs
+-rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/ferveo/src/primitives.rs
+-rw-rw-r--   0     1000     1000    21326 2023-05-04 14:39:38.000000 ferveo-0.1.9/local_dependencies/ferveo/src/pvss.rs
+-rw-rw-r--   0     1000     1000     1976 2023-05-04 12:39:35.000000 ferveo-0.1.9/local_dependencies/ferveo/src/validator.rs
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.9/local_dependencies/subproductdomain/Cargo.toml
+-rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.9/local_dependencies/subproductdomain/src/lib.rs
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 ferveo-0.1.9/Cargo.toml
+-rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.9/.gitignore
+-rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.9/LICENSE
+-rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.9/MANIFEST.in
+-rw-rw-r--   0     1000     1000      226 2023-05-05 14:38:23.000000 ferveo-0.1.9/README.md
+-rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.9/build.rs
+-rw-rw-r--   0     1000     1000     2895 2023-05-05 14:20:00.000000 ferveo-0.1.9/examples/server_api_precomputed.py
+-rw-rw-r--   0     1000     1000     2997 2023-05-05 14:20:00.000000 ferveo-0.1.9/examples/server_api_simple.py
+-rw-rw-r--   0     1000     1000      383 2023-04-26 12:06:08.000000 ferveo-0.1.9/ferveo/__init__.py
+-rw-rw-r--   0     1000     1000     3691 2023-05-05 09:07:06.000000 ferveo-0.1.9/ferveo/__init__.pyi
+-rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.9/ferveo/py.typed
+-rw-rw-r--   0     1000     1000      316 2023-04-14 08:59:50.000000 ferveo-0.1.9/pyproject.toml
+-rw-rw-r--   0     1000     1000     1444 2023-05-05 16:42:07.000000 ferveo-0.1.9/setup.py
+-rw-rw-r--   0     1000     1000    20016 2023-05-05 14:11:07.000000 ferveo-0.1.9/src/lib.rs
+-rw-rw-r--   0     1000     1000     4592 2023-05-05 16:13:12.000000 ferveo-0.1.9/test/test_ferveo.py
+-rw-rw-r--   0     1000     1000     1507 2023-05-05 09:07:06.000000 ferveo-0.1.9/test/test_serialization.py
+-rw-rw-r--   0     1000     1000    57493 2023-05-05 16:42:17.000000 ferveo-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 ferveo-0.1.9/PKG-INFO
```

### Comparing `ferveo-0.1.8/local_dependencies/subproductdomain/src/lib.rs` & `ferveo-0.1.9/local_dependencies/subproductdomain/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/Cargo.toml` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/BENCHMARK.md` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/BENCHMARK.md`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/arkworks.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/benches/arkworks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/tpke.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/benches/tpke.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/api.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/api.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/ciphertext.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/ciphertext.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/combine.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/combine.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/context.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/context.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/decryption.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/decryption.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/key_share.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/key_share.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/lib.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -511,31 +511,42 @@
 
         let (pubkey, _, contexts) =
             setup_simple::<E>(threshold, shares_num, &mut rng);
         let g_inv = &contexts[0].setup_params.g_inv;
 
         let ciphertext = encrypt::<E>(msg, aad, &pubkey, rng).unwrap();
 
+        // We need at least threshold shares to decrypt
         let decryption_shares: Vec<_> = contexts
             .iter()
             .map(|c| c.create_share(&ciphertext, aad).unwrap())
+            .take(threshold)
             .collect();
-
-        let shared_secret = make_shared_secret(
-            &contexts[0].public_decryption_contexts,
-            &decryption_shares,
-        );
+        let pub_contexts =
+            contexts[0].public_decryption_contexts[..threshold].to_vec();
+        let shared_secret =
+            make_shared_secret(&pub_contexts, &decryption_shares);
 
         test_ciphertext_validation_fails(
             msg,
             aad,
             &ciphertext,
             &shared_secret,
             g_inv,
         );
+
+        // If we use less than threshold shares, we should fail
+        let decryption_shares = decryption_shares[..threshold - 1].to_vec();
+        let pub_contexts = pub_contexts[..threshold - 1].to_vec();
+        let shared_secret =
+            make_shared_secret(&pub_contexts, &decryption_shares);
+
+        let result =
+            decrypt_with_shared_secret(&ciphertext, aad, &shared_secret, g_inv);
+        assert!(result.is_err());
     }
 
     #[test]
     fn tdec_precomputed_variant_e2e() {
         let mut rng = &mut test_rng();
         let shares_num = 16;
         let msg: &[u8] = "abc".as_bytes();
```

### Comparing `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/refresh.rs` & `ferveo-0.1.9/local_dependencies/group-threshold-cryptography/src/refresh.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/Cargo.toml` & `ferveo-0.1.9/local_dependencies/ferveo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/Cargo.lock` & `ferveo-0.1.9/local_dependencies/ferveo/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs` & `ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pairing.rs` & `ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/pairing.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs` & `ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs` & `ferveo-0.1.9/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/examples/bench_ark_sizes.rs` & `ferveo-0.1.9/local_dependencies/ferveo/examples/bench_ark_sizes.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/examples/bench_primitives_size.rs` & `ferveo-0.1.9/local_dependencies/ferveo/examples/bench_primitives_size.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/api.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/api.rs`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 pub use ferveo_common::{Keypair, PublicKey};
 use group_threshold_cryptography as tpke;
 use rand::RngCore;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 pub use tpke::api::{
     decrypt_with_shared_secret, encrypt, prepare_combine_simple,
-    share_combine_precomputed, share_combine_simple, Ciphertext,
-    DecryptionSharePrecomputed, DecryptionShareSimple, DomainPoint, Fr,
-    G1Affine, G1Prepared, SharedSecret, E,
+    share_combine_precomputed, share_combine_simple, Ciphertext, DomainPoint,
+    Fr, G1Affine, G1Prepared, SharedSecret, E,
 };
 
-use crate::{do_verify_aggregation, PVSSMap, Result};
+use crate::{do_verify_aggregation, Error, PVSSMap, Result};
 pub use crate::{
     EthereumAddress, PubliclyVerifiableSS as Transcript, Validator,
 };
 
+pub type DecryptionSharePrecomputed = tpke::api::DecryptionSharePrecomputed;
+
 // Normally, we would use a custom trait for this, but we can't because
 // the arkworks will not let us create a blanket implementation for G1Affine
 // and Fr types. So instead, we're using this shared utility function:
 pub fn to_bytes<T: CanonicalSerialize>(item: &T) -> Result<Vec<u8>> {
     let mut writer = Vec::new();
     item.serialize_compressed(&mut writer)?;
     Ok(writer)
@@ -125,15 +126,14 @@
         }
         Ok(AggregatedTranscript(crate::pvss::aggregate(&self.0.vss)))
     }
 
     pub fn public_params(&self) -> DkgPublicParameters {
         DkgPublicParameters {
             g1_inv: self.0.pvss_params.g_inv(),
-            domain_points: self.0.domain.elements().collect(),
         }
     }
 }
 
 fn make_pvss_map(messages: &[ValidatorMessage]) -> PVSSMap<E> {
     let mut pvss_map: PVSSMap<E> = PVSSMap::new();
     messages.iter().for_each(|(validator, transcript)| {
@@ -158,15 +158,15 @@
     ) -> Result<bool> {
         let pvss_params = crate::pvss::PubliclyVerifiableParams::<E>::default();
         let domain = Radix2EvaluationDomain::<Fr>::new(shares_num as usize)
             .expect("Unable to construct an evaluation domain");
 
         let is_valid_optimistic = self.0.verify_optimistic();
         if !is_valid_optimistic {
-            return Err(crate::Error::InvalidTranscriptAggregate);
+            return Err(Error::InvalidTranscriptAggregate);
         }
 
         let pvss_map = make_pvss_map(messages);
         let validators: Vec<_> = messages
             .iter()
             .map(|(validator, _)| validator)
             .cloned()
@@ -205,51 +205,61 @@
     pub fn create_decryption_share_simple(
         &self,
         dkg: &Dkg,
         ciphertext: &Ciphertext,
         aad: &[u8],
         validator_keypair: &Keypair<E>,
     ) -> Result<DecryptionShareSimple> {
-        self.0.make_decryption_share_simple(
+        let share = self.0.make_decryption_share_simple(
             ciphertext,
             aad,
             &validator_keypair.decryption_key,
             dkg.0.me.share_index,
             &dkg.0.pvss_params.g_inv(),
-        )
+        )?;
+        Ok(DecryptionShareSimple {
+            share,
+            domain_point: dkg.0.domain.element(dkg.0.me.share_index),
+        })
     }
 }
 
 #[serde_as]
+#[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
+pub struct DecryptionShareSimple {
+    share: tpke::api::DecryptionShareSimple,
+    #[serde_as(as = "serialization::SerdeAs")]
+    domain_point: Fr,
+}
+
+#[serde_as]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct DkgPublicParameters {
     #[serde_as(as = "serialization::SerdeAs")]
     pub g1_inv: G1Prepared,
-    #[serde_as(as = "serialization::SerdeAs")]
-    pub domain_points: Vec<Fr>,
 }
 
 impl DkgPublicParameters {
     pub fn from_bytes(bytes: &[u8]) -> Result<Self> {
         bincode::deserialize(bytes).map_err(|e| e.into())
     }
 
     pub fn to_bytes(&self) -> Result<Vec<u8>> {
         bincode::serialize(self).map_err(|e| e.into())
     }
 }
 
-pub fn combine_shares_simple(
-    dkg_public_params: &DkgPublicParameters,
-    shares: &[DecryptionShareSimple],
-) -> SharedSecret {
-    let domain_points = &dkg_public_params.domain_points;
-    let lagrange_coefficients = prepare_combine_simple::<E>(&domain_points[..]);
+pub fn combine_shares_simple(shares: &[DecryptionShareSimple]) -> SharedSecret {
+    // Pick domain points that are corresponding to the shares we have.
+    let domain_points: Vec<_> = shares.iter().map(|s| s.domain_point).collect();
+    let lagrange_coefficients = prepare_combine_simple::<E>(&domain_points);
+
+    let shares: Vec<_> = shares.iter().cloned().map(|s| s.share).collect();
     let shared_secret =
-        share_combine_simple(shares, &lagrange_coefficients[..]);
+        share_combine_simple(&shares, &lagrange_coefficients[..]);
     SharedSecret(shared_secret)
 }
 
 #[cfg(test)]
 mod test_ferveo_api {
     use itertools::izip;
     use rand::{prelude::StdRng, thread_rng, SeedableRng};
@@ -293,37 +303,14 @@
                 (sender.clone(), dkg.generate_transcript(rng).unwrap())
             })
             .collect();
         (messages, validators, validator_keypairs)
     }
 
     #[test]
-    fn test_dkg_public_key_serialization() {
-        let shares_num = 4;
-        let validator_keypairs = gen_keypairs(shares_num);
-        let validators = validator_keypairs
-            .iter()
-            .enumerate()
-            .map(|(i, keypair)| Validator {
-                address: gen_address(i),
-                public_key: keypair.public(),
-            })
-            .collect::<Vec<_>>();
-
-        let dkg =
-            Dkg::new(1, shares_num, 2, &validators, &validators[0]).unwrap();
-
-        let serialized = dkg.final_key().to_bytes().unwrap();
-        assert_eq!(serialized.len(), DkgPublicKey::serialized_size());
-
-        let deserialized = DkgPublicKey::from_bytes(&serialized).unwrap();
-        assert_eq!(dkg.final_key(), deserialized);
-    }
-
-    #[test]
     fn test_server_api_tdec_precomputed() {
         let rng = &mut StdRng::seed_from_u64(0);
 
         let tau = 1;
         let shares_num = 4;
         // In precomputed variant, the security threshold is equal to the number of shares
         // TODO: Refactor DKG constructor to not require security threshold or this case.
@@ -336,16 +323,14 @@
         // Now that every validator holds a dkg instance and a transcript for every other validator,
         // every validator can aggregate the transcripts
         let me = validators[0].clone();
         let mut dkg =
             Dkg::new(tau, shares_num, security_threshold, &validators, &me)
                 .unwrap();
 
-        // Lets say that we've only receives `security_threshold` transcripts
-        let messages = messages[..security_threshold as usize].to_vec();
         let pvss_aggregated = dkg.aggregate_transcripts(&messages).unwrap();
         assert!(pvss_aggregated.verify(shares_num, &messages).unwrap());
 
         // At this point, any given validator should be able to provide a DKG public key
         let dkg_public_key = dkg.final_key();
 
         // In the meantime, the client creates a ciphertext and decryption request
@@ -379,23 +364,36 @@
             })
             .collect();
 
         // Now, the decryption share can be used to decrypt the ciphertext
         // This part is part of the client API
 
         let shared_secret = share_combine_precomputed(&decryption_shares);
-
         let plaintext = decrypt_with_shared_secret(
             &ciphertext,
             aad,
             &shared_secret,
             &dkg.0.pvss_params.g_inv(),
         )
         .unwrap();
         assert_eq!(plaintext, msg);
+
+        // Since we're using a precomputed variant, we need all the shares to be able to decrypt
+        // So if we remove one share, we should not be able to decrypt
+        let decryption_shares =
+            decryption_shares[..shares_num as usize - 1].to_vec();
+
+        let shared_secret = share_combine_precomputed(&decryption_shares);
+        let result = decrypt_with_shared_secret(
+            &ciphertext,
+            aad,
+            &shared_secret,
+            &dkg.0.pvss_params.g_inv(),
+        );
+        assert!(result.is_err());
     }
 
     #[test]
     fn test_server_api_tdec_simple() {
         let rng = &mut StdRng::seed_from_u64(0);
 
         let tau = 1;
@@ -403,21 +401,23 @@
         let security_threshold = 3;
 
         let (messages, validators, validator_keypairs) =
             make_test_inputs(rng, tau, security_threshold, shares_num);
 
         // Now that every validator holds a dkg instance and a transcript for every other validator,
         // every validator can aggregate the transcripts
-        let me = validators[0].clone();
-        let mut dkg =
-            Dkg::new(tau, shares_num, security_threshold, &validators, &me)
-                .unwrap();
+        let mut dkg = Dkg::new(
+            tau,
+            shares_num,
+            security_threshold,
+            &validators,
+            &validators[0],
+        )
+        .unwrap();
 
-        // Lets say that we've only receives `security_threshold` transcripts
-        let messages = messages[..security_threshold as usize].to_vec();
         let pvss_aggregated = dkg.aggregate_transcripts(&messages).unwrap();
         assert!(pvss_aggregated.verify(shares_num, &messages).unwrap());
 
         // At this point, any given validator should be able to provide a DKG public key
         let public_key = dkg.final_key();
 
         // In the meantime, the client creates a ciphertext and decryption request
@@ -450,27 +450,41 @@
                     .unwrap()
             })
             .collect();
 
         // Now, the decryption share can be used to decrypt the ciphertext
         // This part is part of the client API
 
-        let lagrange_coeffs =
-            prepare_combine_simple::<E>(&dkg.public_params().domain_points);
-        let shared_secret =
-            share_combine_simple(&decryption_shares, &lagrange_coeffs);
+        // In simple variant, we only need `security_threshold` shares to be able to decrypt
+        let decryption_shares =
+            decryption_shares[..security_threshold as usize].to_vec();
 
+        let shared_secret = combine_shares_simple(&decryption_shares);
         let plaintext = decrypt_with_shared_secret(
             &ciphertext,
             aad,
-            &shared_secret,
+            &shared_secret.0,
             &dkg.public_params().g1_inv,
         )
         .unwrap();
         assert_eq!(plaintext, msg);
+
+        // Let's say that we've only received `security_threshold - 1` shares
+        // In this case, we should not be able to decrypt
+        let decryption_shares =
+            decryption_shares[..security_threshold as usize - 1].to_vec();
+
+        let shared_secret = combine_shares_simple(&decryption_shares);
+        let result = decrypt_with_shared_secret(
+            &ciphertext,
+            aad,
+            &shared_secret.0,
+            &dkg.public_params().g1_inv,
+        );
+        assert!(result.is_err());
     }
 
     #[test]
     fn server_side_local_verification() {
         let rng = &mut StdRng::seed_from_u64(0);
 
         let tau = 1;
```

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/dkg/pv.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/dkg/pv.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/dkg.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/dkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/lib.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/primitives.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/pvss.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/pvss.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo/src/validator.rs` & `ferveo-0.1.9/local_dependencies/ferveo/src/validator.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo-common/src/keypair.rs` & `ferveo-0.1.9/local_dependencies/ferveo-common/src/keypair.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/local_dependencies/ferveo-common/src/serialization.rs` & `ferveo-0.1.9/local_dependencies/ferveo-common/src/serialization.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/Cargo.toml` & `ferveo-0.1.9/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "ferveo-python"
 authors = ["Piotr Roslaniec <p.roslaniec@gmail.com>"]
-version = "0.1.8"
+version = "0.1.9"
 edition = "2018"
 
 [lib]
 crate-type = ["cdylib"]
 name = "ferveo_py"
 
 [features]
```

### Comparing `ferveo-0.1.8/LICENSE` & `ferveo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/examples/server_api_precomputed.py` & `ferveo-0.1.9/examples/server_api_precomputed.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,14 @@
     tau=tau,
     shares_num=shares_num,
     security_threshold=security_threshold,
     validators=validators,
     me=validators[0],
 )
 
-# Let's say that we've only received `security_threshold` transcripts
-messages = messages[:security_threshold]
-
 # Server can aggregate the transcripts
 server_aggregate = dkg.aggregate_transcripts(messages)
 assert server_aggregate.verify(shares_num, messages)
 
 # And the client can also aggregate and verify the transcripts
 client_aggregate = AggregatedTranscript(messages)
 assert client_aggregate.verify(shares_num, messages)
```

### Comparing `ferveo-0.1.8/examples/server_api_simple.py` & `ferveo-0.1.9/examples/server_api_simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,17 +45,14 @@
     tau=tau,
     shares_num=shares_num,
     security_threshold=security_threshold,
     validators=validators,
     me=me,
 )
 
-# Let's say that we've only received `security_threshold` transcripts
-messages = messages[:security_threshold]
-
 # Server can aggregate the transcripts
 server_aggregate = dkg.aggregate_transcripts(messages)
 assert server_aggregate.verify(shares_num, messages)
 
 # And the client can also aggregate and verify the transcripts
 client_aggregate = AggregatedTranscript(messages)
 assert client_aggregate.verify(shares_num, messages)
@@ -90,15 +87,15 @@
         dkg, ciphertext, aad, validator_keypair
     )
     decryption_shares.append(decryption_share)
 
 # Now, the decryption share can be used to decrypt the ciphertext
 # This part is in the client API
 
-shared_secret = combine_decryption_shares_simple(decryption_shares, dkg.public_params)
+shared_secret = combine_decryption_shares_simple(decryption_shares)
 
 # The client should have access to the public parameters of the DKG
 
 plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.public_params)
 assert bytes(plaintext) == msg
 
 print("Success!")
```

### Comparing `ferveo-0.1.8/ferveo/__init__.pyi` & `ferveo-0.1.9/ferveo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/setup.py` & `ferveo-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ferveo",
     description="Ferveo DKG scheme",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.8",
+    version="0.1.9",
     author="Piotr Roslaniec",
     author_email="p.roslaniec@gmail.com",
     url="https://github.com/nucypher/ferveo/tree/master/ferveo-python",
     rust_extensions=[RustExtension(
         "ferveo._ferveo", binding=Binding.PyO3, debug=False)],
     packages=["ferveo"],
     package_data={
```

### Comparing `ferveo-0.1.8/src/lib.rs` & `ferveo-0.1.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -66,28 +66,21 @@
             .map_err(map_py_err)?;
     Ok(Ciphertext(ciphertext))
 }
 
 #[pyfunction]
 pub fn combine_decryption_shares_simple(
     shares: Vec<DecryptionShareSimple>,
-    dkg_public_params: &DkgPublicParameters,
 ) -> SharedSecret {
     let shares = shares
         .iter()
         .map(|share| share.0.clone())
         .collect::<Vec<_>>();
-    let domain_points = &dkg_public_params.0.domain_points;
-    let lagrange_coefficients =
-        ferveo::api::prepare_combine_simple::<E>(&domain_points[..]);
-    let shared_secret = ferveo::api::share_combine_simple(
-        &shares[..],
-        &lagrange_coefficients[..],
-    );
-    SharedSecret(ferveo::api::SharedSecret(shared_secret))
+    let shared_secret = ferveo::api::combine_shares_simple(&shares[..]);
+    SharedSecret(shared_secret)
 }
 
 #[pyfunction]
 pub fn combine_decryption_shares_precomputed(
     shares: Vec<DecryptionSharePrecomputed>,
 ) -> SharedSecret {
     let shares = shares
@@ -671,18 +664,15 @@
                     .unwrap()
             })
             .collect();
 
         // Now, the decryption share can be used to decrypt the ciphertext
         // This part is part of the client API
 
-        let shared_secret = combine_decryption_shares_simple(
-            decryption_shares,
-            &dkg.public_params(),
-        );
+        let shared_secret = combine_decryption_shares_simple(decryption_shares);
 
         // TODO: Fails because of a bad shared secret
         let plaintext = decrypt_with_shared_secret(
             &ciphertext,
             aad,
             &shared_secret,
             &dkg.public_params(),
```

### Comparing `ferveo-0.1.8/test/test_serialization.py` & `ferveo-0.1.9/test/test_serialization.py`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.8/Cargo.lock` & `ferveo-0.1.9/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aead"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c192eb8f11fc081b0fe4259ba5af04217d4e0faddd02417310a927911abd7c8"
+checksum = "d122413f284cf2d62fb1b7db97e02edb8cda96d769b16e443a4f6195e35662b0"
 dependencies = [
  "crypto-common",
  "generic-array",
 ]
 
 [[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "ahash"
 version = "0.8.3"
@@ -62,17 +62,17 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "ark-bls12-381"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c775f0d12169cba7aae4caeb547bb6a50781c7449a8aa53793827c9ec4abf488"
 dependencies = [
@@ -80,34 +80,34 @@
  "ark-ff",
  "ark-serialize",
  "ark-std",
 ]
 
 [[package]]
 name = "ark-ec"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52d7f0c52aff14f216200a9eee06a9990fee2e51fc9599e226df448ad3232886"
+checksum = "defd9a439d56ac24968cca0571f598a61bc8c55f71d50a89cda591cb750670ba"
 dependencies = [
  "ark-ff",
  "ark-poly",
  "ark-serialize",
  "ark-std",
  "derivative",
  "hashbrown 0.13.2",
  "itertools",
  "num-traits",
  "zeroize",
 ]
 
 [[package]]
 name = "ark-ff"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51ee31d8869a353433524dbd5a8f51f95cdafe7c66d458956ec13aa737198562"
+checksum = "ec847af850f44ad29048935519032c33da8aa03340876d351dfab5660d2966ba"
 dependencies = [
  "ark-ff-asm",
  "ark-ff-macros",
  "ark-serialize",
  "ark-std",
  "derivative",
  "digest",
@@ -117,69 +117,69 @@
  "paste",
  "rustc_version",
  "zeroize",
 ]
 
 [[package]]
 name = "ark-ff-asm"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fc8f7ec7fdcc20f3f110783c043d80479b42f500003cf92b71ca90f34a2ba0e"
+checksum = "3ed4aa4fe255d0bc6d79373f7e31d2ea147bcf486cba1be5ba7ea85abdb92348"
 dependencies = [
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ark-ff-macros"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15aa320e38052d644e569740bad208e5f9f5fafedcc9e6b1557f723be1b7ff8d"
+checksum = "7abe79b0e4288889c4574159ab790824d0033b9fdcb2a112a3182fac2e514565"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ark-poly"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88d2e8741caf33ab3063f1fc65617716ffb18cba8e872998aa2eef0d4e4b56d1"
+checksum = "d320bfc44ee185d899ccbadfa8bc31aab923ce1558716e1997a1e74057fe86bf"
 dependencies = [
  "ark-ff",
  "ark-serialize",
  "ark-std",
  "derivative",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "ark-serialize"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ea39d00a8a4c832e6f6520e58ccec7bf909c4845863512e9b8656fd47df355"
+checksum = "adb7b85a02b83d2f22f89bd5cac66c9c89474240cb6207cb1efc16d098e822a5"
 dependencies = [
  "ark-serialize-derive",
  "ark-std",
  "digest",
  "num-bigint",
 ]
 
 [[package]]
 name = "ark-serialize-derive"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "101333772a4020c883890811500d5ecc704c545a90140629af5c3b9f00d78953"
+checksum = "ae3281bc6d0fd7e549af32b52511e1302185bd688fd3359fa36423346ff682ea"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ark-std"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94893f1e0c6eeab764ade8dc4c0db24caf4fe7cbbaafc0eba0a9030f447b5185"
@@ -245,44 +245,32 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "bstr"
-version = "0.2.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
-dependencies = [
- "lazy_static",
- "memchr",
- "regex-automata",
- "serde",
-]
-
-[[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "bytemuck"
-version = "1.13.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c041d3eab048880cb0b86b256447da3f18859a163c3b8d8893f4e6368abe6393"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -296,17 +284,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chacha20"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7fc89c7c5b9e7a02dfe45cd2367bae382f9ed31c61ca8debe5f827c420a2f08"
+checksum = "c3613f74bd2eac03dad61bd53dbe620703d4371614fe0bc3b9f04dd36fe4e818"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
@@ -320,17 +308,17 @@
  "cipher",
  "poly1305",
  "zeroize",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
  "num-integer",
  "num-traits",
  "serde",
  "winapi",
 ]
@@ -360,17 +348,17 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "cipher"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1873270f8f7942c191139cb8a40fd228da6c3fd2fc376d7e92d47aa14aeb59e"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
  "zeroize",
 ]
 
 [[package]]
@@ -382,17 +370,17 @@
  "bitflags",
  "textwrap 0.11.0",
  "unicode-width",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "bitflags",
  "clap_lex",
  "indexmap",
  "textwrap 0.16.0",
 ]
 
@@ -423,32 +411,32 @@
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpp_demangle"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eeaa953eaad386a53111e47172c2fedba671e5684c8dd601a5f474f4f118710f"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.3.6"
@@ -481,15 +469,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
 dependencies = [
  "anes",
  "atty",
  "cast",
  "ciborium",
- "clap 3.2.23",
+ "clap 3.2.25",
  "criterion-plot 0.5.0",
  "itertools",
  "lazy_static",
  "num-traits",
  "oorandom",
  "plotters",
  "rayon",
@@ -519,51 +507,51 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset 0.8.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -573,21 +561,20 @@
  "generic-array",
  "rand_core 0.6.4",
  "typenum",
 ]
 
 [[package]]
 name = "csv"
-version = "1.1.6"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22813a6dc45b335f9bade10bf7271dc477e81113e89eb251a0bc2a8a81c536e1"
+checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
 dependencies = [
- "bstr",
  "csv-core",
- "itoa 0.4.8",
+ "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "csv-core"
 version = "0.1.10"
@@ -595,89 +582,89 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90d59d9acd2a682b4e40605a242f6670eaa58c5957471cbf85e8aa6a0b97a5e8"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebfa40bda659dd5c864e65f4c9a2b0aff19bea56b017b9b77c73d3766a453a38"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "457ce6757c5c70dc6ecdbda6925b958aae7f959bda7d8fb9bde889e34a09dc03"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebf883b7aacd7b2aeb2a7b338648ee19f57c140d4ee8e52c68979c6b2f7f2263"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.3"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0808e1bd8671fb44a113a14e13497557533369847788fa2ae912b6ebfce9fa8"
+checksum = "0558d22a7b463ed0241e993f76f09f30b126687447751a8638587b864e4b3944"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.3"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "001d80444f28e193f30c2f293455da62dcf9a6b29918a4253152ae2b1de592cb"
+checksum = "ab8bfa2e259f8ee1ce5e97824a3c55ec4404a0d772ca7fa96bf19f0752a046eb"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.3"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b36230598a2d5de7ec1c6f51f72d8a99a9208daff41de2084d06e3fd3ea56685"
+checksum = "29a358ff9f12ec09c3e61fef9b5a9902623a695a46a917b07f269bff1445611a"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "debugid"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6ee87af31d84ef885378aebca32be3d682b0e0dc119d5b4860a2c5bb5046730"
@@ -689,26 +676,26 @@
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
@@ -720,18 +707,39 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "fastrand"
-version = "1.8.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "ferveo"
 version = "0.1.1"
@@ -773,15 +781,15 @@
  "rand_core 0.6.4",
  "serde",
  "serde_with",
 ]
 
 [[package]]
 name = "ferveo-python"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "derive_more",
  "ferveo",
  "ferveo-common",
  "itertools",
  "pyo3",
  "pyo3-build-config",
@@ -792,15 +800,15 @@
 name = "ferveo-wasm"
 version = "0.1.0"
 dependencies = [
  "console_error_panic_hook",
  "derive_more",
  "ferveo",
  "ferveo-common",
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
  "group-threshold-cryptography",
  "itertools",
  "js-sys",
  "rand 0.8.5",
  "rand_core 0.6.4",
  "serde",
  "wasm-bindgen",
@@ -824,17 +832,17 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
@@ -845,30 +853,30 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.27.1"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "221996f774192f0f718773def8201c4ae31f02616a54ccfc2d358bb0e5cefdec"
+checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
 
 [[package]]
 name = "group-threshold-cryptography"
 version = "0.1.0"
 dependencies = [
  "ark-bls12-381",
  "ark-ec",
@@ -929,31 +937,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
@@ -966,17 +980,17 @@
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
  "serde",
 ]
 
 [[package]]
@@ -990,15 +1004,15 @@
 version = "0.10.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3886428c6400486522cf44b8626e7b94ad794c14390290f2a274dcf728a58f"
 dependencies = [
  "ahash 0.7.6",
  "atty",
  "indexmap",
- "itoa 1.0.5",
+ "itoa",
  "lazy_static",
  "log",
  "num-format",
  "quick-xml",
  "rgb",
  "str_stack",
 ]
@@ -1021,33 +1035,38 @@
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+dependencies = [
+ "hermit-abi 0.3.1",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "0.4.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
-
-[[package]]
-name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
 version = "0.3.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
@@ -1058,28 +1077,34 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "link-cplusplus"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
+
+[[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1108,17 +1133,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.5.8"
+version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b182332558b18d807c4ce1ca8ca983b34c3ee32765e47b3f0f69b90355cc1dc"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
@@ -1126,23 +1151,14 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
@@ -1188,15 +1204,15 @@
 [[package]]
 name = "num-format"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a652d9771a63711fd3c3deb670acfbe5c30a4072e664d7a3bf5a9e1056ac72c3"
 dependencies = [
  "arrayvec",
- "itoa 1.0.5",
+ "itoa",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
@@ -1231,17 +1247,17 @@
 checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
@@ -1249,71 +1265,48 @@
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
  "instant",
  "lock_api",
- "parking_lot_core 0.8.6",
-]
-
-[[package]]
-name = "parking_lot"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
-dependencies = [
- "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
  "cfg-if",
  "instant",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
-name = "parking_lot_core"
-version = "0.9.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
-dependencies = [
- "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-sys",
-]
-
-[[package]]
 name = "paste"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "plotters"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
 dependencies = [
@@ -1361,15 +1354,15 @@
  "criterion 0.3.6",
  "findshlibs",
  "inferno",
  "lazy_static",
  "libc",
  "log",
  "nix",
- "parking_lot 0.11.2",
+ "parking_lot",
  "smallvec",
  "symbolic-demangle",
  "tempfile",
  "thiserror",
 ]
 
 [[package]]
@@ -1385,70 +1378,70 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset 0.8.0",
- "parking_lot 0.12.1",
+ "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8533f14c8382aaad0d592c812ac3b826162128b65662331e1127b45c3d18536b"
@@ -1520,41 +1513,41 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
 dependencies = [
  "rand_core 0.5.1",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -1564,72 +1557,80 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "regex"
-version = "1.7.1"
+name = "redox_syscall"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "regex-syntax",
+ "bitflags",
 ]
 
 [[package]]
-name = "regex-automata"
-version = "0.1.10"
+name = "regex"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+dependencies = [
+ "regex-syntax",
+]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
-
-[[package]]
-name = "remove_dir_all"
-version = "0.5.3"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
-dependencies = [
- "winapi",
-]
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rgb"
-version = "0.8.35"
+version = "0.8.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7495acf66551cdb696b7711408144bcd3194fc78e32f3a09e809bfe7dd4a7ce3"
+checksum = "20ec2d3e3fc7a92ced357df9cebd5a10b6fb2aa1ee797bf7e9ce2f17dffc8f59"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.37.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bbfc1d1c7c40c01715f47d71444744a81669ca84e8b63e25a55e169b1f86433"
+dependencies = [
+ "bitflags",
+ "errno",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1646,29 +1647,29 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scratch"
-version = "1.0.3"
+version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
+checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
 
 [[package]]
 name = "semver"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bc9567378fc7690d6b2addae4e60ac2eeea07becb2c64b9f218b53865cba2a"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.9"
@@ -1686,60 +1687,60 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.93"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
- "itoa 1.0.5",
+ "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_with"
-version = "2.2.0"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30d904179146de381af4c93d3af6ca4984b3152db687dacb9c3c35e86f39809c"
+checksum = "07ff71d2c147a7b57362cead5e22f772cd52f6ab31cfcd9edcd7f6aeb2a0afbe"
 dependencies = [
  "base64",
  "chrono",
  "hex",
  "indexmap",
  "serde",
  "serde_json",
  "serde_with_macros",
  "time",
 ]
 
 [[package]]
 name = "serde_with_macros"
-version = "2.2.0"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1966009f3c05f095697c537312f5415d1e3ed31ce0a56942bac4c771c5c335e"
+checksum = "881b6f881b17d13214e5d494c939ebab463d01264ce1811e9d4ac3a882e7695f"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
@@ -1812,17 +1813,17 @@
  "cpp_demangle",
  "rustc-demangle",
  "symbolic-common",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1833,43 +1834,30 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "synstructure"
-version = "0.12.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.107",
- "unicode-xid",
-]
-
-[[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.3.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "libc",
- "redox_syscall",
- "remove_dir_all",
- "winapi",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -1910,35 +1898,35 @@
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.17"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a561bf4617eebd33bca6434b988f39ed798e527f51a1e797d0ee4f61c0a38376"
+checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
 dependencies = [
- "itoa 1.0.5",
+ "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
 
 [[package]]
 name = "time-macros"
-version = "0.2.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d967f99f534ca7e495c575c62638eebc2898a8c84c119b89e250477bc4ba16b2"
+checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
@@ -1953,31 +1941,25 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
-name = "unicode-xid"
-version = "0.2.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "universal-hash"
@@ -1999,20 +1981,19 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.9.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2043,28 +2024,28 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-derive"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7301886930edaa72b7d102655ea395774aa9f0614c1a491393648a5fec34435"
 dependencies = [
  "js-sys",
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2090,15 +2071,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
+ "syn 1.0.109",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
@@ -2167,92 +2148,166 @@
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
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
-version = "1.3.3"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44bf07cb3e50ea2003396695d58bf46bc9887a1f362260446fad6bc4e79bd36c"
+checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.107",
- "synstructure",
+ "syn 2.0.15",
 ]
```

### Comparing `ferveo-0.1.8/PKG-INFO` & `ferveo-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferveo
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Piotr Roslaniec <p.roslaniec@gmail.com>
 Author-email: Piotr Roslaniec <p.roslaniec@gmail.com>
 Requires-Python: >=3.7
```

