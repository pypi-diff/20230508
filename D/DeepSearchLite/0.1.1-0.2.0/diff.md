# Comparing `tmp/DeepSearchLite-0.1.1.tar.gz` & `tmp/DeepSearchLite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSearchLite-0.1.1.tar", last modified: Sun May  7 04:14:21 2023, max compression
+gzip compressed data, was "DeepSearchLite-0.2.0.tar", last modified: Mon May  8 16:17:17 2023, max compression
```

## Comparing `DeepSearchLite-0.1.1.tar` & `DeepSearchLite-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/DeepSearchLite/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)    13903 2023-05-07 03:48:20.000000 DeepSearchLite-0.1.1/DeepSearchLite/DeepSearchLite.py
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       65 2023-05-07 01:07:56.000000 DeepSearchLite-0.1.1/DeepSearchLite/__init__.py
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)      275 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/SOURCES.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)        1 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/dependency_links.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       35 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/requires.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       15 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/top_level.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1068 2023-05-07 01:06:14.000000 DeepSearchLite-0.1.1/LICENSE
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     2363 2023-05-07 02:09:18.000000 DeepSearchLite-0.1.1/README.md
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       38 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/setup.cfg
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1044 2023-05-07 02:48:29.000000 DeepSearchLite-0.1.1/setup.py
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/DeepSearchLite/
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)    16114 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/DeepSearchLite/DeepSearchLite.py
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       65 2023-05-07 01:07:56.000000 DeepSearchLite-0.2.0/DeepSearchLite/__init__.py
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     6346 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/PKG-INFO
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)      275 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/SOURCES.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)        1 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/dependency_links.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       35 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/requires.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       15 2023-05-08 16:17:17.000000 DeepSearchLite-0.2.0/DeepSearchLite.egg-info/top_level.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     1068 2023-05-07 01:06:14.000000 DeepSearchLite-0.2.0/LICENSE
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     6346 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/PKG-INFO
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     5655 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/README.md
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       38 2023-05-08 16:17:17.500680 DeepSearchLite-0.2.0/setup.cfg
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     1044 2023-05-08 16:14:43.000000 DeepSearchLite-0.2.0/setup.py
```

### Comparing `DeepSearchLite-0.1.1/DeepSearchLite/DeepSearchLite.py` & `DeepSearchLite-0.2.0/DeepSearchLite/DeepSearchLite.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,199 +1,258 @@
 import os
 import pandas as pd
 from PIL import Image
 from tqdm import tqdm
 import numpy as np
 import faiss
-from typing import List, Union, Dict, Callable, Optional
+from typing import List, Union, Dict, Callable, Optional, Any
 
 
-def image_data_with_features_pkl(metadata_dir, model_name):
+def item_data_with_features_pkl(metadata_dir, model_name):
     data_dir = os.path.join(metadata_dir, f"{model_name}")
 
     # Create the directory if it does not exist
     os.makedirs(data_dir, exist_ok=True)
 
-    image_data_with_features_pkl = os.path.join(data_dir, "image_data_features.pkl")
-    return image_data_with_features_pkl
+    item_data_with_features_pkl = os.path.join(data_dir, "item_data_features.pkl")
+    return item_data_with_features_pkl
 
 
-def image_features_vectors_idx(metadata_dir, model_name):
+def item_features_vectors_idx(metadata_dir, model_name):
     data_dir = os.path.join(metadata_dir, f"{model_name}")
 
     # Create the directory if it does not exist
     os.makedirs(data_dir, exist_ok=True)
 
-    image_features_vectors_idx = os.path.join(data_dir, "image_features_vectors.idx")
-    return image_features_vectors_idx
+    item_features_vectors_idx = os.path.join(data_dir, "item_features_vectors.idx")
+    return item_features_vectors_idx
 
 
 class LoadData:
-    """A class for loading data from single/multiple folders or a CSV file"""
+    """A class for loading data from single/multiple folders or a CSV file."""
 
