# Comparing `tmp/hpverif-2.5.3-py3-none-any.whl.zip` & `tmp/hpverif-2.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 12210 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     3130 b- defN 23-May-04 16:55 hpverif/Calibraton.py
--rw-rw-rw-  2.0 fat     4063 b- defN 23-May-04 16:33 hpverif/FrameCapture.py
--rw-rw-rw-  2.0 fat     2641 b- defN 23-May-04 16:34 hpverif/FrameCapturePLY.py
--rw-rw-rw-  2.0 fat     4101 b- defN 23-May-04 15:36 hpverif/PointCloud.py
--rw-rw-rw-  2.0 fat     5558 b- defN 23-May-04 16:28 hpverif/Segmentation.py
--rw-rw-rw-  2.0 fat     2517 b- defN 23-May-04 15:39 hpverif/ShowFiles.py
--rw-rw-rw-  2.0 fat     5059 b- defN 23-May-04 15:38 hpverif/Theoretical_distance.py
--rw-rw-rw-  2.0 fat     1937 b- defN 23-May-04 16:55 hpverif/Verification.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-13 14:22 hpverif/__init__.py
--rw-rw-rw-  2.0 fat      409 b- defN 23-May-04 16:33 hpverif/driver.py
--rw-rw-rw-  2.0 fat      335 b- defN 23-May-04 16:55 hpverif-2.5.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 16:55 hpverif-2.5.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-04 16:55 hpverif-2.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1086 b- defN 23-May-04 16:55 hpverif-2.5.3.dist-info/RECORD
-14 files, 30936 bytes uncompressed, 10420 bytes compressed:  66.3%
+Zip file size: 12510 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3046 b- defN 23-May-08 14:15 hpverif/Calibraton.py
+-rw-r--r--  2.0 unx      449 b- defN 23-May-08 15:40 hpverif/Driver.py
+-rw-r--r--  2.0 unx     3961 b- defN 23-May-08 14:15 hpverif/FrameCapture.py
+-rw-r--r--  2.0 unx     2576 b- defN 23-May-08 14:15 hpverif/FrameCapturePLY.py
+-rw-r--r--  2.0 unx     3967 b- defN 23-May-08 14:15 hpverif/PointCloud.py
+-rw-r--r--  2.0 unx     5425 b- defN 23-May-08 14:15 hpverif/Segmentation.py
+-rw-r--r--  2.0 unx     2443 b- defN 23-May-08 14:15 hpverif/ShowFiles.py
+-rw-r--r--  2.0 unx     4934 b- defN 23-May-08 14:15 hpverif/Theoretical_distance.py
+-rw-r--r--  2.0 unx     1871 b- defN 23-May-08 15:52 hpverif/Verification.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-08 14:15 hpverif/__init__.py
+-rw-r--r--  2.0 unx      389 b- defN 23-May-08 14:15 hpverif/driver.py
+-rw-r--r--  2.0 unx      321 b- defN 23-May-08 16:40 hpverif-2.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:40 hpverif-2.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-08 16:40 hpverif-2.5.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1159 b- defN 23-May-08 16:40 hpverif-2.5.4.dist-info/RECORD
+15 files, 30641 bytes uncompressed, 10610 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: hpverif/Calibraton.py
 Comment: 
 
+Filename: hpverif/Driver.py
+Comment: 
+
 Filename: hpverif/FrameCapture.py
 Comment: 
 
 Filename: hpverif/FrameCapturePLY.py
 Comment: 
 
 Filename: hpverif/PointCloud.py
@@ -24,20 +27,20 @@
 
 Filename: hpverif/__init__.py
 Comment: 
 
 Filename: hpverif/driver.py
 Comment: 
 
-Filename: hpverif-2.5.3.dist-info/METADATA
+Filename: hpverif-2.5.4.dist-info/METADATA
 Comment: 
 
-Filename: hpverif-2.5.3.dist-info/WHEEL
+Filename: hpverif-2.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: hpverif-2.5.3.dist-info/top_level.txt
+Filename: hpverif-2.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hpverif-2.5.3.dist-info/RECORD
+Filename: hpverif-2.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpverif/Calibraton.py

 * *Ordering differences only*

```diff
@@ -1,84 +1,84 @@
-    
-import pyrealsense2 as rs
-import numpy as np
-import cv2
-
-
-class Calibration:
-   
-    def __init__ (self):
-        self.pipeline = rs.pipeline()
-        self.config = rs.config()
-
-    def enable_stream(self):
-    
-        # Get device product line for setting a supporting resolution
-        pipeline_wrapper = rs.pipeline_wrapper(self.pipeline)
-        pipeline_profile = self.config.resolve(pipeline_wrapper)
-        device = pipeline_profile.get_device()
-        device_product_line = str(device.get_info(rs.camera_info.product_line))
-
-        found_rgb = False
-        for s in device.sensors:
-            if s.get_info(rs.camera_info.name) == 'RGB Camera':
-                found_rgb = True
-                break
-        if not found_rgb:
-            print("The demo requires Depth camera with Color sensor")
-            exit(0)
-
-        self.config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
-
-        if device_product_line == 'L500':
-            self.config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
-        else:
-            self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
-        
-        
-
-
-    def calibrate (self):
-    # Start streaming
-        self.pipeline.start(self.config)
-        depth_frame_set={}
-        color_frame_set={}
-        for x in range(20):
-                # Wait for a coherent pair of frames: depth and color
-                frames = self.pipeline.wait_for_frames()
-                depth_frame_set[x] = frames.get_depth_frame()
-                color_frame_set[x] = frames.get_color_frame()
-                if not depth_frame_set[x] or not color_frame_set[x]:
-                    continue
-
-                # Convert images to numpy arrays
-                depth_image = np.asanyarray(depth_frame_set[x].get_data())
-                color_image = np.asanyarray(color_frame_set[x].get_data())
-
-                # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
-                depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_JET)
-
-                depth_colormap_dim = depth_colormap.shape
-                color_colormap_dim = color_image.shape
-
-                # If depth and color resolutions are different, resize color image to match depth image for display
-                if depth_colormap_dim != color_colormap_dim:
-                    resized_color_image = cv2.resize(color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA)
-                    images = np.hstack((resized_color_image, depth_colormap))
-                else:
-                    images = np.hstack((color_image, depth_colormap))
-
-                # Show images
-                cv2.namedWindow('RealSense', cv2.WINDOW_AUTOSIZE)
-                cv2.imshow('RealSense', images)
-                cv2.waitKey(1)
-
-
-
-            # Stop streaming
-        self.pipeline.stop()
-
-
-        f = open ("./output.txt", "w")
-        f.write( depth_frame_set[1])
-        f.close()
-
+    
+import pyrealsense2 as rs
+import numpy as np
+import cv2
+
+
+class Calibration:
+   
+    def __init__ (self):
+        self.pipeline = rs.pipeline()
+        self.config = rs.config()
+
+    def enable_stream(self):
+    
+        # Get device product line for setting a supporting resolution
+        pipeline_wrapper = rs.pipeline_wrapper(self.pipeline)
+        pipeline_profile = self.config.resolve(pipeline_wrapper)
+        device = pipeline_profile.get_device()
+        device_product_line = str(device.get_info(rs.camera_info.product_line))
+
+        found_rgb = False
+        for s in device.sensors:
+            if s.get_info(rs.camera_info.name) == 'RGB Camera':
+                found_rgb = True
+                break
+        if not found_rgb:
+            print("The demo requires Depth camera with Color sensor")
+            exit(0)
+
+        self.config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
+
+        if device_product_line == 'L500':
+            self.config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
+        else:
+            self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
+        
+        
+
+
+    def calibrate (self):
+    # Start streaming
+        self.pipeline.start(self.config)
+        depth_frame_set={}
+        color_frame_set={}
+        for x in range(20):
+                # Wait for a coherent pair of frames: depth and color
+                frames = self.pipeline.wait_for_frames()
+                depth_frame_set[x] = frames.get_depth_frame()
+                color_frame_set[x] = frames.get_color_frame()
+                if not depth_frame_set[x] or not color_frame_set[x]:
+                    continue
+
+                # Convert images to numpy arrays
+                depth_image = np.asanyarray(depth_frame_set[x].get_data())
+                color_image = np.asanyarray(color_frame_set[x].get_data())
+
+                # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
+                depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_JET)
+
+                depth_colormap_dim = depth_colormap.shape
+                color_colormap_dim = color_image.shape
+
+                # If depth and color resolutions are different, resize color image to match depth image for display
+                if depth_colormap_dim != color_colormap_dim:
+                    resized_color_image = cv2.resize(color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA)
+                    images = np.hstack((resized_color_image, depth_colormap))
+                else:
+                    images = np.hstack((color_image, depth_colormap))
+
+                # Show images
+                cv2.namedWindow('RealSense', cv2.WINDOW_AUTOSIZE)
+                cv2.imshow('RealSense', images)
+                cv2.waitKey(1)
+
+
+
+            # Stop streaming
+        self.pipeline.stop()
+
+
+        f = open ("./output.txt", "w")
+        f.write( depth_frame_set[1])
+        f.close()
+
```

