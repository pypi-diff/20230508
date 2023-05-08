# Comparing `tmp/dreimac-0.1.tar.gz` & `tmp/dreimac-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dreimac-0.1.tar", last modified: Mon Jan  9 16:53:24 2023, max compression
+gzip compressed data, was "dreimac-0.2.0.tar", last modified: Mon May  8 16:30:17 2023, max compression
```

## Comparing `dreimac-0.1.tar` & `dreimac-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:53:24.000000 dreimac-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-01-09 16:53:24.000000 dreimac-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-01-09 16:52:26.000000 dreimac-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/circularcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/emcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/projectivecoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    15662 2023-01-09 16:52:26.000000 dreimac-0.1/dreimac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-09 16:53:24.000000 dreimac-0.1/dreimac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 16:53:24.000000 dreimac-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-09 16:52:26.000000 dreimac-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 16:53:24.000000 dreimac-0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-09 16:52:26.000000 dreimac-0.1/test/test_circular.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-09 16:52:26.000000 dreimac-0.1/test/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-09 16:52:26.000000 dreimac-0.1/test/test_projective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-05-08 16:28:38.000000 dreimac-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.384883 dreimac-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-08 16:28:38.000000 dreimac-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/circularcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/combinatorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/emcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/projectivecoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/toroidalcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:30:17.384883 dreimac-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-08 16:28:38.000000 dreimac-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_circular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_combinatorial_number_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_projective.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dreimac-0.1/dreimac/circularcoords.py` & `dreimac-0.2.0/dreimac/projectivecoords.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,160 @@
 import numpy as np
-import scipy
-from scipy.sparse.linalg import lsqr
-from .utils import *
-from .emcoords import *
-
-
-"""#########################################
-        Main Circular Coordinates Class
-#########################################"""
-
-class CircularCoords(EMCoords):
-    def __init__(self, X, n_landmarks, distance_matrix=False, prime=41, maxdim=1, verbose=False):
-        """
-        Parameters
-        ----------
-        X: ndarray(N, d)
-            A point cloud with N points in d dimensions
-        n_landmarks: int
-            Number of landmarks to use
-        distance_matrix: boolean
-            If true, treat X as a distance matrix instead of a point cloud
-        prime : int
-            Field coefficient with which to compute rips on landmarks
-        maxdim : int
-            Maximum dimension of homology.  Only dimension 1 is needed for circular coordinates,
-            but it may be of interest to see other dimensions (e.g. for a torus)
+import time
+from .utils import PartUnity
+from .emcoords import EMCoords
+
+
+class ProjectiveCoords(EMCoords):
+    """
+    Object that performs multiscale real projective coordinates via
+    persistent cohomology of sparse filtrations (Jose Perea 2018).
+
+    Parameters
+    ----------
+    X: ndarray(N, d)
+        A point cloud with N points in d dimensions
+    n_landmarks: int
+        Number of landmarks to use
+    distance_matrix: boolean
+        If true, treat X as a distance matrix instead of a point cloud
+    maxdim : int
+        Maximum dimension of homology. Only dimension 1 is needed for circular coordinates,
+        but it may be of interest to see other dimensions (e.g. for a torus)
+    partunity_fn: ndarray(n_landmarks, N) -> ndarray(n_landmarks, N)
+        A partition of unity function
+
+    """
+
+    def __init__(self, X, n_landmarks, distance_matrix=False, maxdim=1, verbose=False):
+        EMCoords.__init__(
+            self,
+            X=X,
+            n_landmarks=n_landmarks,
+            distance_matrix=distance_matrix,
+            prime=2,
+            maxdim=maxdim,
+            verbose=verbose,
+        )
+        self.type_ = "proj"
+        # GUI variables
+        self.selected = set([])
+        self.u = np.array([0, 0, 1])
+
+    def get_coordinates(
+        self,
+        perc=0.9,
+        cocycle_idx=0,
+        proj_dim=2,
+        partunity_fn=PartUnity.linear,
+        standard_range=True,
+    ):
         """
-        EMCoords.__init__(self, X=X, n_landmarks=n_landmarks, distance_matrix=distance_matrix, prime=prime, maxdim=maxdim, verbose=verbose)
-        self.type_ = "circ"
+        Get real projective coordinates.
 
