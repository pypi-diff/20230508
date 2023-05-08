# Comparing `tmp/pylinalg-0.3.4.tar.gz` & `tmp/pylinalg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinalg-0.3.4.tar", max compression
+gzip compressed data, was "pylinalg-0.4.0.tar", max compression
```

## Comparing `pylinalg-0.3.4.tar` & `pylinalg-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-04-26 13:22:06.925579 pylinalg-0.3.4/LICENSE
--rw-r--r--   0        0        0      142 2023-04-26 13:22:06.925579 pylinalg-0.3.4/README.md
--rw-r--r--   0        0        0      245 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/__init__.py
--rw-r--r--   0        0        0      216 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/__init__.py
--rw-r--r--   0        0        0    19983 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/matrix.py
--rw-r--r--   0        0        0     4712 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/misc.py
--rw-r--r--   0        0        0     9272 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/quaternion.py
--rw-r--r--   0        0        0    15070 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/func/vector.py
--rw-r--r--   0        0        0        0 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pylinalg/obj/__init__.py
--rw-r--r--   0        0        0      761 2023-04-26 13:22:06.929579 pylinalg-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 pylinalg-0.3.4/setup.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pylinalg-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-08 14:13:36.995311 pylinalg-0.4.0/LICENSE
+-rw-r--r--   0        0        0      595 2023-05-08 14:13:36.995311 pylinalg-0.4.0/README.md
+-rw-r--r--   0        0        0      390 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/__init__.py
+-rw-r--r--   0        0        0    19853 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/matrix.py
+-rw-r--r--   0        0        0     4728 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/misc.py
+-rw-r--r--   0        0        0     9279 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/quaternion.py
+-rw-r--r--   0        0        0    16499 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pylinalg/vector.py
+-rw-r--r--   0        0        0      900 2023-05-08 14:13:36.995311 pylinalg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 pylinalg-0.4.0/PKG-INFO
```

### Comparing `pylinalg-0.3.4/LICENSE` & `pylinalg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylinalg-0.3.4/pylinalg/func/matrix.py` & `pylinalg-0.4.0/pylinalg/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from math import cos, sin
 
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 
 
-def matrix_combine(matrices, /, *, out=None, dtype=None):
+def mat_combine(matrices, /, *, out=None, dtype=None):
     """
     Combine a list of affine matrices by multiplying them.
 
     Note that by matrix multiplication rules, the output matrix will applied the
     given transformations in reverse order. For example, passing a scaling,
     rotation and translation matrix (in that order), will lead to a combined
     transformation matrix that applies translation first, then rotation and finally
@@ -41,15 +41,15 @@
     out[:] = matrices[0]
     for matrix in matrices[1:]:
         np.matmul(out, matrix, out=out)
 
     return out
 
 
-def matrix_make_translation(vector, /, *, out=None, dtype=None):
+def mat_from_translation(vector, /, *, out=None, dtype=None):
     """
     Make a translationmatrix given a translation vector.
 
     Parameters
     ----------
     vector : number or ndarray, [3]
         translation vector
@@ -82,15 +82,15 @@
     out[:] = 0
     diagonal[:] = 1
     out[..., :-1, -1] = vector
 
     return out
 
 
-def matrix_make_scaling(factors, /, *, out=None, dtype=None):
+def mat_from_scale(factors, /, *, out=None, dtype=None):
     """
     Make a scaling matrix given scaling factors per axis, or a
     single uniform scaling factor.
 
     Parameters
     ----------
     factor : number or ndarray, [3]
@@ -116,17 +116,15 @@
     if out is not None:
         out[:] = matrix
         return out
 
     return matrix
 
 
-def matrix_make_rotation_from_euler_angles(
-    angles, /, *, order="xyz", out=None, dtype=None
-):
+def mat_from_euler(angles, /, *, order="xyz", out=None, dtype=None):
     """
     Make a matrix given euler angles (in radians) per axis.
 
     Parameters
     ----------
     angles : ndarray, [3]
         The euler angles.
@@ -148,15 +146,15 @@
 
 
     Notes
     -----
     If you are familiar with TreeJS note that this function uses ``order`` to
     denote both the order in which rotations are applied *and* the order in
     which angles are provided in ``angles``. I.e.,