## hpverif/FrameCapture.py

 * *Ordering differences only*

```diff
@@ -1,103 +1,103 @@
-    
-import pyrealsense2 as rs
-import numpy as np
-import cv2
-
-
-class Frame_Capture:
-   
-    def __init__ (self):
-        self.pipeline = rs.pipeline()
-        self.config = rs.config()
-
-
-
-    def get_and_configure_device (self, high):
-        
-        if(high<2):
-            pipeline_wrapper = rs.pipeline_wrapper(self.pipeline)
-            pipeline_profile = self.config.resolve(pipeline_wrapper)
-            device = pipeline_profile.get_device()
-            device_product_line = str(device.get_info(rs.camera_info.product_line))
-
-            found_rgb = False
-            for s in device.sensors:
-                if s.get_info(rs.camera_info.name) == 'RGB Camera':
-                    found_rgb = True
-                    break
-            if not found_rgb:
-                print("The demo requires Depth camera with Color sensor")
-                exit(0)
-
-            self.config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
-
-            if device_product_line == 'L500':
-                self.config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
-            else:
-                self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
-        
-        
-        else :
-            self.config.enable_device('017322075378')
-            self.config.enable_stream(rs.stream.depth, 1280, 720, rs.format.z16, 30)
-            self.config.enable_stream(rs.stream.color, 1280, 720, rs.format.bgr8, 30)
-            self.config.enable_stream(rs.stream.accel)
-            self.config.enable_stream(rs.stream.gyro)
-        
-
-    def capture (self, frames ,filename, high):
-
-        self.config.enable_record_to_file(filename)
-        
-        # Start streaming
-        pipe_profile = self.pipeline.start(self.config)
-
-        if(high>2):
-            depth_sensor = pipe_profile.get_device().first_depth_sensor()
-
-            #Activem High Accuracy Mode (3); High Density (4)
-            visualpreset = depth_sensor.get_option_value_description(rs.option.visual_preset,4)
-            depth_sensor.set_option(rs.option.visual_preset, 4)
-            
-        # rs.recorder() #Start recording
-        try:
-            for i in range(frames):
-
-                # Wait for a coherent pair of frames: depth and color
-                frames = self.pipeline.wait_for_frames()
-                depth_frame = frames.get_depth_frame()
-                color_frame = frames.get_color_frame()
-                if not depth_frame or not color_frame:
-                    continue
-
-                # Convert images to numpy arrays
-                depth_image = np.asanyarray(depth_frame.get_data())
-                color_image = np.asanyarray(color_frame.get_data())
-
-                if(i==10):
-                    fin_depth_image = depth_image
-                    fin_color_image = color_image
-
-                # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
-                depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_JET)
-
-                depth_colormap_dim = depth_colormap.shape
-                color_colormap_dim = color_image.shape
-
-                # If depth and color resolutions are different, resize color image to match depth image for display
-                if depth_colormap_dim != color_colormap_dim:
-                    resized_color_image = cv2.resize(color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA)
-                    images = np.hstack((resized_color_image, depth_colormap))
-                else:
-                    images = np.hstack((color_image, depth_colormap))
-
-                # Show images
-                cv2.namedWindow('RealSense', cv2.WINDOW_AUTOSIZE)
-                cv2.imshow('RealSense', images)
-                cv2.waitKey(1)
-
-        finally:
-            # Stop streaming
-            self.pipeline.stop()
-            return fin_depth_image,fin_color_image
+    
+import pyrealsense2 as rs
+import numpy as np
+import cv2
+
+
+class Frame_Capture:
+   
+    def __init__ (self):
+        self.pipeline = rs.pipeline()
+        self.config = rs.config()
+
+
+
+    def get_and_configure_device (self, high):
+        
+        if(high<2):
+            pipeline_wrapper = rs.pipeline_wrapper(self.pipeline)
+            pipeline_profile = self.config.resolve(pipeline_wrapper)
+            device = pipeline_profile.get_device()
+            device_product_line = str(device.get_info(rs.camera_info.product_line))
+
+            found_rgb = False
+            for s in device.sensors:
+                if s.get_info(rs.camera_info.name) == 'RGB Camera':
+                    found_rgb = True
+                    break
+            if not found_rgb:
+                print("The demo requires Depth camera with Color sensor")
+                exit(0)
+
+            self.config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
+
+            if device_product_line == 'L500':
+                self.config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
+            else:
+                self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
+        
+        
+        else :
+            self.config.enable_device('017322075378')
+            self.config.enable_stream(rs.stream.depth, 1280, 720, rs.format.z16, 30)
+            self.config.enable_stream(rs.stream.color, 1280, 720, rs.format.bgr8, 30)
+            self.config.enable_stream(rs.stream.accel)
+            self.config.enable_stream(rs.stream.gyro)
+        
+
+    def capture (self, frames ,filename, high):
+
+        self.config.enable_record_to_file(filename)
+        
+        # Start streaming
+        pipe_profile = self.pipeline.start(self.config)
+
+        if(high>2):
+            depth_sensor = pipe_profile.get_device().first_depth_sensor()
+
+            #Activem High Accuracy Mode (3); High Density (4)
+            visualpreset = depth_sensor.get_option_value_description(rs.option.visual_preset,4)
+            depth_sensor.set_option(rs.option.visual_preset, 4)
+            
+        # rs.recorder() #Start recording
+        try:
+            for i in range(frames):
+
+                # Wait for a coherent pair of frames: depth and color
+                frames = self.pipeline.wait_for_frames()
+                depth_frame = frames.get_depth_frame()
+                color_frame = frames.get_color_frame()
+                if not depth_frame or not color_frame:
+                    continue
+
+                # Convert images to numpy arrays
+                depth_image = np.asanyarray(depth_frame.get_data())
+                color_image = np.asanyarray(color_frame.get_data())
+
+                if(i==10):
+                    fin_depth_image = depth_image
+                    fin_color_image = color_image
+
+                # Apply colormap on depth image (image must be converted to 8-bit per pixel first)
+                depth_colormap = cv2.applyColorMap(cv2.convertScaleAbs(depth_image, alpha=0.03), cv2.COLORMAP_JET)
+
+                depth_colormap_dim = depth_colormap.shape
+                color_colormap_dim = color_image.shape
+
+                # If depth and color resolutions are different, resize color image to match depth image for display
+                if depth_colormap_dim != color_colormap_dim:
+                    resized_color_image = cv2.resize(color_image, dsize=(depth_colormap_dim[1], depth_colormap_dim[0]), interpolation=cv2.INTER_AREA)
+                    images = np.hstack((resized_color_image, depth_colormap))
+                else:
+                    images = np.hstack((color_image, depth_colormap))
+
+                # Show images
+                cv2.namedWindow('RealSense', cv2.WINDOW_AUTOSIZE)
+                cv2.imshow('RealSense', images)
+                cv2.waitKey(1)
+
+        finally:
+            # Stop streaming
+            self.pipeline.stop()
+            return fin_depth_image,fin_color_image
```