-    def get_cocycle_projection(self, cocycle, r_cover, do_weighted):
-        """
-        Setup coboundary matrix, delta_0, for Cech_{r_cover }
-        and use it to find a projection of the cocycle
-        onto the image of delta0
-        
-        Parameters
-        ----------
-        cocycle: ndarray(K, 3, dtype=int)
-            Representative cocycle.  First two columns are vertex indices,
-            and third column is value in field of prime self.prime_
-        r_cover: float
-            Covering radius
-        do_weighted : boolean
-            Whether to make a weighted cocycle on the representatives
-        
-        Returns
-        -------
-        tau: ndarray(n_landmarks)
-            Scalar function on the landmarks whose image under delta0 best matches cocycle
-        theta: ndarray(n_edges)
-            The image of tau under delta0
-        """
-        prime = self.prime_
-        n_landmarks = self.n_landmarks_
-        dist_land_land = self.dist_land_land_
-        #Lift to integer cocycle
-        val = np.array(cocycle[:, 2])
-        val[val > (prime-1)/2] -= prime
-        Y = np.zeros((n_landmarks, n_landmarks))
-        Y[cocycle[:, 0], cocycle[:, 1]] = val
-        Y = Y + Y.T
-        #Select edges that are under the threshold
-        [I, J] = np.meshgrid(np.arange(n_landmarks), np.arange(n_landmarks))
-        I = I[np.triu_indices(n_landmarks, 1)]
-        J = J[np.triu_indices(n_landmarks, 1)]
-        Y = Y[np.triu_indices(n_landmarks, 1)]
-        idx = np.arange(len(I))
-        idx = idx[dist_land_land[I, J] < 2*r_cover]
-        I = I[idx]
-        J = J[idx]
-        Y = Y[idx]
-
-        NEdges = len(I)
-        R = np.zeros((NEdges, 2))
-        R[:, 0] = J
-        R[:, 1] = I
-        #Make a flat array of NEdges weights parallel to the rows of R
-        if do_weighted:
-            W = dist_land_land[I, J]
-        else:
-            W = np.ones(NEdges)
-        delta0 = make_delta0(R)
-        wSqrt = np.sqrt(W).flatten()
-        WSqrt = scipy.sparse.spdiags(wSqrt, 0, len(W), len(W))
-        A = WSqrt*delta0
-        b = WSqrt.dot(Y)
-        tau = lsqr(A, b)[0]
-        theta = np.zeros((NEdges, 3))
-        theta[:, 0] = J
-        theta[:, 1] = I
-        theta[:, 2] = -delta0.dot(tau)
-        theta = add_cocycles(cocycle, theta, real=True)
-        return tau, theta
-
-    def get_coordinates(self, perc = 0.99, do_weighted = False, cocycle_idx = [0], partunity_fn = PartUnity.linear):
-        """
-        Perform circular coordinates via persistent cohomology of 
-        sparse filtrations (Jose Perea 2018)
         Parameters
         ----------
         perc : float
-            Percent coverage
-        do_weighted : boolean
-            Whether to make a weighted cocycle on the representatives
+            Percent coverage. Must be between 0 and 1.
         cocycle_idx : list
-            Add the cocycles together at the indices in this list
+            Add the cocycles together, sorted from most to least persistent
+        proj_dim : integer
+            Dimension down to which to project the data
         partunity_fn: (dist_land_data, r_cover) -> phi
             A function from the distances of each landmark to a bump function
-        
+        standard_range : bool
+            Whether to use the parameter perc to choose a filtration parameter that guarantees
+            that the selected cohomology class represents a class in the Cech complex.
+
         Returns
         -------
-        thetas: ndarray(N)
-            Circular coordinates
+        {'variance': ndarray(N-1)
+            The variance captured by each dimension
+        'X': ndarray(N, proj_dim+1)
+            The projective coordinates
+        }
+
         """
         n_landmarks = self.n_landmarks_
         n_data = self.X_.shape[0]
         ## Step 1: Come up with the representative cocycle as a formal sum
         ## of the chosen cocycles
-        cohomdeath, cohombirth, cocycle = EMCoords.get_rep_cocycle(self, cocycle_idx)
-        
+        homological_dimension = 1
+        cohomdeath_rips, cohombirth_rips, cocycle = self.get_representative_cocycle(
+            cocycle_idx, homological_dimension
+        )
 
         ## Step 2: Determine radius for balls
-        r_cover = EMCoords.get_cover_radius(self, perc, cohomdeath, cohombirth)
-        
+        r_cover, _ = EMCoords.get_cover_radius(
+            self, perc, cohomdeath_rips, cohombirth_rips, standard_range
+        )
 
-        ## Step 3: Setup coboundary matrix, delta_0, for Cech_{r_cover }
-        ## and use it to find a projection of the cocycle
-        ## onto the image of delta0
-        tau, theta = self.get_cocycle_projection(cocycle, r_cover, do_weighted)
-        
-
-        ## Step 4: Create the open covering U = {U_1,..., U_{s+1}} and partition of unity
+        ## Step 3: Create the open covering U = {U_1,..., U_{s+1}} and partition of unity
         varphi, ball_indx = EMCoords.get_covering_partition(self, r_cover, partunity_fn)
 
-        ## Step 5: From U_1 to U_{s+1} - (U_1 \cup ... \cup U_s), apply classifying map
+        ## Step 4: From U_1 to U_{s+1} - (U_1 \cup ... \cup U_s), apply classifying map
         # compute all transition functions
