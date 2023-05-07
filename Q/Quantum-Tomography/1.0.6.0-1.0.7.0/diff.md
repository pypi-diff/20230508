# Comparing `tmp/Quantum-Tomography-1.0.6.0.tar.gz` & `tmp/Quantum-Tomography-1.0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quantum-Tomography-1.0.6.0.tar", last modified: Tue Apr 11 23:54:10 2023, max compression
+gzip compressed data, was "Quantum-Tomography-1.0.7.0.tar", last modified: Sun May  7 22:40:09 2023, max compression
```

## Comparing `Quantum-Tomography-1.0.6.0.tar` & `Quantum-Tomography-1.0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.709207 Quantum-Tomography-1.0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/src/QuantumTomography/
--rw-r--r--   0 runner    (1001) docker     (123)    75121 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19099 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClassHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplayHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctionsHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-04-11 23:48:29.000000 Quantum-Tomography-1.0.6.0/src/QuantumTomography/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:54:10.713207 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 23:54:10.000000 Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:40:09.951093 Quantum-Tomography-1.0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-07 22:40:09.951093 Quantum-Tomography-1.0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 22:40:09.951093 Quantum-Tomography-1.0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:40:09.943093 Quantum-Tomography-1.0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:40:09.947093 Quantum-Tomography-1.0.7.0/src/QuantumTomography/
+-rw-r--r--   0 runner    (1001) docker     (123)    74816 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoClassHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoDisplayHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoFunctionsHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-07 22:34:25.000000 Quantum-Tomography-1.0.7.0/src/QuantumTomography/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 22:40:09.951093 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 22:40:09.000000 Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/top_level.txt
```

### Comparing `Quantum-Tomography-1.0.6.0/LICENSE` & `Quantum-Tomography-1.0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/PKG-INFO` & `Quantum-Tomography-1.0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quantum-Tomography
-Version: 1.0.6.0
+Version: 1.0.7.0
 Summary: A python library to help perform tomography on a quantum state.
 Home-page: https://github.com/KwiatQIM/Quantum-Tomography
 Author: University of Illinois
 Author-email: turroscott@gmail.com
 License: MIT
 Project-URL: Documentation, https://quantumtomo.web.illinois.edu/Doc/
 Project-URL: Video Tutorial, https://www.youtube.com/watch?v=I-214P0LOfQ&list=PLJLHMKtk5Pqy9w9aCuyowUF1p7pl2JCI9&index=3