## hpverif/FrameCapturePLY.py

 * *Ordering differences only*

```diff
@@ -1,66 +1,66 @@
-    
-import pyrealsense2 as rs
-
-
-
-class Frame_Capture_PLY:
-   
-    def __init__ (self):
-        self.pipeline = rs.pipeline()
-        self.config = rs.config()
-        self.points = rs.points()
-        self.spatial = rs.spatial_filter()
-        self.temporal = rs.temporal_filter()
-        self.hole_filling = rs.hole_filling_filter()
-
-
-    def get_and_configure_device (self):
-
-        self.config.enable_device('017322075378')
-        self.config.enable_stream(rs.stream.depth, 1280, 720, rs.format.z16, 30)
-        self.config.enable_stream(rs.stream.color, 1280, 720, rs.format.bgr8, 30)
-        self.config.enable_stream(rs.stream.accel)
-        self.config.enable_stream(rs.stream.gyro)
-        self.spatial.set_option(rs.option.filter_magnitude, 2)
-        self.spatial.set_option(rs.option.filter_smooth_alpha, 0.5)
-        self.spatial.set_option(rs.option.filter_smooth_delta, 20)
-
-    def capture (self,filename, high):
-
-        
-
-        # Start streaming with chosen configuration
-        pipe_profile = self.pipeline.start(self.config)
-
-        if(high>2):
-            depth_sensor = pipe_profile.get_device().first_depth_sensor()
-
-            #Activem High Accuracy Mode (3); High Density (4)
-            visualpreset = depth_sensor.get_option_value_description(rs.option.visual_preset,4)
-            depth_sensor.set_option(rs.option.visual_preset, 4)
-        # We'll use the colorizer to generate texture for our PLY
-        # (alternatively, texture can be obtained from color or infrared stream)
-        colorizer = rs.colorizer()
-
-        try:
-            # Wait for the next set of frames from the camera
-            frames = self.pipeline.wait_for_frames()
-            colorized = colorizer.process(frames)
-            depth = frames.get_depth_frame()
-            depth = self.temporal.process(depth)
-            depth = self.spatial.process(depth)
-            color = frames.get_color_frame()
-            # Create save_to_ply object
-            ply = rs.save_to_ply(filename+ ".ply")
-            # Set options to the desired values
-            # In this example we'll generate a textual PLY with normals (mesh is already created by default)
-            ply.set_option(rs.save_to_ply.option_ply_binary, False)
-            ply.set_option(rs.save_to_ply.option_ply_normals, True)
-
-            print("Saving to 1.ply...")
-            # Apply the processing block to the frameset which contains the depth frame and the texture
-            ply.process(colorized)
-            print("Done")
-        finally:
-            self.pipeline.stop()
+    
+import pyrealsense2 as rs
+
+
+
+class Frame_Capture_PLY:
+   
+    def __init__ (self):
+        self.pipeline = rs.pipeline()
+        self.config = rs.config()
+        self.points = rs.points()
+        self.spatial = rs.spatial_filter()
+        self.temporal = rs.temporal_filter()
+        self.hole_filling = rs.hole_filling_filter()
+
+
+    def get_and_configure_device (self):
+
+        self.config.enable_device('017322075378')
+        self.config.enable_stream(rs.stream.depth, 1280, 720, rs.format.z16, 30)
+        self.config.enable_stream(rs.stream.color, 1280, 720, rs.format.bgr8, 30)
+        self.config.enable_stream(rs.stream.accel)
+        self.config.enable_stream(rs.stream.gyro)
+        self.spatial.set_option(rs.option.filter_magnitude, 2)
+        self.spatial.set_option(rs.option.filter_smooth_alpha, 0.5)
+        self.spatial.set_option(rs.option.filter_smooth_delta, 20)
+
+    def capture (self,filename, high):
+
+        
+
+        # Start streaming with chosen configuration
+        pipe_profile = self.pipeline.start(self.config)
+
+        if(high>2):
+            depth_sensor = pipe_profile.get_device().first_depth_sensor()
+
+            #Activem High Accuracy Mode (3); High Density (4)
+            visualpreset = depth_sensor.get_option_value_description(rs.option.visual_preset,4)
+            depth_sensor.set_option(rs.option.visual_preset, 4)
+        # We'll use the colorizer to generate texture for our PLY
+        # (alternatively, texture can be obtained from color or infrared stream)
+        colorizer = rs.colorizer()
+
+        try:
+            # Wait for the next set of frames from the camera
+            frames = self.pipeline.wait_for_frames()
+            colorized = colorizer.process(frames)
+            depth = frames.get_depth_frame()
+            depth = self.temporal.process(depth)
+            depth = self.spatial.process(depth)
+            color = frames.get_color_frame()
+            # Create save_to_ply object
+            ply = rs.save_to_ply(filename+ ".ply")
+            # Set options to the desired values
+            # In this example we'll generate a textual PLY with normals (mesh is already created by default)
+            ply.set_option(rs.save_to_ply.option_ply_binary, False)
+            ply.set_option(rs.save_to_ply.option_ply_normals, True)
+
+            print("Saving to 1.ply...")
+            # Apply the processing block to the frameset which contains the depth frame and the texture
+            ply.process(colorized)
+            print("Done")
+        finally:
+            self.pipeline.stop()
```

## hpverif/PointCloud.py

 * *Ordering differences only*