-    ``matrix_make_rotation_from_euler_angles([np.pi, np.pi, 0], order="zyx")``
+    ``mat_from_euler([np.pi, np.pi, 0], order="zyx")``
     will first rotate 180° ccw (counter-clockwise) around the z-axis, then 180°
     ccw around the y-axis, and finally 0° around the x axis.
 
     """
     angles = np.asarray(angles, dtype=float)
     order = order.lower()
 
@@ -177,18 +175,18 @@
 
         affine_matrix = np.identity(4, dtype=dtype)
         affine_matrix[:3, :3] = matrix
 
         matrices.append(affine_matrix)
 
     # note: combining in the loop would save time and memory usage
-    return matrix_combine([x for x in reversed(matrices)], out=out, dtype=dtype)
+    return mat_combine([x for x in reversed(matrices)], out=out, dtype=dtype)
 
 
-def matrix_make_rotation_from_axis_angle(axis, angle, /, *, out=None, dtype=None):
+def mat_from_axis_angle(axis, angle, /, *, out=None, dtype=None):
     """
     Make a rotation matrix given a rotation axis and an angle (in radians).
 
     Parameters
     ----------
     axis : ndarray, [3]
         The rotation axis.
@@ -220,15 +218,15 @@
     rotation += np.sin(angle) * np.cross(axis, eye * -1)
     rotation += (1 - np.cos(angle)) * (np.outer(axis, axis))
     out[:3, :3] = rotation
 
     return out
 
 
-def matrix_to_quaternion(matrix, /, *, out=None, dtype=None):
+def quat_from_mat(matrix, /, *, out=None, dtype=None):
     """
     Make a quaternion given a rotation matrix.
 
     Parameters
     ----------
     matrix : ndarray, [3]
         The rotation matrix.
@@ -278,15 +276,15 @@
 
     if out is None:
         out = np.empty((4,), dtype=dtype)
     out[:] = np.array([x, y, z, w])
     return out
 
 
-def matrix_make_transform(translation, rotation, scaling, /, *, out=None, dtype=None):
+def mat_compose(translation, rotation, scaling, /, *, out=None, dtype=None):
     """
     Compose a transformation matrix given a translation vector, a
     quaternion and a scaling vector.
 
     Parameters
     ----------
     translation : number or ndarray, [3]
@@ -304,28 +302,28 @@
         Overrides the data type of the result.
 
     Returns
     -------
     ndarray, [4, 4]
         Transformation matrix
     """
-    from .quaternion import quaternion_to_matrix
+    from .quaternion import mat_from_quat
 
-    return matrix_combine(
+    return mat_combine(
         [
-            matrix_make_translation(translation),
-            quaternion_to_matrix(rotation),
-            matrix_make_scaling(scaling),
+            mat_from_translation(translation),
+            mat_from_quat(rotation),
+            mat_from_scale(scaling),
         ],
         out=out,
         dtype=dtype,
     )
 
 
-def matrix_decompose(matrix, /, *, dtype=None, out=None):
+def mat_decompose(matrix, /, *, dtype=None, out=None):
     """
     Decompose a transformation matrix into a translation vector, a
     quaternion and a scaling vector.
 
     Parameters
     ----------
     matrix : ndarray, [4, 4]
@@ -361,20 +359,20 @@
         scaling = np.empty((3,), dtype=dtype)
     scaling[:] = np.linalg.norm(matrix[:-1, :-1], axis=0)
     if np.linalg.det(matrix) < 0:
         scaling[0] *= -1
 
     rotation = out[1] if out is not None else None
     rotation_matrix = matrix[:-1, :-1] * (1 / scaling)[None, :]
-    rotation = matrix_to_quaternion(rotation_matrix, out=rotation, dtype=dtype)
+    rotation = quat_from_mat(rotation_matrix, out=rotation, dtype=dtype)
 
     return translation, rotation, scaling
 
 