-    def __init__(self):
+    def __init__(self, data_type: str = "image"):
         """
-        Initializes an instance of LoadData class
+        Initializes an instance of LoadData class.
+
+        Parameters:
+        -----------
+        data_type : str, optional (default='image')
+            The type of data to load. Supported types: 'image', 'video', 'text', etc.
         """
-        pass
+        self.data_type = data_type
 
-    def from_folder(self, folder_list: list):
+    def from_folder(self, folder_list: list) -> List[str]:
         """
-        Adds images from the specified folders to the image_list.
+        Adds data files from the specified folders to the data_list.
 
         Parameters:
         -----------
         folder_list : list
-            A list of paths to the folders containing images to be added to the image_list.
+            A list of paths to the folders containing data files to be added to the data_list.
+
+        Returns:
+        --------
+        data_paths : list
+            A list of paths to the loaded data files.
         """
         self.folder_list = folder_list
-        image_path = []
+        data_paths = []
         for folder in self.folder_list:
             for root, dirs, files in os.walk(folder):
                 for file in files:
-                    if file.lower().endswith((".png", ".jpg", ".jpeg", ".gif", ".bmp")):
-                        image_path.append(os.path.join(root, file))
-        return image_path
+                    if self._is_supported_file(file):
+                        data_paths.append(os.path.join(root, file))
+        return data_paths
 
-    def from_csv(self, csv_file_path: str, images_column_name: str):
+    def _is_supported_file(self, file: str) -> bool:
         """
-        Adds images from the specified column of a CSV file to the image_list.
+        Checks if a file has a supported extension based on the data_type.
+
+        Parameters:
+        -----------
+        file : str
+            The file name to check for supported extensions.
+
+        Returns:
+        --------
+        bool
+            True if the file has a supported extension, False otherwise.
+        """
+        if self.data_type == "image":
+            return file.lower().endswith((".png", ".jpg", ".jpeg", ".gif", ".bmp"))
+
+        # TODO: Add other data types (e.g., video, text, etc.) and their supported extensions
+
+        # Add other data types (e.g., video, text, etc.) and their supported extensions
+        # elif self.data_type == 'video':
+        #     return file.lower().endswith((".mp4", ".avi", ".mov", ".mkv"))
+        # elif self.data_type == 'text':
+        #     return file.lower().endswith((".txt", ".csv", ".tsv", ".json"))
+        else:
+            raise ValueError(f"Unsupported data type: {self.data_type}")
+
+    def from_csv(self, csv_file_path: str, items_column_name: str):
+        """
+        Adds items from the specified column of a CSV file to the item_list.
 
         Parameters:
         -----------
         csv_file_path : str
             The path to the CSV file.
-        images_column_name : str
-            The name of the column containing the paths to the images to be added to the image_list.
+        items_column_name : str
+            The name of the column containing the paths to the items to be added to the item_list.
         """
         self.csv_file_path = csv_file_path
-        self.images_column_name = images_column_name
-        return pd.read_csv(self.csv_file_path)[self.images_column_name].to_list()
+        self.items_column_name = items_column_name
+        return pd.read_csv(self.csv_file_path)[self.items_column_name].to_list()
 
 
 class SearchSetup:
-    """A class for setting up and running image similarity search."""
+    """A class for setting up and running similarity search for various data types (e.g., images, videos, texts, etc.)."""
 
     def __init__(
         self,
-        image_list: list,
+        item_list: List[str],
         feature_extractor: Optional[Callable] = None,
         dim_reduction: Optional[Callable] = None,
-        image_count: Optional[int] = None,
         metadata_dir: Optional[str] = "metadata_dir",
         feature_extractor_name: Optional[str] = "feature_extractor",
         mode: str = "index",
+        item_loader: Optional[Callable] = None,
     ):
         """
+        Initializes an instance of the SearchSetup class.
+
         Parameters:
         -----------
-        image_list : list
-            A list of images to be indexed and searched.
+        item_list : List[str]
+            A list of items to be indexed and searched. The items can be any type of data (e.g., images, videos, texts, etc.).
         feature_extractor : Callable, optional
             Custom model for feature extraction (default=None).
         dim_reduction : Callable, optional
             Custom dimensionality reduction function (default=None).
-        image_count : int, optional
-            The number of images to be indexed and searched. If None, all images in the image_list will be used (default=None).
         metadata_dir : str, optional
             The directory to store metadata files (default="metadata_dir").
         feature_extractor_name : str, optional
             Name of the custom feature extractor (default="feature_extractor").
         mode : str, optional
             The mode to run the search in. Can be either "index" or "search" (default="index").
+        item_loader : Callable, optional
+            Custom function to load items from file paths. If None, the default image item loader is used (default=None).
         """