```diff
@@ -1,134 +1,134 @@
-import open3d as o3d
-import cv2
-import numpy as np
-import os 
-import imageio.v3 as iio
-
-class PointCloud:
-
-    def __init__(self) -> None:
-        pass
-
-    
-    def createPointCloud (self, depthframe, filename):
-
-
-      
-      
-        
-        os.makedirs(filename, exist_ok=True)
-        
-
-        # Load the depth frame as a 16-bit grayscale image
-        depth_image = np.array(depthframe)
-        height, width = depth_image.shape
-        min =  np.min(depth_image)
-        max =  np.max(depth_image)
-        print("max:"+str(max) +"  min:"+ str(min))
-        depth_frame_norm=0
-        fact=0
-        # Normalize the depth values between 0 and 255
-        print(height,width)
-        '''
-        if((max-min)>=0.50 and (max-min)<0.60):
-
-            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024
-        if((max-min)>=0.60 and (max-min)<0.70):
-
-            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024    
-
-        if((max-min)>=0.70 and (max-min)<0.80):
-
-            depth_frame_norm = (((depth_image - min) / max)*120) #225,2048,1024
-
-        if((max-min)>=0.80 and (max-min)<1):
-
-            depth_frame_norm = (((depth_image - min) / max)*150) #225,2048,1024
-    '''
-        if((max-min)>=0.1 and (max-min)<1):
-
-            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024
-            fact = 100
-        if((max-min)>=1):
-
-            depth_frame_norm = (((depth_image - min) / max)*200) #225,2048,1024
-            fact = 200
-        print (depth_image [320][400])
-        # Convert the depth frame to a color map
-        
-
-        # Save the depth map as a PNG image
-        cv2.imwrite("./"+filename + "/"+filename+'.png', depth_frame_norm)
-
-        '''    
-        depth_image = cv2.imread("./"+filename + "/"+filename+'.png',cv2.IMREAD_ANYDEPTH)
-        print(depth_image)
-        hole_mask = depth_image == 0
-        cv2.imwrite("./"+filename + "/"+filename+'_mask.png', hole_mask.astype(np.uint8)*255)
-
-        # Apply the inpainting algorithm
-        filled_depth = cv2.inpaint(depth_image, hole_mask.astype(np.uint8), 5, cv2.INPAINT_TELEA)
-
-        # Save the filled depth frame
-        cv2.imwrite("./"+filename + "/"+filename+ '_filled.png', filled_depth)
-        
-       #depth_image = filled_depth.astype(np.uint16)
-        
-        #depth_o3d = o3d.geometry.Image(depth_image)
-'''
-       # print(depth_o3d)
-        depth_image = iio.imread("./"+filename + "/"+filename+ '.png')
-        
-        
-        '''
-        # Create a depth image from the numpy array
-
-        intrinsic = o3d.camera.PinholeCameraIntrinsic(640, 480, 616.962, 616.962, 329.215, 237.106)
-        im = o3d.geometry.PointCloud.create_from_depth_image(depth_o3d,intrinsic)
-        '''
-        CX_DEPTH=322.282 # 322.282
-        CY_DEPTH = 322.282
-
-        FX_DEPTH=320.818 #320.818
-        FY_DEPTH=178.779 #178.779
-
-        pcd = []
-        height, width = depth_image.shape
-        for i in range(height):
-            for j in range(width):
-                z = depth_image[i][j]
-                x = (j - CX_DEPTH) * z / FX_DEPTH
-                y = (i - CY_DEPTH) * z / FY_DEPTH
-                pcd.append([x, y, z])
-        '''        
-        for i in range (100):
-             k=i
-             
-             if (i<200):
-                
-                pcd.append([0, 0, 2*i])
-             for j in range(100):
-                 t=j
-                 if(i%2):
-                     k= i*(-1)
-                 if(j%2):
-                     t= j*(-1)
-                 pcd.append([k, t, 0])
-       '''
-
-        pcd_o3d = o3d.geometry.PointCloud()  # create point cloud object
-        pcd_o3d.points = o3d.utility.Vector3dVector(pcd)  # set pcd_np as the point cloud points
-        # Visualize:
-        o3d.visualization.draw_geometries([pcd_o3d])
-        
-    
-        #s = verif.matrixDiagn(dp)
-
-        o3d.io.write_point_cloud("./"+filename + "/"+filename+".ply", pcd_o3d)
-        return min,max, fact
-
-
-
-
-
-
+import open3d as o3d
+import cv2
+import numpy as np
+import os 
+import imageio.v3 as iio
+
+class PointCloud:
+
+    def __init__(self) -> None:
+        pass
+
+    
+    def createPointCloud (self, depthframe, filename):
+
+
+      
+      
+        
+        os.makedirs(filename, exist_ok=True)
+        
+
+        # Load the depth frame as a 16-bit grayscale image
+        depth_image = np.array(depthframe)
+        height, width = depth_image.shape
+        min =  np.min(depth_image)
+        max =  np.max(depth_image)
+        print("max:"+str(max) +"  min:"+ str(min))
+        depth_frame_norm=0
+        fact=0
+        # Normalize the depth values between 0 and 255
+        print(height,width)
+        '''
+        if((max-min)>=0.50 and (max-min)<0.60):
+
+            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024
+        if((max-min)>=0.60 and (max-min)<0.70):
+
+            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024    
+
+        if((max-min)>=0.70 and (max-min)<0.80):
+
+            depth_frame_norm = (((depth_image - min) / max)*120) #225,2048,1024
+
+        if((max-min)>=0.80 and (max-min)<1):
+
+            depth_frame_norm = (((depth_image - min) / max)*150) #225,2048,1024
+    '''
+        if((max-min)>=0.1 and (max-min)<1):
+
+            depth_frame_norm = (((depth_image - min) / max)*100) #225,2048,1024
+            fact = 100
+        if((max-min)>=1):
+
+            depth_frame_norm = (((depth_image - min) / max)*200) #225,2048,1024
+            fact = 200
+        print (depth_image [320][400])
+        # Convert the depth frame to a color map
+        
+
+        # Save the depth map as a PNG image
+        cv2.imwrite("./"+filename + "/"+filename+'.png', depth_frame_norm)
+
+        '''    
+        depth_image = cv2.imread("./"+filename + "/"+filename+'.png',cv2.IMREAD_ANYDEPTH)
+        print(depth_image)
+        hole_mask = depth_image == 0
+        cv2.imwrite("./"+filename + "/"+filename+'_mask.png', hole_mask.astype(np.uint8)*255)
+
+        # Apply the inpainting algorithm
+        filled_depth = cv2.inpaint(depth_image, hole_mask.astype(np.uint8), 5, cv2.INPAINT_TELEA)
+
+        # Save the filled depth frame
+        cv2.imwrite("./"+filename + "/"+filename+ '_filled.png', filled_depth)
+        
+       #depth_image = filled_depth.astype(np.uint16)
+        
+        #depth_o3d = o3d.geometry.Image(depth_image)
+'''
+       # print(depth_o3d)
+        depth_image = iio.imread("./"+filename + "/"+filename+ '.png')
+        
+        
+        '''
+        # Create a depth image from the numpy array
+
+        intrinsic = o3d.camera.PinholeCameraIntrinsic(640, 480, 616.962, 616.962, 329.215, 237.106)
+        im = o3d.geometry.PointCloud.create_from_depth_image(depth_o3d,intrinsic)
+        '''
+        CX_DEPTH=322.282 # 322.282
+        CY_DEPTH = 322.282
+
+        FX_DEPTH=320.818 #320.818
+        FY_DEPTH=178.779 #178.779
+
+        pcd = []
+        height, width = depth_image.shape
+        for i in range(height):
+            for j in range(width):
+                z = depth_image[i][j]
+                x = (j - CX_DEPTH) * z / FX_DEPTH
+                y = (i - CY_DEPTH) * z / FY_DEPTH
+                pcd.append([x, y, z])
+        '''        
+        for i in range (100):
+             k=i
+             
+             if (i<200):
+                
+                pcd.append([0, 0, 2*i])
+             for j in range(100):
+                 t=j
+                 if(i%2):
+                     k= i*(-1)
+                 if(j%2):
+                     t= j*(-1)
+                 pcd.append([k, t, 0])
+       '''
+
+        pcd_o3d = o3d.geometry.PointCloud()  # create point cloud object
+        pcd_o3d.points = o3d.utility.Vector3dVector(pcd)  # set pcd_np as the point cloud points
+        # Visualize:
+        o3d.visualization.draw_geometries([pcd_o3d])
+        
+    
+        #s = verif.matrixDiagn(dp)
+
+        o3d.io.write_point_cloud("./"+filename + "/"+filename+".ply", pcd_o3d)
+        return min,max, fact
+
+
+
+
+
+
```

## hpverif/Segmentation.py

 * *Ordering differences only*

