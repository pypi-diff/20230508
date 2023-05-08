# Comparing `tmp/onnx2kerastl-0.0.85.tar.gz` & `tmp/onnx2kerastl-0.0.85.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.85.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.85.5.tar", max compression
```

## Comparing `onnx2kerastl-0.0.85.tar` & `onnx2kerastl-0.0.85.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.85/LICENSE
--rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.85/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.85/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.85/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.85/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-02 11:17:38.559496 onnx2kerastl-0.0.85/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    13847 2023-04-30 14:23:50.230260 onnx2kerastl-0.0.85/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      499 2022-10-19 12:00:07.113116 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.85/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.85/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.85/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.85/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3309 2023-04-02 11:17:38.561313 onnx2kerastl-0.0.85/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.85/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-01 11:07:12.428128 onnx2kerastl-0.0.85/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.85/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.85/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.85/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    16675 2023-04-30 14:23:13.631400 onnx2kerastl-0.0.85/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5354 2023-04-30 14:23:13.631673 onnx2kerastl-0.0.85/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.85/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.85/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-01 11:27:13.237750 onnx2kerastl-0.0.85/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.85/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.85.5/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-08 05:49:57.483750 onnx2kerastl-0.0.85.5/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.85.5/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-24 14:18:00.054331 onnx2kerastl-0.0.85.5/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.85.5/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17867 2023-05-08 05:48:07.753079 onnx2kerastl-0.0.85.5/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5354 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1032 2023-05-08 05:54:36.302817 onnx2kerastl-0.0.85.5/pyproject.toml
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.85.5/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.85/LICENSE` & `onnx2kerastl-0.0.85.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,25 @@
                 keras_inputs.append(layers[input_name])
 
                 logger.debug('Found input {0} with shape {1}'.format(input_name, input_shape))
 
     # Convert every operation separable
     node_names = []
     for node_index, node in enumerate(onnx_nodes):
+        if node.op_type == 'If':
+            if layers[node.input[0]][0]:
+                replace_node = node.attribute[0].g.node[0]
+            else:
+                replace_node = node.attribute[1].g.node[0]
+            replace_node.output.pop()
+            for i in range(len(node.output)):
+                replace_node.output.append(node.output[i])
+            node = replace_node
         node_type = node.op_type
         node_params = onnx_node_attributes_to_dict(node.attribute)
-
         # Add global converter info:
         node_params['change_ordering'] = change_ordering
         node_params['name_policy'] = name_policy
 
         node_name = str(node.output[0])
         keras_names = []
         for output_index, output in enumerate(node.output):
```

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/convolution_layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -86,27 +86,14 @@
         "use_bias": has_bias,
         "activation": None,
         "dilation_rate": dilation,
         "name": keras_name,
         "groups": n_groups}
         partial_conv = partial(keras.layers.Conv3D, **conv_args)
         layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
-        # conv = keras.layers.Conv3D(
-        #     filters=out_channels,
-        #     kernel_size=(dimension, height, width),
-        #     strides=(strides[0], strides[1], strides[2]),
-        #     padding='valid',
-        #     weights=weights,
-        #     use_bias=has_bias,
-        #     activation=None,
-        #     dilation_rate=dilation,
-        #     name=keras_name,
-        #     groups=n_groups
-        # )
-        # layers[node_name] = conv(input_0)
 
     elif len(W.shape) == 4:  # 2D conv
         logger.debug('2D convolution')
 
         padding = None
         if len(pads) == 2 and (pads[0] > 0 or pads[1] > 0):
             padding = (pads[0], pads[1])
@@ -126,40 +113,27 @@
         W = W.transpose(2, 3, 1, 0)
         height, width, channels_per_group, out_channels = W.shape
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
+
         conv_args = {"filters": out_channels,
         "kernel_size": (height, width),
         "strides": (strides[0], strides[1]),
         "padding": 'valid',
         "weights": weights,
         "use_bias": has_bias,
         "activation": None,
         "dilation_rate": dilation,
         "name": keras_name,
         "groups": n_groups}
         partial_conv = partial(keras.layers.Conv2D, **conv_args)
         layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
-        # conv = keras.layers.Conv2D(
-        #     filters=out_channels,
-        #     kernel_size=(height, width),
-        #     strides=(strides[0], strides[1]),
-        #     padding='valid',
-        #     weights=weights,
-        #     use_bias=has_bias,
-        #     activation=None,
-        #     dilation_rate=dilation,
-        #     groups=n_groups,
-        #     name=keras_name
-        # )
-        #
-        # layers[node_name] = conv(input_0)
     else:
         # 1D conv
         W = W.transpose(2, 1, 0)
         width, channels, n_filters = W.shape
         print(width, channels, n_filters, has_bias)
 
         if has_bias:
@@ -177,44 +151,19 @@
         "use_bias": has_bias,
         "activation": None,
         "dilation_rate": dilation,
         "name": keras_name,
         "groups": n_groups}
         if padding:
             conv_args['padding'] = 'same'
-            # conv = keras.layers.Conv1D(
-            #     filters=n_filters,
-            #     kernel_size=width,
-            #     strides=strides[0],
-            #     padding='same',
-            #     weights=weights,
-            #     use_bias=has_bias,
-            #     activation=None,
-            #     dilation_rate=dilation,
-            #     groups=n_groups,
-            #     name=keras_name,
-            #     data_format='channels_first')
         else:
             conv_args['padding'] = 'valid'
 
-            # conv = keras.layers.Conv1D(
-            #     filters=n_filters,
-            #     kernel_size=width,
-            #     strides=strides[0],
-            #     padding='valid',
-            #     weights=weights,
-            #     use_bias=has_bias,
-            #     activation=None,
-            #     dilation_rate=dilation,
-            #     groups=n_groups,
-            #     name=keras_name,
-            #     data_format='channels_first')
         partial_conv = partial(keras.layers.Conv1D, **conv_args)
         layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
-        # layers[node_name] = conv(input_0)
 
         # padding_name = keras_name + '_pad'
         # padding_layer = keras.layers.ZeroPadding1D(
         #     padding=(pads[0]),
         #     name=padding_name
         # )
         # print(input_0)
```

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/ltsm_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import tensorflow as tf
 import numpy as np