-def matrix_make_perspective(
+def mat_perspective(
     left, right, top, bottom, near, far, /, *, depth_range=(-1, 1), out=None, dtype=None
 ):
     """
     Create a perspective projection matrix.
 
     Parameters
     ----------
@@ -430,15 +428,15 @@
     out[2, 2] = c
     out[2, 3] = d
     out[3, 2] = -1
 
     return out
 
 
-def matrix_make_orthographic(
+def mat_orthographic(
     left, right, top, bottom, near, far, /, *, depth_range=(-1, 1), out=None, dtype=None
 ):
     """Create an orthographic projection matrix.
 
     The result projects points from local space into NDC (normalized device
     coordinates). Elements inside the viewing frustum defind by left, right,
     top, bottom, near, far, are projected into the unit cube centered at the
@@ -523,15 +521,15 @@
     out[..., 0, :] /= right - left
     out[..., 1, :] /= top - bottom
     out[..., 2, :] /= far - near
 
     return out
 
 
-def matrix_make_look_at(eye, target, up_reference, /, *, out=None, dtype=None):
+def mat_look_at(eye, target, up_reference, /, *, out=None, dtype=None):
     """
     Rotation that aligns two vectors.
 
     Given an entity at position `eye` looking at position `target`, this
     function computes a rotation matrix that makes the local frame "look at" the
     same direction, i.e., the matrix will rotate the local frame's z-axes
     (forward) to point in direction ``target - eye``.
@@ -612,8 +610,10 @@
         out[..., :-1, 2], out[..., :-1, 0], axisa=-1, axisb=-1, axisc=-1
     )
     out /= np.linalg.norm(out, axis=-2)[..., None, :]
 
     return out
 
 
-__all__ = [name for name in globals() if name.startswith("matrix_")]
+__all__ = [
+    name for name in globals() if name.startswith(("vec_", "mat_", "quat_", "aabb_"))
+]
```

### Comparing `pylinalg-0.3.4/pylinalg/func/misc.py` & `pylinalg-0.4.0/pylinalg/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 
-__all__ = ["aabb_to_sphere", "aabb_transform", "axis_angle_from_quaternion"]
-
 
 def aabb_to_sphere(aabb, /, *, out=None, dtype=None):
     """A sphere that envelops an Axis-Aligned Bounding Box.
 
     Parameters
     ----------
     aabb : ndarray, [2, 3]
@@ -105,15 +103,15 @@
     corners = corners @ matrix
     out[..., 0, :] = np.min(corners[..., :-1], axis=-2)
     out[..., 1, :] = np.max(corners[..., :-1], axis=-2)
 
     return out
 
 
-def axis_angle_from_quaternion(quaternion, /, *, out=None, dtype=None):
+def quat_to_axis_angle(quaternion, /, *, out=None, dtype=None):
     """Convert a quaternion to axis-angle representation.
 
     Parameters
     ----------
     quaternion : ndarray, [4]
         A quaternion describing the rotation.
     out : Tuple[ndarray, ...], optional
@@ -147,7 +145,12 @@
             2 * np.arccos(quaternion[..., 3]),
         )
     else:
         out[0][:] = quaternion[..., :3] / np.sqrt(1 - quaternion[..., 3] ** 2)
         out[1][:] = 2 * np.arccos(quaternion[..., 3])
 
     return out
+
+
+__all__ = [
+    name for name in globals() if name.startswith(("vec_", "mat_", "quat_", "aabb_"))
+]
```

### Comparing `pylinalg-0.3.4/pylinalg/func/quaternion.py` & `pylinalg-0.4.0/pylinalg/quaternion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Note that we assume unit quaternions for faster implementations"""
 
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 
 
-def quaternion_to_matrix(quaternion, /, *, out=None, dtype=None):
+def mat_from_quat(quaternion, /, *, out=None, dtype=None):
     """
     Make a rotation matrix given a quaternion.
 
     Parameters
     ----------
     quaternion : ndarray, [4]
         Quaternion.
@@ -70,15 +70,15 @@
     out[..., 0, 2] = xz + wy
     out[..., 1, 2] = yz - wx
     out[..., 2, 2] = 1 - (xx + yy)
 
     return out
 
 
-def quaternion_multiply(a, b, /, *, out=None, dtype=None):
+def quat_mul(a, b, /, *, out=None, dtype=None):
     """
     Multiply two quaternions
 
     Parameters
     ----------
     a : ndarray, [4]
         Left-hand quaternion
@@ -108,15 +108,15 @@
 
     out[:3] = xyz
     out[3] = w
 
     return out
 
 
-def quaternion_make_from_unit_vectors(source, target, /, *, out=None, dtype=None):
+def quat_from_vecs(source, target, /, *, out=None, dtype=None):
     """Rotate one vector onto another.
 
     Create a quaternion that rotates ``source`` onto ``target``.
 
     Parameters
     ----------
     source : ndarray, [3]
@@ -178,18 +178,18 @@
 
         # if two axes are non-zero we can use those
         if np.any(both_nonzero):
             fallback[both_nonzero, :] = (0, -1, 1) * template[both_nonzero, [0, 2, 1]]
 
         axis[use_fallback] = np.squeeze(fallback)
 
-    return quaternion_make_from_axis_angle(axis, angle, out=out)
+    return quat_from_axis_angle(axis, angle, out=out)
 
 
-def quaternion_inverse(quaternion, /, *, out=None, dtype=None):
+def quat_inv(quaternion, /, *, out=None, dtype=None):
     """
     Inverse of a given quaternion
 
     Parameters
     ----------
     a : ndarray, [3]
         First unit vector
@@ -213,15 +213,15 @@
 
     out[:] = quaternion
     out[..., :3] *= -1
 
     return out
 
 
-def quaternion_make_from_axis_angle(axis, angle, /, *, out=None, dtype=None):
+def quat_from_axis_angle(axis, angle, /, *, out=None, dtype=None):
     """Quaternion from axis-angle pair.
 
     Create a quaternion representing the rotation of an given angle
     about a given unit vector
 
     Parameters
     ----------
@@ -247,23 +247,24 @@
     angle = np.asarray(angle, dtype=float)
 
     if out is None:
         out_shape = np.broadcast_shapes(axis.shape[:-1], angle.shape)
         out = np.empty((*out_shape, 4), dtype=dtype)
 
     # result should be independent of the length of the given axis
-    axis /= np.linalg.norm(axis, axis=-1)
+    lengths_shape = axis.shape[:-1] + (1,)
+    axis /= np.linalg.norm(axis, axis=-1).reshape(lengths_shape)
 
-    out[..., :3] = axis * np.sin(angle / 2)
+    out[..., :3] = axis * np.sin(angle / 2).reshape(lengths_shape)
     out[..., 3] = np.cos(angle / 2)
 
     return out
 
 
-def quaternion_make_from_euler_angles(angles, /, *, order="XYZ", out=None, dtype=None):
+def quat_from_euler(angles, /, *, order="XYZ", out=None, dtype=None):
     """
     Create a quaternion from euler angles.
 
     Parameters
     ----------
     angles : ndarray, [3]
         A set of XYZ euler angles.
@@ -300,15 +301,17 @@
     quaternions[:, ..., -1] = np.cos(angles / 2)
     quaternions[np.arange(len(order)), ..., order] = np.sin(angles / 2)
 
     # multiple euler-angle quaternions respecting
     out[:] = quaternions[0]
     for idx in range(1, len(quaternions)):
         if is_extrinsic[idx]:
-            quaternion_multiply(out, quaternions[idx], out=out)
+            quat_mul(out, quaternions[idx], out=out)
         else:
-            quaternion_multiply(quaternions[idx], out, out=out)
+            quat_mul(quaternions[idx], out, out=out)
 
     return out
 
 
-__all__ = [name for name in globals() if name.startswith("quaternion_")]
+__all__ = [
+    name for name in globals() if name.startswith(("vec_", "mat_", "quat_", "aabb_"))
+]
```

### Comparing `pylinalg-0.3.4/pylinalg/func/vector.py` & `pylinalg-0.4.0/pylinalg/vector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-def vector_normalize(vectors, /, *, out=None, dtype=None):
+def vec_normalize(vectors, /, *, out=None, dtype=None):
     """
     Normalize an array of vectors.
 
     Parameters
     ----------
     vectors : array_like, [..., 3]
         array of vectors
@@ -27,15 +27,15 @@
         out = np.empty_like(vectors, dtype=dtype)
 
     lengths_shape = vectors.shape[:-1] + (1,)
     lengths = np.linalg.norm(vectors, axis=-1).reshape(lengths_shape)
     return np.divide(vectors, lengths, out=out)
 
 
-def vector_make_homogeneous(vectors, /, *, w=1, out=None, dtype=None):
+def vec_homogeneous(vectors, /, *, w=1, out=None, dtype=None):
     """
     Append homogeneous coordinates to vectors.
 
     Parameters
     ----------
     vectors : array_like, [..., 3]
         array of vectors
@@ -63,15 +63,15 @@
     if out is None:
         out = np.empty_like(vectors, shape=shape, dtype=dtype)
     out[..., -1] = w
     out[..., :-1] = vectors
     return out
 
 
-def vector_apply_matrix(vectors, matrix, /, *, w=1, out=None, dtype=None):
+def vec_transform(vectors, matrix, /, *, w=1, out=None, dtype=None):
     """
     Apply a transformation matrix to a vector.
 
     Parameters
     ----------
     vectors : ndarray, [3]
         Array of vectors
@@ -98,23 +98,23 @@
     vectors = np.asarray(vectors, dtype=float)
     matrix = np.asarray(matrix, dtype=float)
 
     if out is None:
         out_shape = np.broadcast_shapes(vectors.shape[:-1], matrix.shape[:-2])
         out = np.empty((*out_shape, 3), dtype=dtype)
 
-    vectors = vector_make_homogeneous(vectors, w=w)
+    vectors = vec_homogeneous(vectors, w=w)
     result = matrix @ vectors[..., None]
     result /= result[..., -1, :][..., None, :]
     out[:] = result[..., :-1, 0]
 
     return out
 
 
-def vector_unproject(vector, matrix, /, *, depth=0, out=None, dtype=None):
+def vec_unproject(vector, matrix, /, *, depth=0, out=None, dtype=None):
     """
     Un-project a vector from 2D space to 3D space.
 
     Find a ``vectorB`` in 3D euclidean space such that the projection
     ``matrix @ vectorB`` yields the provided vector (in 2D euclidean
     space). Since the solution to the above is a 1D subspace of 3D space (a
     line), ``depth`` is used to select a single vector within.
@@ -170,15 +170,15 @@
     out_hom = vector_hom @ inverse_projection.T
     scale = out_hom[..., -1][..., None]
     out[:] = (out_hom / scale)[..., :-1]
 
     return out
 
 
-def vector_apply_quaternion(vector, quaternion, /, *, out=None, dtype=None):
+def vec_transform_quat(vector, quaternion, /, *, out=None, dtype=None):
     """Rotate a vector using a quaternion.
 
     Parameters
     ----------
     vector : ndarray, [3]
         The vector to be rotated.
     quaternion : ndarray, [4]
@@ -215,15 +215,15 @@
         quat_scalar**2 - np.sum(quat_vector * quat_vector, axis=-1, keepdims=True)
     ) * vector
     out += 2 * quat_scalar * np.cross(quat_vector, vector)
 
     return out
 
 
-def vector_spherical_to_euclidean(spherical, /, *, out=None, dtype=None):
+def vec_spherical_to_euclidian(spherical, /, *, out=None, dtype=None):
     """Convert spherical -> euclidian coordinates.
 
     Parameters
     ----------
     spherical : ndarray, [3]
         A vector in spherical coordinates (r, phi, theta). Phi and theta are
         measured in radians.
@@ -257,15 +257,15 @@
     out[..., 0] = r * np.sin(phi) * np.sin(theta)
     out[..., 1] = r * np.cos(phi)
     out[..., 2] = r * np.sin(phi) * np.cos(theta)
 
     return out
 
 
-def vector_distance_between(vector_a, vector_b, /, *, out=None, dtype=None):
+def vec_dist(vector_a, vector_b, /, *, out=None, dtype=None):
     """The distance between two vectors
 
     Parameters
     ----------
     vector_a : ndarray, [3]
         The first vector.
     vector_b : ndarray, [3]
@@ -295,15 +295,15 @@
         out[:] = np.linalg.norm(vector_a - vector_b, axis=-1)
     else:
         raise ValueError("Can't use `out` with scalar output.")
 
     return out
 
 
-def vector_angle_between(vector_a, vector_b, /, *, out=None, dtype=None):
+def vec_angle(vector_a, vector_b, /, *, out=None, dtype=None):
     """The angle between two vectors
 
     Parameters
     ----------
     vector_a : ndarray, [3]
         The first vector.
     vector_b : ndarray, [3]
@@ -346,15 +346,15 @@
         out[:] = np.arccos(the_cos)
     else:
         raise ValueError("Can't use `out` with scalar output.")
 
     return out
 
 
-def vector_from_matrix_position(homogeneous_matrix, /, *, out=None, dtype=None):
+def mat_decompose_translation(homogeneous_matrix, /, *, out=None, dtype=None):
     """Position component of a homogeneous matrix.
 
     Parameters
     ----------
     homogeneous_matrix : ndarray, [4, 4]
         The matrix of which the position/translation component will be
         extracted.
@@ -379,15 +379,15 @@
         out = np.empty((*homogeneous_matrix.shape[:-2], 3), dtype=dtype)
 
     out[:] = homogeneous_matrix[..., :-1, -1]
 
     return out
 
 
-def vector_euclidean_to_spherical(euclidean, /, *, out=None, dtype=None):
+def vec_euclidian_to_spherical(euclidean, /, *, out=None, dtype=None):
     """Convert euclidean -> spherical coordinates
 
     Parameters
     ----------
     euclidean : ndarray, [3]
         A vector in euclidean coordinates.
     out : ndarray, optional
@@ -429,15 +429,15 @@
     out[..., 2] = np.divide(euclidean[..., 1], out[..., 0], where=r_nonzero)
     out[..., 2] = np.arccos(out[..., 2], where=r_nonzero)
     out[..., 2] = np.where(needs_flip, 2 * np.pi - out[..., 2], out[..., 2])
 
     return out
 
 
-def vector_make_spherical_safe(vector, /, *, out=None, dtype=None):
+def vec_spherical_safe(vector, /, *, out=None, dtype=None):
     """Normalize sperhical coordinates.
 
     Normalizes a vector of spherical coordinates to restrict phi to [0, pi) and
     theta to [0, 2pi).
 
     Parameters
     ----------
@@ -472,8 +472,61 @@
 
     out[..., 1] = np.where(out[..., 1] == np.pi, 0, out[..., 1])
     out[..., 2] = np.where(out[..., 2] == 2 * np.pi, 0, out[..., 2])
 
     return out
 
 
-__all__ = [name for name in globals() if name.startswith("vector_")]
+def quat_to_euler(quaternion, /, *, out=None, dtype=None):
+    """Convert quaternions to XYZ Euler angles.
+
+    Parameters
+    ----------
+    quaternion : ndarray, [4]
+        The quaternion to convert (in xyzw format).
+    out : ndarray, optional
+        A location into which the result is stored. If provided, it
+        must have a shape that the inputs broadcast to. If not provided or
+        None, a freshly-allocated array is returned. A tuple must have
+        length equal to the number of outputs.
+    dtype : data-type, optional
+        Overrides the data type of the result.
+
+    Returns
+    -------
+    out : ndarray, [3]
+        The XYZ Euler angles.
+    """
+    quaternion = np.asarray(quaternion, dtype=float)
+
+    if out is None:
+        out = np.empty((*quaternion.shape[:-1], 3), dtype=dtype)
+
+    ysqr = quaternion[..., 1] ** 2
+
+    t0 = 2 * (
+        quaternion[..., 3] * quaternion[..., 0]
+        + quaternion[..., 1] * quaternion[..., 2]
+    )
+    t1 = 1 - 2 * (quaternion[..., 0] ** 2 + ysqr)
+    out[..., 0] = np.arctan2(t0, t1)
+
+    t2 = 2 * (
+        quaternion[..., 3] * quaternion[..., 1]
+        - quaternion[..., 2] * quaternion[..., 0]
+    )
+    t2 = np.clip(t2, a_min=-1, a_max=1)
+    out[..., 1] = np.arcsin(t2)
+
+    t3 = 2 * (
+        quaternion[..., 3] * quaternion[..., 2]
+        + quaternion[..., 0] * quaternion[..., 1]
+    )
+    t4 = 1 - 2 * (ysqr + quaternion[..., 2] ** 2)
+    out[..., 2] = np.arctan2(t3, t4)
+
+    return out
+
+
+__all__ = [
+    name for name in globals() if name.startswith(("vec_", "mat_", "quat_", "aabb_"))
+]
```

### Comparing `pylinalg-0.3.4/pyproject.toml` & `pylinalg-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 [tool.poetry]
 name = "pylinalg"
-version = "0.3.4"
+version = "0.4.0"
 description = "Linear algebra utilities for Python"
 authors = ["Korijn van Golen <korijn@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/pygfx/pylinalg"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 numpy = ">=1.20.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "*"
 flake8 = "*"
 black = "*"
 flake8-black = "*"
 flake8-isort = "*"
 pep8-naming = "*"
 pytest-cov = "*"
+packaging = "*"
 twine = { version = "*", python = "<4.0.0" }
 pytest-watcher = { version = "*", python = "<4.0.0" }
 isort = { version = "*", python = "<4.0.0" }
 hypothesis = {extras = ["numpy"], version = "^6.61.0"}
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "*"
+sphinx-rtd-theme = "*"
+
 [build-system]
-requires = ["poetry>=1.2.0"]
+requires = ["poetry>=1.4.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