```diff
@@ -1,134 +1,134 @@
-import numpy as np
-import open3d as o3d
-import matplotlib.pyplot as plt
-import math
-
-
-class Segmentation:
-
-    def __init__(self,filename,min,max,fact) :
-        self.pcd =   o3d.io.read_point_cloud(filename)
-        #pcd =self.pcd.voxel_down_sample(voxel_size=0.02)  #down sampling por si imagen muy compleja
-        self.pcd.remove_statistical_outlier(nb_neighbors= 10, std_ratio=2.0)
-        o3d.visualization.draw_geometries([self.pcd]) 
-        self.min = min
-        self.max = max
-        self.fact = fact
-        #pcd.remove_radius_outlier(nb_points=16, radius=0.05) # esta eliminacion tarda mucho si la imagen tiene muchos puntos
-
-
-    def planeSegmentation(self):
-        
-        if ((self.max-self.min) > 1):
-            rest = 0.035 
-        else :
-            rest= 0.02
-
-        plane_model, inliers = self.pcd.segment_plane(distance_threshold=(((rest - self.min) / self.max)*self.fact), ransac_n=3,num_iterations=1000) #0.02. El q funcionaba bien era 0.008 #3
-        [a, b, c, d] = plane_model
-        print(f"Plane equation: {a:.2f}x + {b:.2f}y + {c:.2f}z + {d:.2f} = 0")
-        theta = (math.acos(abs(c) / math.sqrt(a**2 + b**2 + c**2)))*180/math.pi
-        print(f"theta:{theta:.2f}")
-        inlier_cloud = self.pcd.select_by_index(inliers)
-        inlier_cloud.paint_uniform_color([1.0, 0, 0])
-        outlier_cloud = self.pcd.select_by_index(inliers, invert=True)     
-        o3d.visualization.draw_geometries([inlier_cloud, outlier_cloud])  
-        self.pcd = outlier_cloud
-
-        depth_values_plane= np.asarray(inlier_cloud.points)[:,2] 
-        depth_value_plane= ((np.mean(depth_values_plane)/self.fact)*self.max)+self.min
-        print("distancia pared final: " + str(depth_value_plane))
-
-
-        plane_model, inliers = self.pcd.segment_plane(distance_threshold=(((0.015 - self.min) / self.max)*self.fact), ransac_n=3,num_iterations=1000) #2.8
-        [a, b, c, d] = plane_model
-        print(f"Plane equation: {a:.2f}x + {b:.2f}y + {c:.2f}z + {d:.2f} = 0")
-        inlier_cloud = self.pcd.select_by_index(inliers)
-        outlier_cloud = self.pcd.select_by_index(inliers, invert=True) 
-        inlier_cloud.paint_uniform_color([1.0, 0, 0])
-        outlier_cloud.paint_uniform_color([1.0, 0, 0])
-        o3d.visualization.draw_geometries([inlier_cloud]) 
-        o3d.visualization.draw_geometries([outlier_cloud]) 
-        pcd = outlier_cloud
-
-        depth_values_obj= np.asarray(inlier_cloud.points)[:,2] 
-        depth_value_obj= ((np.mean(depth_values_obj)/self.fact)*self.max)+self.min
-        if(theta < 8):
-            print("distancia segundo objeto plano/suelo: " + str(depth_value_obj))
-        else:
-            print("distancia suelo: " + str(depth_value_obj))
-
-        return depth_value_plane,depth_value_obj, theta
-
-        
-
-
-
-    def segmentation(self):   
-
-        with o3d.utility.VerbosityContextManager(
-            o3d.utility.VerbosityLevel.Debug) as cm:
-            labels = np.array(
-                self.pcd.cluster_dbscan(eps=(((0.03 - self.min) / self.max)*self.fact), min_points=50, print_progress=True)) # inclinado: 3.2, y min_p=50.     1.8
-
-        max_label = labels.max()
-        print(f"point cloud has {max_label + 1} clusters")
-        colors = plt.get_cmap("tab20")(labels / (max_label if max_label > 0 else 1))
-        colors[labels < 0] = 0
-        self.pcd.colors = o3d.utility.Vector3dVector(colors[:, :3])
-        o3d.visualization.draw_geometries([self.pcd])
-
-
-    
-        #Buscamos la region que nos interesa
-        target_label= 0
-        selected_indices = np.where(labels == target_label)[0]
-        selected_pcd = self.pcd.select_by_index(selected_indices)
-        max_pcd= selected_pcd
-
-
-        for i in range(max_label):
-            target_label = i
-            if(target_label> 0):
-                selected_indices = np.where(labels == target_label)[0]
-                selected_pcd = self.pcd.select_by_index(selected_indices)
-
-                if(i==1):
-                    max2_pcd= selected_pcd
-            
-                if( len(selected_pcd.points) > len(max2_pcd.points) ):
-                    max2_pcd = selected_pcd
-
-                if( len(selected_pcd.points)> len(max_pcd.points)):  # np.asarray(selected_pcd.points).size> np.asarray(max_pcd.points).size
-                    max2_pcd = max_pcd
-                    max_pcd= selected_pcd
-                
-        o3d.visualization.draw_geometries([max_pcd])
-        o3d.visualization.draw_geometries([max2_pcd])
-        max_points = np.asarray(max_pcd.points)
-        max_points2 = np.asarray(max2_pcd.points)
-
-        print("varianza:" + str(np.var(max_points2[:,2])))
-
-        print("varianza:" + str(np.var(max_points[:,2])))
-
-        ''' 
-        if( (np.var(max_points[:,2]) <= np.var(max_points[:,2]) +1.2*np.var(max_points2[:,2]))):
-            pcd_final = max_pcd
-        elif(np.var(max_points2[:,2])<0.8*np.var(max_points[:,2]) ):
-            pcd_final = max2_pcd
-        else:
-            pcd_final= max_pcd
-        '''
-        if(np.var(max_points2[:,2])<np.var(max_points2[:,2])):
-            pcd_final=max2_pcd
-        else:
-            pcd_final=max_pcd
-
-
-        o3d.visualization.draw_geometries([pcd_final])
-
-        depth_values_obj= np.asarray(pcd_final.points)[:,2] 
-        depth_value_plane= ((np.mean(depth_values_obj)/self.fact)*self.max)+self.min
-        print("distancia objeto inclinado: " + str(depth_value_plane))
+import numpy as np
+import open3d as o3d
+import matplotlib.pyplot as plt
+import math
+
+
+class Segmentation:
+
+    def __init__(self,filename,min,max,fact) :
+        self.pcd =   o3d.io.read_point_cloud(filename)
+        #pcd =self.pcd.voxel_down_sample(voxel_size=0.02)  #down sampling por si imagen muy compleja
+        self.pcd.remove_statistical_outlier(nb_neighbors= 10, std_ratio=2.0)
+        o3d.visualization.draw_geometries([self.pcd]) 
+        self.min = min
+        self.max = max
+        self.fact = fact
+        #pcd.remove_radius_outlier(nb_points=16, radius=0.05) # esta eliminacion tarda mucho si la imagen tiene muchos puntos
+
+
+    def planeSegmentation(self):
+        
+        if ((self.max-self.min) > 1):
+            rest = 0.035 
+        else :
+            rest= 0.02
+
+        plane_model, inliers = self.pcd.segment_plane(distance_threshold=(((rest - self.min) / self.max)*self.fact), ransac_n=3,num_iterations=1000) #0.02. El q funcionaba bien era 0.008 #3
+        [a, b, c, d] = plane_model
+        print(f"Plane equation: {a:.2f}x + {b:.2f}y + {c:.2f}z + {d:.2f} = 0")
+        theta = (math.acos(abs(c) / math.sqrt(a**2 + b**2 + c**2)))*180/math.pi
+        print(f"theta:{theta:.2f}")
+        inlier_cloud = self.pcd.select_by_index(inliers)
+        inlier_cloud.paint_uniform_color([1.0, 0, 0])
+        outlier_cloud = self.pcd.select_by_index(inliers, invert=True)     
+        o3d.visualization.draw_geometries([inlier_cloud, outlier_cloud])  
+        self.pcd = outlier_cloud
+
+        depth_values_plane= np.asarray(inlier_cloud.points)[:,2] 
+        depth_value_plane= ((np.mean(depth_values_plane)/self.fact)*self.max)+self.min
+        print("distancia pared final: " + str(depth_value_plane))
+
+
+        plane_model, inliers = self.pcd.segment_plane(distance_threshold=(((0.015 - self.min) / self.max)*self.fact), ransac_n=3,num_iterations=1000) #2.8
+        [a, b, c, d] = plane_model
+        print(f"Plane equation: {a:.2f}x + {b:.2f}y + {c:.2f}z + {d:.2f} = 0")
+        inlier_cloud = self.pcd.select_by_index(inliers)
+        outlier_cloud = self.pcd.select_by_index(inliers, invert=True) 
+        inlier_cloud.paint_uniform_color([1.0, 0, 0])
+        outlier_cloud.paint_uniform_color([1.0, 0, 0])
+        o3d.visualization.draw_geometries([inlier_cloud]) 
+        o3d.visualization.draw_geometries([outlier_cloud]) 
+        pcd = outlier_cloud
+
+        depth_values_obj= np.asarray(inlier_cloud.points)[:,2] 
+        depth_value_obj= ((np.mean(depth_values_obj)/self.fact)*self.max)+self.min
+        if(theta < 8):
+            print("distancia segundo objeto plano/suelo: " + str(depth_value_obj))
+        else:
+            print("distancia suelo: " + str(depth_value_obj))
+
+        return depth_value_plane,depth_value_obj, theta
+
+        
+
+
+
+    def segmentation(self):   
+
+        with o3d.utility.VerbosityContextManager(
+            o3d.utility.VerbosityLevel.Debug) as cm:
+            labels = np.array(
+                self.pcd.cluster_dbscan(eps=(((0.03 - self.min) / self.max)*self.fact), min_points=50, print_progress=True)) # inclinado: 3.2, y min_p=50.     1.8
+
+        max_label = labels.max()
+        print(f"point cloud has {max_label + 1} clusters")
+        colors = plt.get_cmap("tab20")(labels / (max_label if max_label > 0 else 1))
+        colors[labels < 0] = 0
+        self.pcd.colors = o3d.utility.Vector3dVector(colors[:, :3])
+        o3d.visualization.draw_geometries([self.pcd])
+
+
+    
+        #Buscamos la region que nos interesa
+        target_label= 0
+        selected_indices = np.where(labels == target_label)[0]
+        selected_pcd = self.pcd.select_by_index(selected_indices)
+        max_pcd= selected_pcd
+
+
+        for i in range(max_label):
+            target_label = i
+            if(target_label> 0):
+                selected_indices = np.where(labels == target_label)[0]
+                selected_pcd = self.pcd.select_by_index(selected_indices)
+
+                if(i==1):
+                    max2_pcd= selected_pcd
+            
+                if( len(selected_pcd.points) > len(max2_pcd.points) ):
+                    max2_pcd = selected_pcd
+
+                if( len(selected_pcd.points)> len(max_pcd.points)):  # np.asarray(selected_pcd.points).size> np.asarray(max_pcd.points).size
+                    max2_pcd = max_pcd
+                    max_pcd= selected_pcd
+                
+        o3d.visualization.draw_geometries([max_pcd])
+        o3d.visualization.draw_geometries([max2_pcd])
+        max_points = np.asarray(max_pcd.points)
+        max_points2 = np.asarray(max2_pcd.points)
+
+        print("varianza:" + str(np.var(max_points2[:,2])))
+
+        print("varianza:" + str(np.var(max_points[:,2])))
+
+        ''' 
+        if( (np.var(max_points[:,2]) <= np.var(max_points[:,2]) +1.2*np.var(max_points2[:,2]))):
+            pcd_final = max_pcd
+        elif(np.var(max_points2[:,2])<0.8*np.var(max_points[:,2]) ):
+            pcd_final = max2_pcd
+        else:
+            pcd_final= max_pcd
+        '''
+        if(np.var(max_points2[:,2])<np.var(max_points2[:,2])):
+            pcd_final=max2_pcd
+        else:
+            pcd_final=max_pcd
+
+
+        o3d.visualization.draw_geometries([pcd_final])
+
+        depth_values_obj= np.asarray(pcd_final.points)[:,2] 
+        depth_value_plane= ((np.mean(depth_values_obj)/self.fact)*self.max)+self.min
+        print("distancia objeto inclinado: " + str(depth_value_plane))
         return depth_value_plane
```