+from onnx2kerastl.customonnxlayer.onnxlstm import OnnxLSTM
 
 from .exceptions import UnsupportedLayer
 from .utils import ensure_tf_type, ensure_numpy_type
 
 
 def convert_lstm(node, params, layers, lambda_func, node_name, keras_name):
     """
@@ -23,28 +24,27 @@
         raise UnsupportedLayer('LSTM with non default sequence_lens')
     if 'direction' in params:
         direction = params['direction']
         if isinstance(direction, bytes):
             direction = direction.decode("utf-8")
         if direction != 'forward':
             raise UnsupportedLayer(f"LSTM with {direction} direction")
-
+    should_return_state = len(node.output) == 3
     input_tensor = tf.transpose(ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name[0]), perm=[1, 0, 2])
     weights_w = ensure_numpy_type(layers[node.input[1]])[0]
     weights_r = ensure_numpy_type(layers[node.input[2]])[0]
     weights_b = ensure_numpy_type(layers[node.input[3]])[0]
 
     initial_h_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[5]]), axis=1), input_tensor.dtype)
     initial_c_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[6]]), axis=1), input_tensor.dtype)
 
     tf.keras.backend.set_image_data_format("channels_last")
     hidden_size = params['hidden_size']
-    lstm_tensor = tf.keras.layers.LSTM(hidden_size, return_sequences=True) \
-        (input_tensor, initial_state=[initial_h_state, initial_c_state])
-
+    lstm_layer = OnnxLSTM(hidden_size, return_sequences=True, return_lstm_state=should_return_state)
+    res = lstm_layer(input_tensor, initial_h_state, initial_c_state)
     # prepare the keras lstm weights from the onnx inputs:
     w1 = np.concatenate([weights_w[0:hidden_size, :], weights_w[2 * hidden_size:3 * hidden_size, :],
                          weights_w[3 * hidden_size:4 * hidden_size, :],
                          weights_w[hidden_size:2 * hidden_size, :]]).transpose()
     w2 = np.concatenate([weights_r[0:hidden_size, :], weights_r[2 * hidden_size:3 * hidden_size, :],
                          weights_r[3 * hidden_size:4 * hidden_size, :],
                          weights_r[hidden_size:2 * hidden_size, :]]).transpose()
@@ -53,14 +53,22 @@
     bias1 = np.concatenate([weights_b_part1[0:hidden_size], weights_b_part1[2 * hidden_size:3 * hidden_size],
                             weights_b_part1[3 * hidden_size:4 * hidden_size],
                             weights_b_part1[hidden_size:2 * hidden_size]]).transpose()
     bias2 = np.concatenate([weights_b_part2[0:hidden_size], weights_b_part2[2 * hidden_size:3 * hidden_size],
                             weights_b_part2[3 * hidden_size:4 * hidden_size],
                             weights_b_part2[hidden_size:2 * hidden_size]]).transpose()
     bias = bias1 + bias2
-    lstm_tensor.node.layer.set_weights([w1, w2, bias])
+    res.node.layer.set_weights([w1, w2, bias])
     tf.keras.backend.set_image_data_format("channels_first")
-
+    if should_return_state:
+        c_out = res[:, -hidden_size:]
+        h_out = res[:, -2*hidden_size:-hidden_size]
+        flat_lstm_tensor = res[:, :-2*hidden_size]
+        lstm_tensor = tf.keras.layers.Reshape((-1, hidden_size))(flat_lstm_tensor)
+        layers[node.output[1]] = c_out
+        layers[node.output[2]] = h_out
+    else:
+        lstm_tensor = res
     lstm_tensor_in_onnx_order = tf.transpose(lstm_tensor, perm=[1, 0, 2])
     lstm_tensor_in_onnx_order = tf.expand_dims(lstm_tensor_in_onnx_order, axis=1)
-
     layers[node_name] = lstm_tensor_in_onnx_order
+
```

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/reshape_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,28 +201,39 @@
                     layers[node_name] = input_0
 
                 reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
                 layers[node_name] = reshape(layers[node_name])
 
             else:
                 input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
-                logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
-                logger.debug('Target shape :')
-                logger.debug(np.int32(input_1[1:]))
-
-                if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
-                    logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
-                    flatten = keras.layers.Flatten(name=keras_name)
-                    layers[node_name] = flatten(input_0)
+                input_0_shape = input_0.shape
+                first_mismatch = np.argmin(np.array(input_0_shape[:len(input_1)]) == input_1)
+                if (input_1 == None).any() and (np.array(input_0_shape) == None).any() and len(input_1) < len(input_0_shape)\
+                        and input_1[first_mismatch] == -1: #reshape end
+                    end_match_arr = np.array(input_0_shape[-len(input_1):]) == input_1
+                    end_idx_match = np.argmax((np.array(input_0_shape[-len(input_1):]) == input_1))
+                    end_idx_match = end_idx_match + len(input_0_shape) - len(input_1) if end_idx_match > first_mismatch \
+                                                     and end_match_arr[end_idx_match] else len(input_0_shape) + 1
+                    tf_shape = tf.shape(input_0)
+                    layers[node_name] = tf.reshape(input_0, [*tf_shape[:first_mismatch], -1, *tf_shape[end_idx_match:]])
                 else:
-                    if input_0.shape[0] != input_1[0]:  # keras reshape don't work
-                        layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
+                    logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
+                    logger.debug('Target shape :')
+                    logger.debug(np.int32(input_1[1:]))
+
+                    if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
+                        logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
+                        flatten = keras.layers.Flatten(name=keras_name)
+                        layers[node_name] = flatten(input_0)
                     else:
-                        reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
-                        layers[node_name] = reshape(input_0)
+                        if input_0.shape[0] != input_1[0]:  # keras reshape don't work
+                            layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
+                        else:
+                            reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
+                            layers[node_name] = reshape(input_0)
     else:
         raise AttributeError('Can\'t reshape dynamic size.')
 
 
 def convert_unsqueeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert unsqueeze.
@@ -319,23 +330,23 @@
             axis_index = axes_positives.index(axis)
             start = starts[axis_index]
             end = ends[axis_index] if ends[axis_index] < 2147483647 else None
             step = steps[axis_index]
             slice_spec_param.append({'start': start, 'step': step, 'stop': end})
         else:
             slice_spec_param.append({'start': None, 'step': None, 'stop': None})
-
-    input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
-    slicing_layer = SlicingOpLambda(tf.__operators__.getitem)
-    sliced = slicing_layer(input_0, slice_spec=slice_spec_param)
-
-    if is_numpy(layers[node.input[0]]):
-        layers[node_name] = sliced.numpy()
+    if is_numpy(layers[node.input[0]]) and not np.array([not x is None for x in layers[node.input[0]]]).all(): # shape with None
+        sliced = layers[node.input[0]][start:end:step]
     else:
-        layers[node_name] = sliced
+        input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
+        slicing_layer = SlicingOpLambda(tf.__operators__.getitem)
+        sliced = slicing_layer(input_0, slice_spec=slice_spec_param)
+        if is_numpy(layers[node.input[0]]):
+            sliced = sliced.numpy()
+    layers[node_name] = sliced
 
 
 def convert_squeeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert Squeeze layer
     :param node: current operation node
     :param params: operation attributes
```

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.85.5/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85/pyproject.toml` & `onnx2kerastl-0.0.85.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.85"
+version = "0.0.85.5"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.85/PKG-INFO` & `onnx2kerastl-0.0.85.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.85
+Version: 0.0.85.5
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