```

### Comparing `Quantum-Tomography-1.0.6.0/README.md` & `Quantum-Tomography-1.0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/setup.py` & `Quantum-Tomography-1.0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open('README.md') as f:
         README  = f.read()
     return README
 
 
 setup(
     name = "Quantum-Tomography",
-    version = "1.0.6.0",
+    version = "1.0.7.0",
     description = "A python library to help perform tomography on a quantum state.",
     long_description = readme(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/KwiatQIM/Quantum-Tomography",
     author = "University of Illinois",
     author_email = "turroscott@gmail.com",
     license = "MIT",
```

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClass.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,24 +259,22 @@
         self.conf['Method'] = method
         [coincidences, measurements_densities, measurements_pures, accidentals,overall_norms] = self.filter_data(tomo_input)
 
         # get the starting state from tomography_LINEAR if not defined
         starting_matrix = self.conf['RhoStart']
         if method.upper() == "LINEAR" or not isinstance(starting_matrix,np.ndarray):
             try:
-                # todo: go over linear tomography. Clean it up. Figure out why it fails on the very rare occasion.
                 [starting_matrix,inten_linear] = self.tomography_LINEAR(coincidences, measurements_pures,overall_norms)
                 # Currently linear tomography gets the phase wrong. So a temporary fix is to just transpose it.
                 starting_matrix = starting_matrix.transpose()
                 starting_matrix = make_positive(starting_matrix)
                 starting_matrix = starting_matrix / np.trace(starting_matrix)
             except:
                 raise RuntimeError('Failed to run linear Tomography')
 
-
         # Run tomography and find an estimate for the state
         if method == "MLE":
             [rhog, intensity, fvalp] = self.tomography_MLE(starting_matrix, coincidences, measurements_densities, accidentals,overall_norms)
         elif method.upper() == "HMLE":
             [rhog, intensity, fvalp] = self.tomography_HMLE(starting_matrix, coincidences, measurements_densities,
                                                            accidentals, overall_norms)
         # elif method.upper() == "BME":
@@ -724,48 +722,39 @@
     Returns
     -------
     rhog : ndarray with shape = (2^numQubits, 2^numQubits)
         The starting predicted state.
     intensity : float
         The predicted overall intensity used to normalize the state.
     """
-    def tomography_LINEAR(self, coincidences, measurements, overall_norms=-1,m_set = ()):
+
+    def tomography_LINEAR(self, coincidences, measurements, overall_norms=-1):
         # If overall_norms not given then assume uniform
         if not isinstance(overall_norms,np.ndarray):
             overall_norms = np.ones(coincidences.shape[0])
         elif not (len(overall_norms.shape) == 1 and overall_norms.shape[0] == coincidences.shape[0]):
             raise ValueError("Invalid intensities array")
 
-        if m_set == ():
-            m_set = independent_set(measurements)
-        if np.isscalar(m_set):
-            n = len(coincidences)
-            linear_measurements = measurements
-            linear_data = coincidences
-        else:
-            n = int(np.sum(m_set))
-            linear_measurements = measurements[(np.rot90(m_set == 1.0)[0])]
-            linear_data = coincidences[(np.rot90(m_set == 1.0)[0])]
-
-        linear_rhog = np.zeros([measurements.shape[1], measurements.shape[1]])
-
-        b = b_matrix(linear_measurements)
-        b_inv = np.linalg.inv(b)
-
-        m = np.zeros([measurements.shape[1], measurements.shape[1], n]) + 0j
-        for j in range(n):
-            m[:, :, j] = m_matrix(j, linear_measurements, b_inv)
-            linear_rhog = linear_rhog + linear_data[j] * m[:, :, j]
+        coincidences = coincidences.flatten()
+
+        pauli_basis = generalized_pauli_basis(self.getNumQubits())
+        stokes_measurements = np.array([get_stokes_parameters(m,pauli_basis) for m in measurements]) / 2**self.getNumQubits()
+        freq_array = coincidences / overall_norms
+
+        B_inv = np.linalg.inv(np.matmul(stokes_measurements.T,stokes_measurements))
+        stokes_params = np.matmul(stokes_measurements.T,freq_array)
+        stokes_params = np.matmul(B_inv,stokes_params)
+        linear_rhog = np.multiply(pauli_basis,stokes_params[:, np.newaxis,np.newaxis])
+        linear_rhog = np.sum(linear_rhog,axis=0)
 
         intensity = np.trace(linear_rhog)
         rhog = linear_rhog / intensity
 
         return [rhog, intensity]
 
-
     """
     filter_data(tomo_input)
     Desc: Filters the data into separate arrays.
 
     Parameters
     ----------
     tomo_input : ndarray
```

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoClassHelpers.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoClassHelpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -84,158 +84,24 @@
     for j in range(len(prediction)):
         prediction[j] = overall_norms[j] * np.real(np.trace(np.dot(measurements[j,:,:], rhog))) + accidentals[j]
         prediction[j] = np.max([prediction[j], 0.01])
     hedge = np.repeat(np.real((bet * np.log(np.linalg.det(rhog))) / len(prediction)), len(prediction))
     val = np.sqrt(np.real((((prediction - coincidences) ** 2) / (2 * prediction)) - hedge) + 1000)
     return np.real(val)
 
-# This are some old functions that have since been reworked.
-#
-# """
-# maxlike_fitness_old(t, coincidences, accidentals, m, prediction)
-# Desc: Calculates the diffrence between the current predicted state data and the actual data
-#
-# Parameters
-# ----------
-# t : ndarray
-#     T values of the current predicted state.
-# coincidences : ndarray with length = number of measurements or shape = (number of measurements, 2^numQubits) for 2 det/qubit
-#     The counts of the tomography.
-# accidentals : ndarray with length = number of measurements or shape = (number of measurements, 2^numQubits) for 2 det/qubit
-#     The singles values of the tomography. Used for accidental correction.
-# m : ndarray with shape = (2^numQubits, 2^numQubits, number of measurements)
-#     The measurements of the tomography in density matrix form.
-# prediction : ndarray
-#     Predicted counts from the predicted state.
-# overall_norms : 1darray with length = number of measurements or length = number of measurements * 2^numQubits for 2 det/qubit
-#     The relative weights of each measurment. Used for drift correction.
-#
-# Returns
-# -------
-# val : float
-#     value of the optimization function.
-# """
-# def maxlike_fitness_old(t, coincidences, accidentals, m, prediction,overall_norms=-1):
-#     rhog = t_to_density(t,normalize=False)
-#     for j in range(len(prediction)):
-#         prediction[j] = np.float64(np.real(overall_norms[j] * np.real(np.trace(np.dot(m[:, :, j], rhog))) + accidentals[j]))
-#         prediction[j] = np.max([prediction[j], 0.01])
-#     val = (prediction - coincidences) / np.sqrt(prediction)
-#     val = np.float64(np.real(val))
-#     return val
-#
-#
-# """
-# maxlike_fitness_hedged_old(t, coincidences, accidentals, m, prediction, bet)
-# Desc: Calculates the diffrence between the current predicted state data and the actual data using hedged maximum likelihood.
-#
-# Parameters
-# ----------
-# t : ndarray
-#     T values of the current predicted state.
-# coincidences : ndarray with length = number of measurements or shape = (number of measurements, 2^numQubits) for 2 det/qubit
-#     The counts of the tomography.
-# accidentals : ndarray with length = number of measurements or shape = (number of measurements, 2^numQubits) for 2 det/qubit
-#     The singles values of the tomography. Used for accidental correction.
-# m : ndarray with shape = (2^numQubits, 2^numQubits, number of measurements)
-#     The measurements of the tomography in density matrix form .
-# prediction : ndarray
-#     Predicted counts from the predicted state.
-# bet : float 0 to .5
-#     The beta value used.
-# overall_norms : 1darray with length = number of measurements or length = number of measurements * 2^numQubits for 2 det/qubit
-#     The relative weights of each measurment. Used for drift correction.
-#
-# Returns
-# -------
-# val : float
-#     value of the optimization function.
-# """
-# def maxlike_fitness_hedged_old(t, coincidences, accidentals, m, prediction, bet,overall_norms=-1):
-#     # If overall_norms not given then assume uniform
-#     if not isinstance(overall_norms,np.ndarray):
-#         overall_norms = np.ones(coincidences.shape[0])
-#     elif not (len(overall_norms.shape) == 1 and overall_norms.shape[0] == coincidences.shape[0]):
-#         raise ValueError("Invalid intensities array")
-#
-#     rhog = t_to_density(t,normalize=False)
-#     for j in range(len(prediction)):
-#         prediction[j] = overall_norms[j] * np.real(np.trace(np.dot(m[:, :, j], rhog))) + accidentals[j]
-#         prediction[j] = np.max([prediction[j], 0.01])
-#
-#     hedge = np.repeat(np.real((bet * np.log(np.linalg.det(np.mat(rhog)))) / len(prediction)), len(prediction))
-#     val = np.sqrt(np.real((((prediction - coincidences) ** 2) / (2 * prediction)) - hedge) + 1000)
-#
-#     val = np.float64(np.real(val))
-#
-#     return val
-
-# helper function used in linear tomography
-def independent_set(measurements):
-    m = measurements[0, :].conj().transpose()
-    # may have to switched order of m and measurements, may be wrong but has little effect
-    matrix = rho2stokes(np.outer(m, measurements[0, :]))
-    max_rank = matrix.shape[0]
-
-    if (measurements.shape[0]) == max_rank:
-        s = np.ones([measurements.shape[0], 1])
-        return s
-
-    s = np.zeros([measurements.shape[0], 1])
-    s[0] = 1
-    cur_rank = 1
-    for j in np.arange(1, measurements.shape[0], 1):
-    # may have to switched order of m and measurements, may be wrong but has little effect
-        m = measurements[j, :].conj().transpose()
-        sv = rho2stokes(np.outer(m, measurements[j, :]))
-        if (np.linalg.matrix_rank(np.concatenate((matrix, sv), axis = 1), tol = 0.001)) > cur_rank:
-            matrix = np.concatenate((matrix, sv), axis = 1)
-            cur_rank += 1
-            s[j] = 1
-        else:
-            s[j] = 0
-        if cur_rank == max_rank:
-            break
-    return s
-
 # This function converts a list of loglikelihoods to normalized likelihoods. Also returns the index of
 # the min loglike
 def normalizeLikelihoods(likelihoods):
     nIndex = np.argmin(likelihoods)
     nFactor = likelihoods[nIndex]
     scaled = likelihoods - nFactor
     likelihoods = np.exp(-1 * scaled)
     likelihoods = likelihoods/sum(likelihoods)
     return likelihoods, nIndex,scaled
 
-
-# helper function that formats the projects into a single matrix
-def b_matrix(projectors):
-    dim_m = projectors.shape[1]
-    dim_b = dim_m**2
-    tmp = np.zeros([dim_b, dim_b])+0j
-    for i in range(dim_b):
-        for j in range(dim_b):
-            tmp[i][j] = np.inner(projectors[i], np.inner(sigma_n(j, dim_m), projectors[i].conj().transpose()))
-    b = tmp.transpose()
-    return b
-
-
-# helper function that formats the measurements into a single matrix
-def m_matrix(mu, projectors, b_inv):
-    dim_m = projectors.shape[1]
-    dim_b = dim_m**2
-
-    tmp = np.zeros([dim_m, dim_m])
-    for j in range(dim_b):
-        tmp = tmp + b_inv[mu][j]*sigma_n(j, dim_m)
-    m = tmp
-
-    return m
-
 # # Helper function for looping through a multi indexed array
 # def multiloop_index(j, lengths):
 #     ind = np.zeros(len(lengths))
 #     for k in range(len(lengths)-1):
 #         sz = np.prod(lengths[np.arange(k+1, len(lengths))])
 #         ind[k] = np.fix(j/sz)+1
 #         j % = sz
@@ -247,55 +113,14 @@
     d, v = np.linalg.eig(rhog_in)
     rhog = np.zeros(rhog_in.shape)
     for j in range(len(d)):
         rhog = rhog + np.abs(d[j])*np.outer(v[:, j], v[:, j].conj().transpose())
     rhog = (rhog + rhog.conj().transpose())/2.0
     return rhog
 
-# helper function for re formatting matrices
-def sigma_n(j, nn):
-    if j < 0 or j > nn**2-1:
-        print('sigma_N: j out of range for SU(N)')
-
-    m = int(np.fix(j/nn))
-    n = int(j % nn)
-    tmp1 = np.zeros([nn, 1])
-    tmp2 = np.zeros([nn, 1])
-    tmp1[m] = 1
-    tmp2[n] = 1
-
-    if m < n:
-        matrix = (np.outer(tmp1, tmp2.conj().transpose())+np.outer(tmp2, tmp1.conj().transpose()))*np.sqrt(nn/2.0)
-    elif m > n:
-        matrix = 1j*(np.outer(tmp1, tmp2.conj().transpose())-np.outer(tmp2, tmp1.conj().transpose()))*np.sqrt(nn/2.0)
-    elif (m+1) < nn:
-        z = np.zeros(nn)
-        for i in range(m+1):
-            z[i] = 1
-        matrix = -(np.sqrt(nn/((m+1.0)**2+m+1.0)))*np.diag(z)
-        matrix[m+1, m+1] = (m+1.0)*(np.sqrt(nn/((m+1.0)**2+m+1.0)))
-    else:  # n = m = N
-        matrix = np.identity(nn)
-
-    return matrix
-
-# Helper function for independent_set function
-def rho2stokes(rhog):
-    if rhog.ndim == 1:
-        rhog = np.outer(rhog, rhog.conj().transpose())
-
-    d = len(rhog)
-    n = d**2
-
-    ss = np.zeros([n, 1])+0j
-    for j in range(n):
-        ss[j] = np.trace(np.inner(rhog, sigma_n(j, d)))
-
-    return ss
-
 # Helper function for calculating the bell settings
 def coinmat(a, b):
     k = np.array([np.cos(a)*np.cos(b), np.cos(a)*np.sin(b), np.sin(a)*np.cos(b), np.sin(a)*np.sin(b)])
     cmat = np.outer(k, k)
 
     return cmat
```

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplay.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoDisplay.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoDisplayHelpers.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoDisplayHelpers.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctions.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoFunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,14 +129,64 @@
     """
 def toDensity(psiMat):
     if not isStateVector(psiMat):
         raise ValueError("Invalid input state with shape " + str(psiMat.shape))
     psiMat = np.outer(psiMat, psiMat.conj())
     return psiMat / np.trace(psiMat)
 
+pauli_matrices = np.array([[[1,0],[0,1]],
+                           [[0,1],[1,0]],
+                           [[0,-1j],[1j,0]],
+                           [[1,0],[0,-1]],],dtype=complex)
+"""
+generalized_pauli_basis(num_qubits)
+Desc: Returns a set of pauli matrices.
+
+Parameters
+----------
+num_qubits : int
+    Number of qubits to define the dimensionality of the basis.
+
+Returns
+-------
+basis : ndarray with shape = (4^numQubits, 2^numQubits, 2^numQubits)
+    Pauli Basis
+    """
+def generalized_pauli_basis(num_qubits):
+    if num_qubits == 1:
+        return pauli_matrices
+    else:
+        return np.kron(generalized_pauli_basis(num_qubits-1),pauli_matrices)
+
+
+"""
+get_stokes_parameters(state,basis)
+Desc: Given a density or pure state, return the stokes parameters.
+
+Parameters
+----------
+state : Pure State or Density
+    Given State
+basis : ndarray with shape = (4^numQubits, 2^numQubits, 2^numQubits)
+    Pauli Basis
+
+Returns
+-------
+stokes : ndarray with length = 4^numQubits
+    The stokes parameters for state
+    """
+def get_stokes_parameters(state,basis=None):
+    if basis is None:
+        num_qubits = np.log2(state.shape[0])
+        num_qubits = int(num_qubits)
+        basis = generalized_pauli_basis(num_qubits)
+    if isStateVector(state):
+        state = toDensity(state)
+    stokes = np.array([np.trace(np.matmul(state,b)) for b in basis])
+    return stokes
 
 """
 t_matrix(t)
 Desc: Converts a list of t values to an lower t matrix.
 
 Parameters
 ----------
```

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/TomoFunctionsHelpers.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/TomoFunctionsHelpers.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/Utilities.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/Utilities.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/__init__.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/__init__.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/QuantumTomography/cli.py` & `Quantum-Tomography-1.0.7.0/src/QuantumTomography/cli.py`

 * *Files identical despite different names*

### Comparing `Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/PKG-INFO` & `Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quantum-Tomography
-Version: 1.0.6.0
+Version: 1.0.7.0
 Summary: A python library to help perform tomography on a quantum state.
 Home-page: https://github.com/KwiatQIM/Quantum-Tomography
 Author: University of Illinois
 Author-email: turroscott@gmail.com
 License: MIT
 Project-URL: Documentation, https://quantumtomo.web.illinois.edu/Doc/
 Project-URL: Video Tutorial, https://www.youtube.com/watch?v=I-214P0LOfQ&list=PLJLHMKtk5Pqy9w9aCuyowUF1p7pl2JCI9&index=3
```

### Comparing `Quantum-Tomography-1.0.6.0/src/Quantum_Tomography.egg-info/SOURCES.txt` & `Quantum-Tomography-1.0.7.0/src/Quantum_Tomography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