## hpverif/ShowFiles.py

 * *Ordering differences only*

```diff
@@ -1,75 +1,75 @@
-import cv2                                # state of the art computer vision algorithms library
-import numpy as np                        # fundamental package for scientific computing
-import pyrealsense2 as rs  
-
-
-
-
-class Show_Files:
-   
-    def __init__ (self):
-        self.pipeline = rs.pipeline()
-        self.config = rs.config()
-        self.pc = rs.pointcloud()
-
-
-
-
-    def enable_file (self, file):
-         
-
-        rs.config.enable_device_from_file(self.config , file)
-        self.config.enable_stream(rs.stream.depth, rs.format.z16, 30)
-        self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
-        
-        profile = self.pipeline.start(self.config)
-
-
-
-    def show (self, frame):
-
-        cv2.namedWindow("Depth Stream", cv2.WINDOW_AUTOSIZE)
-  
-        pointcloud=rs.pointcloud()
-       
-
-        # Create colorizer object
-        colorizer = rs.colorizer()
-        iter = 0
-            # Streaming loop
-        while True:
-                iter = iter + 1
-                # Get frameset of depth
-                frames = self.pipeline.wait_for_frames()
-
-                # Get depth frame
-                depth_frame = frames.get_depth_frame()
-                color_frame = frames.get_color_frame()
-
-                #points = pointcloud.calculate(depth_frame)
-
-                #verts = np.asarray(points.get_vertices())
-                #rgbs = np.asarray(color_frame.get_data())
-                #pcd = o3d.geometry.PointCloud()
-                #pcd.points = o3d.utility.Vector3dVector(verts)
-                #pcd.colors = o3d.utility.Vector3dVector(rgbs)
-
-                 # Visualizar el pointcloud
-                #o3d.visualization.draw_geometries([pcd])
-
-                if(iter == frame-6):
-                     final_depth = depth_frame
-                     final_rgb = color_frame 
-                # Colorize depth frame to jet colormap
-                depth_color_frame = colorizer.colorize(depth_frame)
-
-                # Convert depth_frame to numpy array to render image in opencv
-                depth_color_image = np.asanyarray(depth_color_frame.get_data())
-
-                # Render image in opencv window
-                cv2.imshow("Depth Stream", depth_color_image)
-                key = cv2.waitKey(1)
-                # if pressed escape exit program
-                if key == 27:
-                    cv2.destroyAllWindows()
+import cv2                                # state of the art computer vision algorithms library
+import numpy as np                        # fundamental package for scientific computing
+import pyrealsense2 as rs  
+
+
+
+
+class Show_Files:
+   
+    def __init__ (self):
+        self.pipeline = rs.pipeline()
+        self.config = rs.config()
+        self.pc = rs.pointcloud()
+
+
+
+
+    def enable_file (self, file):
+         
+
+        rs.config.enable_device_from_file(self.config , file)
+        self.config.enable_stream(rs.stream.depth, rs.format.z16, 30)
+        self.config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
+        
+        profile = self.pipeline.start(self.config)
+
+
+
+    def show (self, frame):
+
+        cv2.namedWindow("Depth Stream", cv2.WINDOW_AUTOSIZE)
+  
+        pointcloud=rs.pointcloud()
+       
+
+        # Create colorizer object
+        colorizer = rs.colorizer()
+        iter = 0
+            # Streaming loop
+        while True:
+                iter = iter + 1
+                # Get frameset of depth
+                frames = self.pipeline.wait_for_frames()
+
+                # Get depth frame
+                depth_frame = frames.get_depth_frame()
+                color_frame = frames.get_color_frame()
+
+                #points = pointcloud.calculate(depth_frame)
+
+                #verts = np.asarray(points.get_vertices())
+                #rgbs = np.asarray(color_frame.get_data())
+                #pcd = o3d.geometry.PointCloud()
+                #pcd.points = o3d.utility.Vector3dVector(verts)
+                #pcd.colors = o3d.utility.Vector3dVector(rgbs)
+
+                 # Visualizar el pointcloud
+                #o3d.visualization.draw_geometries([pcd])
+
+                if(iter == frame-6):
+                     final_depth = depth_frame
+                     final_rgb = color_frame 
+                # Colorize depth frame to jet colormap
+                depth_color_frame = colorizer.colorize(depth_frame)
+
+                # Convert depth_frame to numpy array to render image in opencv
+                depth_color_image = np.asanyarray(depth_color_frame.get_data())
+
+                # Render image in opencv window
+                cv2.imshow("Depth Stream", depth_color_image)
+                key = cv2.waitKey(1)
+                # if pressed escape exit program
+                if key == 27:
+                    cv2.destroyAllWindows()
                     return final_depth, final_rgb, self.pc
```