-        theta_matrix = np.zeros((n_landmarks, n_landmarks))
-        I = np.array(theta[:, 0], dtype = np.int64)
-        J = np.array(theta[:, 1], dtype = np.int64)
-        theta = theta[:, 2]
-        theta = np.mod(theta + 0.5, 1) - 0.5
-        theta_matrix[I, J] = theta
-        theta_matrix[J, I] = -theta
-        class_map = -tau[ball_indx]
+        cocycle_matrix = np.ones((n_landmarks, n_landmarks))
+        cocycle_matrix[cocycle[:, 0], cocycle[:, 1]] = -1
+        cocycle_matrix[cocycle[:, 1], cocycle[:, 0]] = -1
+        class_map = np.sqrt(varphi.T)
         for i in range(n_data):
-            class_map[i] += theta_matrix[ball_indx[i], :].dot(varphi[:, i])    
-        thetas = np.mod(2*np.pi*class_map, 2*np.pi)
-
-        return thetas
+            class_map[i, :] *= cocycle_matrix[ball_indx[i], :]
+        res = _ppca(class_map, proj_dim, self.verbose)
+        return res
+
+
+def _ppca(class_map, proj_dim, verbose=False):
+    """
+    Principal Projective Component Analysis (Jose Perea 2017)
+
+    Parameters
+    ----------
+    class_map : ndarray (N, d)
+        For all N points of the dataset, membership weights to
+        d different classes are the coordinates
+    proj_dim : integer
+        The dimension of the projective space onto which to project
+    verbose : boolean
+        Whether to print information during iterations
+
+    Returns
+    -------
+    {'variance': ndarray(N-1)
+        The variance captured by each dimension
+    'X': ndarray(N, proj_dim+1)
+        The projective coordinates
+    }
+
+    """
+    if verbose:
+        print(
+            "Doing ppca on %i points in %i dimensions down to %i dimensions"
+            % (class_map.shape[0], class_map.shape[1], proj_dim)
+        )
+    X = class_map.T
+    variance = np.zeros(X.shape[0] - 1)
+
+    n_dim = class_map.shape[1]
+    tic = time.time()
+    # Projective dimensionality reduction : Main Loop
+    XRet = None
+    for i in range(n_dim - 1):
+        # Project onto an "equator"
+        try:
+            _, U = np.linalg.eigh(X.dot(X.T))
+            U = np.fliplr(U)
+        except:
+            U = np.eye(X.shape[0])
+        variance[-i - 1] = np.mean(
+            (np.pi / 2 - np.real(np.arccos(np.abs(U[:, -1][None, :].dot(X))))) ** 2
+        )
+        Y = (U.T).dot(X)
+        y = np.array(Y[-1, :])
+        Y = Y[0:-1, :]
+        X = Y / np.sqrt(1 - np.abs(y) ** 2)[None, :]
+        if i == n_dim - proj_dim - 2:
+            XRet = np.array(X)
+    if verbose:
+        print("Elapsed time ppca: %.3g" % (time.time() - tic))
+    # Return the variance and the projective coordinates
+    return {"variance": variance, "X": XRet.T}
```

### Comparing `dreimac-0.1/setup.py` & `dreimac-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,53 @@
-import sys
-import os
-import platform
-
 from setuptools import setup
 
 ## Get version information from _version.py
 import re
-VERSIONFILE="dreimac/_version.py"
+
+VERSIONFILE = "dreimac/_version.py"
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
-# Use README.md as the package long description  
-with open('README.md') as f:
+# Use README.md as the package long description
+with open("README.md") as f:
     long_description = f.read()
 
 
+# get requirements
+def requirements():
+    with open("requirements.txt") as f:
+        return [line.strip() for line in f if line.strip()]
+
+
 setup(
     name="dreimac",
     version=verstr,
-    description="Dimension reduction with Eilenberg-MacClane coordinates",
+    description="DREiMac: Dimension reduction with Eilenberg-MacLane coordinates",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author="Chris Tralie, Jose Perea, Luis Scoccola",
+    author="Jose A. Perea, Luis Scoccola, Chris Tralie",
     author_email="ctralie@alumni.princeton.edu",
-    license='Apache2',
-    packages=['dreimac'],
-    setup_requires=[
-        'cython', 'numpy'
-    ],
-    install_requires=[
-        'cython', 'numpy', 'scipy', 'matplotlib', 'numba', 'persim', 'ripser'
-    ],
+    license="Apache2",
+    packages=["dreimac"],
+    install_requires=requirements(),
     extras_require={
-        'testing': [ # `pip install -e ".[testing]"``
-            'pytest'  
-        ],
-        'docs': [ # `pip install -e ".[docs]"`
-            'sktda_docs_config'
-        ],
-        'examples': []
+        "testing": ["pytest"],
+        "examples": [],
     },
-    python_requires='>=3.6',
+    python_requires=">=3.8, <3.10",
     classifiers=[
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Education',
-        'Intended Audience :: Financial and Insurance Industry',
-        'Intended Audience :: Healthcare Industry',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Topic :: Scientific/Engineering :: Mathematics',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Education",
+        "Intended Audience :: Financial and Insurance Industry",
+        "Intended Audience :: Healthcare Industry",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Mathematics",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
-    keywords='topological data analysis, dimension reduction'
+    keywords="topological data analysis, dimension reduction",
 )
```