-        self.image_data = pd.DataFrame()
+        self.item_data = pd.DataFrame()
         self.model_name = feature_extractor_name
 
         self.mode = mode
 
-        self.image_list = (
-            image_list[:image_count] if image_count is not None else image_list
-        )
+        self.item_list = item_list
 
         self.feature_extractor = feature_extractor
         self.dim_reduction = dim_reduction
 
+        if item_loader is None:
+            self.item_loader = self._image_item_loader
+        else:
+            self.item_loader = item_loader
+
         # Create metadata directory
         self.metadata_dir = metadata_dir
         os.makedirs(self.metadata_dir, exist_ok=True)
 
         if self.mode == "index":
             self.run_index()
         elif self.mode == "search":
             self.load_metadata()
         else:
             raise ValueError("Invalid mode. Must be 'index' or 'search'.")
 
-    def _extract(self, img: Image.Image) -> np.ndarray:
-        """Extract features from the image."""
-        # Resize and convert the image
-        img = img.resize((224, 224))
-        img = img.convert("RGB")
+    def _image_item_loader(
+        self, image_path: str, image_size: tuple = (224, 224)
+    ) -> Image.Image:
+        """Load an image from a file path."""
+        return Image.open(image_path).resize(image_size).convert("RGB")
 
-        feature = self.feature_extractor(img)
+    def _extract(self, query_item) -> np.ndarray:
+        """
+        Extracts features from the query item using the feature extractor,
+        performs dimensionality reduction if applicable, and normalizes the feature vector.
+
+        Parameters:
+        -----------
+        query_item :
+            The query item.
+
+        Returns:
+        --------
+        feature : np.ndarray
+            The normalized feature vector.
+        """
+
+        # Extract features from the query item
+        feature = self.feature_extractor(query_item)
 
         # Normalize the feature vector
         feature = feature.flatten()
 
         # Dimensionality reduction
         if self.dim_reduction is not None:
             feature = self.dim_reduction(feature)
 
         return feature / np.linalg.norm(feature)
 
-    def _get_feature(self, image_data: List[str]) -> List[Union[np.ndarray, None]]:
-        self.image_data = image_data
+    def _get_feature(self, item_data: List[str]) -> List[Union[np.ndarray, None]]:
+        self.item_data = item_data
         features = []
-        for img_path in tqdm(self.image_data):  # Iterate through images
-            # Extract features from the image
+        for item_path in tqdm(self.item_data):  # Iterate through items
+            # Extract features from the item
             try:
-                feature = self._extract(img=Image.open(img_path))
+                feature = self._extract(self.item_loader(item_path))
                 features.append(feature)
             except Exception as e:
-                print(f"Error processing image {img_path}: {e}")
+                print(f"Error processing item {item_path}: {e}")
                 features.append(None)
                 continue
         return features
 
     def _start_feature_extraction(self) -> pd.DataFrame:
-        image_data = pd.DataFrame()
-        image_data["images_paths"] = self.image_list
-        f_data = self._get_feature(self.image_list)
-        image_data["features"] = f_data
-        image_data = image_data.dropna().reset_index(drop=True)
+        item_data = pd.DataFrame()
+        item_data["items_paths"] = self.item_list
+        f_data = self._get_feature(self.item_list)
+        item_data["features"] = f_data
+        item_data = item_data.dropna().reset_index(drop=True)
 
