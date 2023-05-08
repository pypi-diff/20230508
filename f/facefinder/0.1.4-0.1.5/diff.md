# Comparing `tmp/facefinder-0.1.4.tar.gz` & `tmp/facefinder-0.1.5.tar.gz`

## Comparing `facefinder-0.1.4.tar` & `facefinder-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.4/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.4/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.4/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.4/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.4/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    22216 2023-05-03 03:58:18.000000 facefinder-0.1.4/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.4/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.4/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-05-03 04:00:17.000000 facefinder-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.5/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.5/.gitignore
+-rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.5/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.5/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.5/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    22918 2023-05-08 10:50:24.000000 facefinder-0.1.5/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.5/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.5/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-05-08 10:52:24.000000 facefinder-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.5/PKG-INFO
```

### Comparing `facefinder-0.1.4/.github/workflows/CI.yml` & `facefinder-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/.gitignore` & `facefinder-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/pyproject.toml` & `facefinder-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/src/python/facefinder/interact.py` & `facefinder-0.1.5/src/python/facefinder/interact.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/src/python/facefinder/metadata.py` & `facefinder-0.1.5/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/src/python/facefinder/metrics.py` & `facefinder-0.1.5/src/python/facefinder/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,22 +457,26 @@
         total_distance += np.sum(distance)
         total_size += distance.size
 
     return total_distance / total_size
 
 
 def merge_metrics(metrics: list[dict[str, Any]]) -> dict[str, Any]:
+    if not metrics:
+        raise ValueError(f"list of metrics must not be empty, {len(metrics)=}")
+
     paths = metrics[0]["paths"]
     representations = {m["metadata"]["model"]: m["representations"] for m in metrics}
     metadata = {
         "model": [m["metadata"]["model"] for m in metrics],
         "target_distance_bias": [
             m["metadata"]["target_distance_bias"] for m in metrics
         ],
     }
+    """
     means = [distance_mean(m["distances"]) for m in metrics]
     grand_mean = np.mean(np.array(means))
     distances = {
         "embedding_target": [],
         "embedding_embedding": [],
         "candidate_target": [],
         "candidate_embedding": [],
@@ -484,14 +488,32 @@
             if len(v.shape) == 1:
                 v = v[:, None]
             distances[k].append(scaler(v)[:, :, None])
     distances = {
         k: np.mean(np.concatenate(v, axis=2), axis=2) * 2 * grand_mean
         for k, v in distances.items()
     }
+    """
+
+    # TODO THIS IS A TEMPORARY FIX THAT DOES NOT SCALE THE VALUES
+    distances = {
+        "embedding_target": [],
+        "embedding_embedding": [],
+        "candidate_target": [],
+        "candidate_embedding": [],
+        "pairs": [],
+    }
+
+    for k in distances:
+        for m in metrics:
+            distance = m["distances"][k]
+            if len(distance.shape) == 1:
+                distance = distance[:, None]
+            distances[k].append(distance[..., None])
+        distances[k] = np.mean(np.concatenate(distances[k], axis=2), axis=2)
 
     candidate_weighted_distances = calculate_weighted_distances(
         distances["embedding_target"],
         distances["candidate_embedding"],
         np.mean(metadata["target_distance_bias"]),
     )
     embedding_weighted_distances = calculate_weighted_distances(
@@ -593,15 +615,15 @@
         image_path = str(output_dir.joinpath(image_name))
         cv2.imwrite(image_path, cv2.imread(str(path)))
 
 
 def main(interactive: bool = False) -> None:
     # Processing Images
     metrics = get_multimodel_metrics(
-        ["Facenet512"], target_distance_bias=1
+        ["Facenet512", "SFace"], target_distance_bias=1
     )  # "SFace", "ArcFace"])
 
     # Saving scored images
     save_processed_embedding_images(metrics)
     save_processed_candidate_images(metrics)
 
     if interactive:
```

### Comparing `facefinder-0.1.4/src/python/facefinder/prompting.py` & `facefinder-0.1.5/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.4/Cargo.lock` & `facefinder-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