## hpverif/Theoretical_distance.py

 * *Ordering differences only*

```diff
@@ -1,126 +1,126 @@
-import matplotlib.pyplot as plt
-import math
-import ast
-
-class Theoretical_distance:
-
-    def __init__ (self):
-        pass
-
-    def theoric_distance(self, mapa, point, angle_degrees, show):
-        #Carreguem mapa
-        lines = self.loadMap(mapa)
-
-        # Definim posició i angles (graus)
-        #point, angle_degrees = (150, 100), 30
-
-        #Ample de visió de la càmara d435i
-        angle_FOV = 86/2
-
-        #Calculem distancia central
-        dist, interseccio_paret = self.distancia_propera(point, angle_degrees, lines)
-
-        #Camp de visió càmara
-        FOV_right, interseccio_paret_right = self.distancia_propera(point, angle_degrees - angle_FOV, lines)
-        FOV_left, interseccio_paret_left = self.distancia_propera(point, angle_degrees + angle_FOV, lines)
-
-
-        #--------------------< REPRESENTACIÓ >--------------------
-        if(show):
-            #Creem mapa
-            fig, ax = plt.subplots()
-            # Setejem la nostra posició
-            ax.scatter(point[0],point[1], label=f'Camera location: {(point[0], point[1])}' + ' cm.', color='blue', marker='o', s=30)
-            # Graficar mapa
-            for i in range(len(lines)):
-                x1, y1 = lines[i][0][0], lines[i][0][1]
-                x2, y2 = lines[i][1][0], lines[i][1][1]
-                ax.plot([x1, x2], [y1, y2], 'k-')
-
-            #Mostrem distancia  
-            ax.plot([point[0],interseccio_paret[0]], [point[1],interseccio_paret[1]], 'g-', label=f'Central distance: {round(dist, 3)}' + ' cm.')
-
-            #Mostrem rang de visió de la càmara
-            ax.plot([point[0],interseccio_paret_right[0]], [point[1],interseccio_paret_right[1]], 'r-', label=f'Field of view.')
-            ax.plot([point[0],interseccio_paret_left[0]], [point[1],interseccio_paret_left[1]], 'r-')
-
-            ax.legend(loc='upper left')
-
-            #Redimensionar finestra
-            ax.set_aspect('equal')
-
-            plt.title('Distance between HP SitePrint and the objective')
-            plt.xlabel('X Axis (cm)')
-            plt.ylabel('Y Axis (cm)')
-
-            #Establim valor de la distància teòrica
-            plt.text(interseccio_paret[0], interseccio_paret[1], f"{round(dist, 3)}" + " cm", ha='right', va='bottom')
-            plt.text(point[0], point[1], f"{(point[0], point[1])}" + " cm  ", ha='right', va='bottom')
-
-
-            plt.show()
-
-        return dist
-    
-    def line_intersection(self, line1, line2):
-        x1, y1 = line1[0]
-        x2, y2 = line1[1]
-        x3, y3 = line2[0]
-        x4, y4 = line2[1]
-        det = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4)
-        
-        if det == 0:
-            return (-1,-1) #si no hi ha interseccio
-        else:
-            px = ((x1*y2 - y1*x2)*(x3 - x4) - (x1 - x2)*(x3*y4 - y3*x4)) / det
-            py = ((x1*y2 - y1*x2)*(y3 - y4) - (y1 - y2)*(x3*y4 - y3*x4)) / det
-            if (x1-1 <= px<= x2+1 or x1+1>=px>=x2-1)and(y1-1<=py<=y2+1 or y1+1>=py>=y2-1) and (x3-1 <= px <= x4+1 or x3+1>=px>=x4-1)and(y3-1<=py<=y4+1 or y3+1>=py>=y4-1):
-                return (px, py)
-            else:
-                return(-1,-1)
-
-    def distance_between_points(self, point1, point2):
-        x1, y1 = point1
-        x2, y2 = point2
-        return math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
-
-    def loadMap(self, map_name):
-        if '.txt' in map_name:
-            map_name = map_name.replace(".txt", "")
-        with open(map_name + '.txt', 'r') as file:
-            lines = file.readlines()
-            #Assignem a un vector els valors de archiu
-            lines_strip = [line.strip() for line in lines]
-            #Separem les coordenades dels punts per poder-hi accedir posteriorment
-            lines_clean = [ast.literal_eval(linea) for linea in lines_strip]
-            
-            return lines_clean
-        
-    def distancia_propera(self, point, angle_degrees, lines):  
-
-        # Convert the angle to radians
-        angle_radians = (angle_degrees*math.pi)/180
-
-        # Calculate the coordinates of the end point of the ray
-        dx = 1000 * math.cos(angle_radians)
-        dy = 1000 * math.sin(angle_radians)
-        ray_end = (point[0] + dx, point[1] + dy)
-
-        # Check which line the ray intersects with
-        intersection_points = []
-        for line in lines:
-            intersection_point = self.line_intersection((point, ray_end), line)
-            
-            if intersection_point[0] >= 0 and intersection_point[1] >= 0:
-                intersection_points.append(intersection_point)
-
-        # Find the closest intersection point to the point
-        closest_intersection_point = None
-        closest_distance = float("inf")
-        for p in intersection_points:
-            distance = self.distance_between_points(p, point)
-            if distance < closest_distance:
-                closest_intersection_point = p
-                closest_distance = distance
-
+import matplotlib.pyplot as plt
+import math
+import ast
+
+class Theoretical_distance:
+
+    def __init__ (self):
+        pass
+
+    def theoric_distance(self, mapa, point, angle_degrees, show):
+        #Carreguem mapa
+        lines = self.loadMap(mapa)
+
+        # Definim posició i angles (graus)
+        #point, angle_degrees = (150, 100), 30
+
+        #Ample de visió de la càmara d435i
+        angle_FOV = 86/2
+
+        #Calculem distancia central
+        dist, interseccio_paret = self.distancia_propera(point, angle_degrees, lines)
+
+        #Camp de visió càmara
+        FOV_right, interseccio_paret_right = self.distancia_propera(point, angle_degrees - angle_FOV, lines)
+        FOV_left, interseccio_paret_left = self.distancia_propera(point, angle_degrees + angle_FOV, lines)
+
+
+        #--------------------< REPRESENTACIÓ >--------------------
+        if(show):
+            #Creem mapa
+            fig, ax = plt.subplots()
+            # Setejem la nostra posició
+            ax.scatter(point[0],point[1], label=f'Camera location: {(point[0], point[1])}' + ' cm.', color='blue', marker='o', s=30)
+            # Graficar mapa
+            for i in range(len(lines)):
+                x1, y1 = lines[i][0][0], lines[i][0][1]
+                x2, y2 = lines[i][1][0], lines[i][1][1]
+                ax.plot([x1, x2], [y1, y2], 'k-')
+
+            #Mostrem distancia  
+            ax.plot([point[0],interseccio_paret[0]], [point[1],interseccio_paret[1]], 'g-', label=f'Central distance: {round(dist, 3)}' + ' cm.')
+
+            #Mostrem rang de visió de la càmara
+            ax.plot([point[0],interseccio_paret_right[0]], [point[1],interseccio_paret_right[1]], 'r-', label=f'Field of view.')
+            ax.plot([point[0],interseccio_paret_left[0]], [point[1],interseccio_paret_left[1]], 'r-')
+
+            ax.legend(loc='upper left')
+
+            #Redimensionar finestra
+            ax.set_aspect('equal')
+
+            plt.title('Distance between HP SitePrint and the objective')
+            plt.xlabel('X Axis (cm)')
+            plt.ylabel('Y Axis (cm)')
+
+            #Establim valor de la distància teòrica
+            plt.text(interseccio_paret[0], interseccio_paret[1], f"{round(dist, 3)}" + " cm", ha='right', va='bottom')
+            plt.text(point[0], point[1], f"{(point[0], point[1])}" + " cm  ", ha='right', va='bottom')
+
+
+            plt.show()
+
+        return dist
+    
+    def line_intersection(self, line1, line2):
+        x1, y1 = line1[0]
+        x2, y2 = line1[1]
+        x3, y3 = line2[0]
+        x4, y4 = line2[1]
+        det = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4)
+        
+        if det == 0:
+            return (-1,-1) #si no hi ha interseccio
+        else:
+            px = ((x1*y2 - y1*x2)*(x3 - x4) - (x1 - x2)*(x3*y4 - y3*x4)) / det
+            py = ((x1*y2 - y1*x2)*(y3 - y4) - (y1 - y2)*(x3*y4 - y3*x4)) / det
+            if (x1-1 <= px<= x2+1 or x1+1>=px>=x2-1)and(y1-1<=py<=y2+1 or y1+1>=py>=y2-1) and (x3-1 <= px <= x4+1 or x3+1>=px>=x4-1)and(y3-1<=py<=y4+1 or y3+1>=py>=y4-1):
+                return (px, py)
+            else:
+                return(-1,-1)
+
+    def distance_between_points(self, point1, point2):
+        x1, y1 = point1
+        x2, y2 = point2
+        return math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
+
+    def loadMap(self, map_name):
+        if '.txt' in map_name:
+            map_name = map_name.replace(".txt", "")
+        with open(map_name + '.txt', 'r') as file:
+            lines = file.readlines()
+            #Assignem a un vector els valors de archiu
+            lines_strip = [line.strip() for line in lines]
+            #Separem les coordenades dels punts per poder-hi accedir posteriorment
+            lines_clean = [ast.literal_eval(linea) for linea in lines_strip]
+            
+            return lines_clean
+        
+    def distancia_propera(self, point, angle_degrees, lines):  
+
+        # Convert the angle to radians
+        angle_radians = (angle_degrees*math.pi)/180
+
+        # Calculate the coordinates of the end point of the ray
+        dx = 1000 * math.cos(angle_radians)
+        dy = 1000 * math.sin(angle_radians)
+        ray_end = (point[0] + dx, point[1] + dy)
+
+        # Check which line the ray intersects with
+        intersection_points = []
+        for line in lines:
+            intersection_point = self.line_intersection((point, ray_end), line)
+            
+            if intersection_point[0] >= 0 and intersection_point[1] >= 0:
+                intersection_points.append(intersection_point)
+
+        # Find the closest intersection point to the point
+        closest_intersection_point = None
+        closest_distance = float("inf")
+        for p in intersection_points:
+            distance = self.distance_between_points(p, point)
+            if distance < closest_distance:
+                closest_intersection_point = p
+                closest_distance = distance
+
         return(closest_distance, closest_intersection_point)
```