-        image_data.to_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        item_data.to_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
 
         print(
-            f"\033[94m Image Meta Information Saved: [os.path.join(self.metadata_dir, self.model_name, 'image_data_features.pkl')]"
+            f"\033[94m Item Meta Information Saved: {os.path.join(self.metadata_dir, self.model_name, 'item_data_features.pkl')}"
         )
-        return image_data
+        return item_data
 
-    def _start_indexing(self, image_data: pd.DataFrame) -> None:
-        self.image_data = image_data
-        d = len(image_data["features"][0])  # Length of item vector that will be indexed
+    def _start_indexing(self, item_data: pd.DataFrame) -> None:
+        self.item_data = item_data
+        d = len(item_data["features"][0])  # Length of item vector that will be indexed
         self.d = d
         index = faiss.IndexFlatL2(d)
-        features_matrix = np.vstack(image_data["features"].values).astype(np.float32)
+        features_matrix = np.vstack(item_data["features"].values).astype(np.float32)
         index.add(features_matrix)  # Add the features matrix to the index
         faiss.write_index(
-            index, image_features_vectors_idx(self.metadata_dir, self.model_name)
+            index, item_features_vectors_idx(self.metadata_dir, self.model_name)
         )
 
         print(
             "\033[94m Saved The Indexed File:"
-            + f"[os.path.join(self.metadata_dir, self.model_name, 'image_features_vectors.idx')]"
+            + f"{os.path.join(self.metadata_dir, self.model_name, 'item_features_vectors.idx')}"
         )
 
     def run_index(self) -> None:
         """
-        Indexes the images in the image_list and creates an index file for fast similarity search.
+        Indexes the items in the item_list and creates an index file for fast similarity search.
         """
         if len(os.listdir(self.metadata_dir)) == 0:
             data = self._start_feature_extraction()
             self._start_indexing(data)
         else:
             user_input = input(
                 "\033[91m Metadata and Features are already present, Do you want Extract Again? Enter yes or no: "
@@ -201,166 +260,157 @@
 
             if user_input.lower() == "yes":
                 data = self._start_feature_extraction()
                 self._start_indexing(data)
             else:
                 print("\033[93m Meta data already Present, Please Apply Search!")
                 print(os.listdir(self.metadata_dir))
-        self.image_data = pd.read_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        self.item_data = pd.read_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
-        self.f = len(self.image_data["features"][0])
+        self.f = len(self.item_data["features"][0])
 
-    def add_images_to_index(self, new_image_paths: List[str]) -> None:
+    def add_items_to_index(self, new_item_paths: List[str]) -> None:
         """
-        Adds new images to the existing index.
+        Adds new items to the existing index.
 
         Parameters:
         -----------
-        new_image_paths : list
-            A list of paths to the new images to be added to the index.
+        new_item_paths : list
+            A list of paths to the new items to be added to the index.
         """
         # Load existing metadata and index
-        self.image_data = pd.read_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        self.item_data = pd.read_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
         index = faiss.read_index(
-            image_features_vectors_idx(self.metadata_dir, self.model_name)
+            item_features_vectors_idx(self.metadata_dir, self.model_name)
         )
 
-        for new_image_path in tqdm(new_image_paths):
-            # Extract features from the new image
+        for new_item_path in tqdm(new_item_paths):
+            # Extract features from the new item
             try:
-                img = Image.open(new_image_path)
-                feature = self._extract(img)
+                query_item = self.item_loader(new_item_path)
+                feature = self._extract(query_item)
             except Exception as e:
-                print(f"\033[91m Error extracting features from the new image: {e}")
+                print(f"\033[91m Error extracting features from the new item: {e}")
                 continue
 
-            # Add the new image to the metadata
+            # Add the new item to the metadata
             new_metadata = pd.DataFrame(
-                {"images_paths": [new_image_path], "features": [feature]}
+                {"items_paths": [new_item_path], "features": [feature]}
             )
-            self.image_data = pd.concat(
-                [self.image_data, new_metadata], axis=0, ignore_index=True
+            self.item_data = pd.concat(
+                [self.item_data, new_metadata], axis=0, ignore_index=True
             )
 
-            # Add the new image to the index
+            # Add the new item to the index
             index.add(np.array([feature], dtype=np.float32))
 
         # Save the updated metadata and index
-        self.image_data.to_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        self.item_data.to_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
         faiss.write_index(
-            index, image_features_vectors_idx(self.metadata_dir, self.model_name)
+            index, item_features_vectors_idx(self.metadata_dir, self.model_name)
         )
 
-        print(f"\033[92m New images added to the index: {len(new_image_paths)}")
+        print(f"\033[92m New items added to the index: {len(new_item_paths)}")
 
     def _search_by_vector(self, v: np.ndarray, n: int) -> Dict[int, str]:
         index = faiss.read_index(
-            image_features_vectors_idx(self.metadata_dir, self.model_name)
+            item_features_vectors_idx(self.metadata_dir, self.model_name)
         )
         D, I = index.search(np.array([v], dtype=np.float32), n)
-        return dict(zip(I[0], self.image_data.iloc[I[0]]["images_paths"].to_list()))
-
-    def _get_query_vector(self, image_path: str) -> np.ndarray:
-        img = Image.open(image_path)
-        query_vector = self._extract(img)
-        return query_vector
-
-    def get_similar_images(
-        self, image_path: str, number_of_images: int = 10
-    ) -> Dict[int, str]:
-        """
-        Returns the most similar images to a given query image according to the indexed image features.
-
-        Parameters:
-        -----------
-        image_path : str
-            The path to the query image.
-        number_of_images : int, optional (default=10)
-            The number of most similar images to the query image to be returned.
-        """
-        query_vector = self._get_query_vector(image_path)
-        img_dict = self._search_by_vector(query_vector, number_of_images)
-        return img_dict
-
-    def get_similar_images_list(
-        self, image_path: str, number_of_images: int = 10
-    ) -> List[str]:
-        """
-        Returns the most similar images to a given query image according to the indexed image features.
+        return dict(zip(I[0], self.item_data.iloc[I[0]]["items_paths"].to_list()))
 
-        Parameters:
-        -----------
-        image_path : str
-            The path to the query image.
-        number_of_images : int, optional (default=10)
-            The number of most similar images to the query image to be returned.
-        """
-        img_dict = self.get_similar_images(image_path, number_of_images)
-        similar_n_images =  list(img_dict.values())
-        similar_n_images_names = [os.path.basename(image_path) for image_path in similar_n_images]
-        return similar_n_images_names
-
-    def get_image_metadata_file(self) -> pd.DataFrame:
+    def get_item_metadata_file(self) -> pd.DataFrame:
         """
-        Returns the metadata file containing information about the indexed images.
+        Returns the metadata file containing information about the indexed items.
 
         Returns:
         --------
         DataFrame
             The Panda DataFrame of the metadata file.
         """
-        image_data = pd.read_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        item_data = pd.read_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
-        return image_data
+        return item_data
 
     def load_metadata(self):
         """Loads the metadata and index for search mode."""
-        self.image_data = pd.read_pickle(
-            image_data_with_features_pkl(self.metadata_dir, self.model_name)
+        self.item_data = pd.read_pickle(
+            item_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
-        self.f = len(self.image_data["features"][0])
-
+        self.f = len(self.item_data["features"][0])
 
-    def _get_query_vector_from_image(self, image: Image) -> np.ndarray:
-        query_vector = self._extract(image)
+    def _get_query_vector(self, item) -> np.ndarray:
+        query_vector = self._extract(item)
         return query_vector
-    
-    def get_similar_images_from_image(
-        self, image: Image, number_of_images: int = 10
-    ) -> Dict[int, str]:
-        """
-        Returns the most similar images to a given query image according to the indexed image features.
 
-        Parameters:
-        -----------
-        image : Image
-            The query image.
-        number_of_images : int, optional (default=10)
-            The number of most similar images to the query image to be returned.
-        """
-        query_vector = self._get_query_vector_from_image(image)
-        img_dict = self._search_by_vector(query_vector, number_of_images)
-        return img_dict
-    
-    def get_similar_images_list_from_image(
-        self, image: Image, number_of_images: int = 10
-    ) -> List[str]:
-        """
-        Returns the most similar images to a given query image according to the indexed image features.
+    def get_similar_items(
+        self,
+        item: Union[str, Any],
+        number_of_items: int = 10,
+        return_paths: bool = True,
+    ) -> Union[List[str], Dict[int, str]]:
+        """
+        Given a query item or the path to a query item, this method returns the most
+        similar items according to the indexed features. The item can be any type
+        of item (e.g., image, video, text, etc.) as long as it is compatible with
+        the feature extraction and indexing methods used in the class.
 
         Parameters:
         -----------
-        image : Image
-            The query image.
-        number_of_images : int, optional (default=10)
-            The number of most similar images to the query image to be returned.
-        """
-        img_dict = self.get_similar_images_from_image(image, number_of_images)
-        similar_n_images =  list(img_dict.values())
-        similar_n_images_names = [os.path.basename(image_path) for image_path in similar_n_images]
-        return similar_n_images_names
+        item : Union[str, Any]
+            The query item or the path to the query item. If a string is provided,
+            it is assumed to be a path to a file. If a non-string item is provided,
+            it is assumed to be the query item itself. The item can be any type of
+            item (e.g., image, video, text, etc.) as long as it is compatible with
+            the feature extraction and indexing methods used in the class.
+        number_of_items : int, optional (default=10)
+            The number of most similar items to the query item to be returned. The
+            method will return up to this number of items, depending on the
+            availability of similar items in the index.
+        return_paths : bool, optional (default=True)
+            If True, return a list of paths to the most similar items.
+            If False, return a dictionary mapping indices to paths of the most
+            similar items. The indices are based on the order of the items in the
+            index and can be used to reference specific items.
+
+        Returns:
+        --------
+        Union[List[str], Dict[int, str]]
+            The most similar items to the query item, either as a list of paths or
+            as a dictionary mapping indices to paths. The paths represent the
+            location of the similar items in the file system. If the original items
+            are not stored as files, these paths can be used as identifiers or
+            references to the items in a custom storage system.
+
+        Raises:
+        -------
+        ValueError
+            If the provided item is a string but not a valid file path, a ValueError
+            is raised with a message indicating that the item is not a valid file path.
+        """
+        # We first load the item
+        if isinstance(
+            item, str
+        ):  # If the item is a string, we assume it is a path to a file
+            if os.path.isfile(item):
+                item = self.item_loader(item)
+            else:
+                raise ValueError(f"Item {item} is not a valid file path.")
+
+        # We then extract the features from the item
+        query_vector = self._get_query_vector(item)
+
+        # We then search for the most similar items
+        item_dict = self._search_by_vector(query_vector, number_of_items)
+
+        # Now we return items according to the return_paths parameter
+        if return_paths:
+            return list(item_dict.values())
+
+        else:
+            return item_dict
```

### Comparing `DeepSearchLite-0.1.1/LICENSE` & `DeepSearchLite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.1.1/setup.py` & `DeepSearchLite-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DeepSearchLite",
-    version="0.1.1",
+    version="0.2.0",
     author="Ibad Rather",
     author_email="ibad.rather.ir@gmail.com",
     description="A package for image similarity search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibadrather/DeepSearchLite",
     packages=find_packages(),
@@ -19,15 +19,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires='>=3.8',
+    python_requires=">=3.8",
     install_requires=[
         "numpy",
         "pandas",
         "Pillow",
         "faiss-cpu",
         "tqdm",
     ],
```