## hpverif/Verification.py

```diff
@@ -1,59 +1,59 @@
-from .Calibraton import Calibration
-from .FrameCapture import Frame_Capture
-from .ShowFiles import Show_Files
-from .FrameCapturePLY import Frame_Capture_PLY
-from .PointCloud import PointCloud
-from .Segmentation import Segmentation
-import numpy as np
-from .Theoretical_distance import Theoretical_distance as dt
-
-
-class Verification:
-    def __init__ (self):
-        pass
-
-    
-    def calibration(self):
-        calibrate = Calibration()
-        calibrate.enable_stream()
-        calibrate.calibrate()
-
-
-    def capture_frame(self,frames, filename, high):
-        frame_capture = Frame_Capture()
-        frame_capture.get_and_configure_device(high)
-        return frame_capture.capture(frames, filename, high)
-    
-    def capture_frame_ply(self,filename, high):
-        frame_capture = Frame_Capture_PLY()
-        frame_capture.get_and_configure_device()
-        frame_capture.capture(filename, high)
-
-    def show_files(self, frame,  filename):
-        show = Show_Files()
-        show.enable_file(filename)
-        return show.show(frame)
-    
-    #def kmeans (self,matrix, k):
-      #  km = Kmeans()
-       # km.CalculateKMeans(matrix, k)
-    
-    def pointCloud (self, dp, filename):
-        pc = PointCloud()
-        return pc.createPointCloud(0.001*np.asanyarray(dp.get_data()),filename)
-        
-    
-    def segmentation (self, filename, min, max , fact):
-        seg = Segmentation(filename,min,max,fact)
-        dist_pared, dist_obj_plane, theta=seg.planeSegmentation()
-        dist_obj_incline=0
-        if(theta>8):
-            dist_obj_incline= seg.segmentation()
-        return dist_pared,dist_obj_plane, dist_obj_incline
-    
-
-    def dist_teorica(self, mapa, point, angle_degrees, show):
-        d = dt.Theoretical_distance()
-        dist = d.theoric_distance(mapa, point, angle_degrees,show)
-        print("Distància teorica: " + str(dist))
+from .Calibraton import Calibration
+from .FrameCapture import Frame_Capture
+from .ShowFiles import Show_Files
+from .FrameCapturePLY import Frame_Capture_PLY
+from .PointCloud import PointCloud
+from .Segmentation import Segmentation
+from .Theoretical_distance import Theoretical_distance 
+import numpy as np
+
+
+class Verification:
+    def __init__ (self):
+        pass
+
+    
+    def calibration(self):
+        calibrate = Calibration()
+        calibrate.enable_stream()
+        calibrate.calibrate()
+
+
+    def capture_frame(self,frames, filename, high):
+        frame_capture = Frame_Capture()
+        frame_capture.get_and_configure_device(high)
+        return frame_capture.capture(frames, filename, high)
+    
+    def capture_frame_ply(self,filename, high):
+        frame_capture = Frame_Capture_PLY()
+        frame_capture.get_and_configure_device()
+        frame_capture.capture(filename, high)
+
+    def show_files(self, frame,  filename):
+        show = Show_Files()
+        show.enable_file(filename)
+        return show.show(frame)
+    
+    #def kmeans (self,matrix, k):
+      #  km = Kmeans()
+       # km.CalculateKMeans(matrix, k)
+    
+    def pointCloud (self, dp, filename):
+        pc = PointCloud()
+        return pc.createPointCloud(0.001*np.asanyarray(dp.get_data()),filename)
+        
+    
+    def segmentation (self, filename, min, max , fact):
+        seg = Segmentation(filename,min,max,fact)
+        dist_pared, dist_obj_plane, theta=seg.planeSegmentation()
+        dist_obj_incline=0
+        if(theta>8):
+            dist_obj_incline= seg.segmentation()
+        return dist_pared,dist_obj_plane, dist_obj_incline
+    
+
+    def dist_teorica(self, mapa, point, angle_degrees, show):
+        d = Theoretical_distance()
+        dist = d.theoric_distance(mapa, point, angle_degrees,show)
+        print("Distància teorica: " + str(dist))
         return dist
```

## hpverif/driver.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-import Verification  as v
-
-
-
-verif = v.Verification()
-#dp,dc = verif.capture_frame(100, "prueba3m.bag", 0)
-
-
-       
-dp,dc,p = verif.show_files(26,'prueba_estatica2.bag')
-min,max,fact= verif.pointCloud(dp,'prueba_estatica2')
-
-dist1,dist2,dist3=verif.segmentation("./prueba_estatica2/prueba_estatica2.ply",min,max, fact)
-
-print(".................")
-print(dist1)
-print(dist2)
-print(dist3)
-
-
+import Verification  as v
+
+
+
+verif = v.Verification()
+#dp,dc = verif.capture_frame(100, "prueba3m.bag", 0)
+
+
+       
+dp,dc,p = verif.show_files(26,'prueba_estatica2.bag')
+min,max,fact= verif.pointCloud(dp,'prueba_estatica2')
+
+dist1,dist2,dist3=verif.segmentation("./prueba_estatica2/prueba_estatica2.ply",min,max, fact)
+
+print(".................")
+print(dist1)
+print(dist2)
+print(dist3)
+
+
```

