# Comparing `tmp/oakutils-0.0.2.tar.gz` & `tmp/oakutils-0.0.3.tar.gz`

## Comparing `oakutils-0.0.2.tar` & `oakutils-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,49 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 oakutils-0.0.2/Makefile
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 oakutils-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 oakutils-0.0.2/.github/workflows/build-check.yaml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 oakutils-0.0.2/.github/workflows/release-publish.yaml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 oakutils-0.0.2/examples/calibration.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oakutils-0.0.2/examples/camera.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 oakutils-0.0.2/examples/point_cloud.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 oakutils-0.0.2/scripts/update_version.sh
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/__init__.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/camera.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/calibration/__init__.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/calibration/_classes.py
--rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/calibration/_funcs.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/point_clouds/__init__.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/point_clouds/_classes.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 oakutils-0.0.2/src/oakutils/point_clouds/_funcs.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 oakutils-0.0.2/tests/camera.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 oakutils-0.0.2/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 oakutils-0.0.2/LICENSE
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 oakutils-0.0.2/README.md
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 oakutils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 oakutils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 oakutils-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 oakutils-0.0.3/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 oakutils-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 oakutils-0.0.3/.github/workflows/build-check.yaml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 oakutils-0.0.3/.github/workflows/release-publish.yaml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 oakutils-0.0.3/.github/workflows/test-publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oakutils-0.0.3/blobs/generate.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 oakutils-0.0.3/blobs/definitions/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 oakutils-0.0.3/blobs/definitions/gaussian.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 oakutils-0.0.3/blobs/definitions/laplacian.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/api.rst
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/usage.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/source/oakutils.calibration.rst
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/source/oakutils.point_clouds.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 oakutils-0.0.3/docs/source/oakutils.rst
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 oakutils-0.0.3/examples/calibration.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 oakutils-0.0.3/examples/camera.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 oakutils-0.0.3/examples/point_cloud.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 oakutils-0.0.3/scripts/update_version.sh
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/__init__.py
+-rw-r--r--   0        0        0    29935 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/camera.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/calibration/__init__.py
+-rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/calibration/_classes.py
+-rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/calibration/_funcs.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/__init__.py
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/color_camera.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/image_manip.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/imu.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/mono_camera.py
+-rw-r--r--   0        0        0    19274 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/nodes/stereo_depth.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/point_clouds/__init__.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/point_clouds/_classes.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/point_clouds/_funcs.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/tools/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 oakutils-0.0.3/src/oakutils/tools/parsing.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 oakutils-0.0.3/tests/camera.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 oakutils-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 oakutils-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 oakutils-0.0.3/README.md
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 oakutils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 oakutils-0.0.3/PKG-INFO
```

### Comparing `oakutils-0.0.2/examples/calibration.py` & `oakutils-0.0.3/examples/calibration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from oakutils.calibration import create_camera_calibration
-
-# Create a CalibrationData object for the camera
-# create_camera_calibration requires an open device through depthai
-# this function will also pre-create the primary mono camera
-calibration = create_camera_calibration(
-    rgb_size=(1920, 1080),
-    mono_size=(640, 400),
-    is_primary_mono_left=True,
-)
-
-# print out the K matrices
-print(f"K matrix for rgb: {calibration.rgb.K}")
-print(f"K matrix for left: {calibration.left.K}")
-print(f"K matrix for right: {calibration.right.K}")
-print(f"K matrix for primary: {calibration.primary.K}")
-
-# print out the distortion coefficients
-print(f"Distortion coefficients for rgb: {calibration.rgb.D}")
-print(f"Distortion coefficients for left: {calibration.left.D}")
-print(f"Distortion coefficients for right: {calibration.right.D}")
-print(f"Distortion coefficients for primary: {calibration.primary.D}")
-
-# print out the stereo information
-print(f"Q matrix: {calibration.stereo.cv2_Q}")
+from oakutils.calibration import get_camera_calibration
+
+# Create a CalibrationData object for the camera
+# create_camera_calibration requires an open device through depthai
+# this function will also pre-create the primary mono camera
+calibration = get_camera_calibration(
+    rgb_size=(1920, 1080),
+    mono_size=(640, 400),
+    is_primary_mono_left=True,
+)
+
+# print out the K matrices
+print(f"K matrix for rgb: {calibration.rgb.K}")
+print(f"K matrix for left: {calibration.left.K}")
+print(f"K matrix for right: {calibration.right.K}")
+print(f"K matrix for primary: {calibration.primary.K}")
+
+# print out the distortion coefficients
+print(f"Distortion coefficients for rgb: {calibration.rgb.D}")
+print(f"Distortion coefficients for left: {calibration.left.D}")
+print(f"Distortion coefficients for right: {calibration.right.D}")
+print(f"Distortion coefficients for primary: {calibration.primary.D}")
+
+# print out the stereo information
+print(f"Q matrix: {calibration.stereo.cv2_Q}")
+print(f"Manual Left Q matrix: {calibration.stereo.Q_left}")
+print(f"Manual Right Q matrix: {calibration.stereo.Q_right}")
```

### Comparing `oakutils-0.0.2/examples/camera.py` & `oakutils-0.0.3/examples/camera.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Simple example of using the Camera class to display the output of the OAK-D camera
-import time
-
-import cv2
-from oakutils import Camera
-
-
-DISPLAY_TIME = 10
-
-cam = Camera(
-    display_depth=True,
-    display_mono=True,
-    display_rectified=True,
-    compute_im3d_on_demand=True,  # on demand, so must call compute_im3d to update
-)
-
-cam.start_display()
-cam.start()
-
-start_time = time.time()
-while True:
-    if time.time() - start_time > DISPLAY_TIME:
-        break
-
-    cam.compute_im3d(block=True)
-    cv2.imshow("im3d", cam.im3d)
-    cv2.waitKey(1)
-
-    time.sleep(0.05)
-
-cam.stop()
+# Simple example of using the Camera class to display the output of the OAK-D camera
+import time
+
+import cv2
+from oakutils import Camera
+
+
+DISPLAY_TIME = 10
+
+cam = Camera(
+    display_depth=True,
+    display_mono=True,
+    display_rectified=True,
+    compute_im3d_on_demand=True,  # on demand, so must call compute_im3d to update
+)
+
+cam.start_display()
+cam.start()
+
+start_time = time.time()
+while True:
+    if time.time() - start_time > DISPLAY_TIME:
+        break
+
+    cam.compute_im3d(block=True)
+    cv2.imshow("im3d", cam.im3d)
+    cv2.waitKey(1)
+
+    time.sleep(0.05)
+
+cam.stop()
```

### Comparing `oakutils-0.0.2/examples/point_cloud.py` & `oakutils-0.0.3/examples/point_cloud.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Simple example of using the Camera class to display the point cloud
-import time
-
-from oakutils import Camera
-from oakutils.point_clouds import get_point_cloud_from_depth_image, PointCloudVisualizer
-
-
-DISPLAY_TIME = 10
-
-# using threading on the Visualizers can potentially improve performance
-VIS = PointCloudVisualizer(window_name="Depth Point Cloud")
-VIS2 = PointCloudVisualizer(
-    window_name="RGB Point Cloud", use_threading=False
-)  # showing that both options work
-
-cam = Camera(
-    display_point_cloud=False,  # the camera class has built in point cloud for RGBD images but we will be explicit
-    compute_point_cloud_on_demand=True,  # on demand, so must call compute_point_cloud to update
-)
-
-cam.start_display()
-cam.start()
-
-start_time = time.time()
-while True:
-    if time.time() - start_time > DISPLAY_TIME:
-        break
-
-    cam.compute_im3d(block=True)
-    cam.compute_point_cloud(block=True)
-
-    pcd = get_point_cloud_from_depth_image(cam.depth, cam.calibration.primary.pinhole)
-    VIS.update(pcd)
-    VIS2.update(cam.point_cloud)
-
-    time.sleep(0.05)
-
-VIS.stop()
-VIS2.stop()
-cam.stop()
+# Simple example of using the Camera class to display the point cloud
+import time
+
+from oakutils import Camera
+from oakutils.point_clouds import get_point_cloud_from_depth_image, PointCloudVisualizer
+
+
+DISPLAY_TIME = 10
+
+# using threading on the Visualizers can potentially improve performance
+VIS = PointCloudVisualizer(window_name="Depth Point Cloud")
+VIS2 = PointCloudVisualizer(
+    window_name="RGB Point Cloud", use_threading=False
+)  # showing that both options work
+
+cam = Camera(
+    display_point_cloud=False,  # the camera class has built in point cloud for RGBD images but we will be explicit
+    compute_point_cloud_on_demand=True,  # on demand, so must call compute_point_cloud to update
+)
+
+cam.start_display()
+cam.start()
+
+start_time = time.time()
+while True:
+    if time.time() - start_time > DISPLAY_TIME:
+        break
+
+    cam.compute_im3d(block=True)
+    cam.compute_point_cloud(block=True)
+
+    pcd = get_point_cloud_from_depth_image(cam.depth, cam.calibration.primary.pinhole)
+    VIS.update(pcd)
+    VIS2.update(cam.point_cloud)
+
+    time.sleep(0.05)
+
+VIS.stop()
+VIS2.stop()
+cam.stop()
```

### Comparing `oakutils-0.0.2/src/oakutils/camera.py` & `oakutils-0.0.3/src/oakutils/camera.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,720 +1,833 @@
-from threading import Thread, Condition
-from typing import List, Tuple, Optional
-import atexit
-
-import depthai as dai
-import numpy as np
-import cv2
-import open3d as o3d
-
-from .calibration import CalibrationData, create_camera_calibration
-from .point_clouds import PointCloudVisualizer, get_point_cloud_from_rgb_depth_image, filter_point_cloud
-
-
-# TODO: Implement all from link
-# https://docs.luxonis.com/projects/api/en/latest/samples/StereoDepth/depth_post_processing/#depth-post-processing
-
-# TODO: Implement all from link
-# https://docs.luxonis.com/projects/api/en/latest/tutorials/image_quality/#improving-image-quality
-
-# TODO: Implement all from link
-# https://docs.luxonis.com/projects/api/en/latest/components/nodes/stereo_depth/#currently-configurable-blocks
-
-
-# KNOWN BUGS:
-# - Enabling the speckle filter crashes the camera
-class Camera:
-    """
-    Class for interfacing with the OAK-D camera.
-    Params:
-        rgb_size: Size of the RGB image. Options are 1080p, 4K
-        enable_rgb: Whether to enable the RGB camera
-        mono_size: Size of the monochrome image. Options are 720p, 480p, 400p
-        enable_mono: Whether to enable the monochrome camera
-        primary_mono_left: Whether the primary monochrome image is the left image or the right image
-        use_cv2_Q_matrix: Whether to use the cv2.Q matrix for disparity to depth conversion
-        compute_im3d_on_demand: Whether to compute the IM3D on update
-        compute_point_cloud_on_demand: Whether to compute the point cloud on update
-        display_size: Size of the display window
-        display_rgb: Whether to display the RGB image
-        display_mono: Whether to display the monochrome image
-        display_depth: Whether to display the depth image
-        display_disparity: Whether to display the disparity image
-        display_rectified: Whether to display the rectified image
-        display_point_cloud: Whether to display the point cloud
-        extended_disparity: Whether to use extended disparity
-        subpixel: Whether to use subpixel
-        lr_check: Whether to use left-right check
-        median_filter: Whether to use median filter. If so, what size
-        stereo_confidence_threshold: Confidence threshold for stereo matching
-        stereo_speckle_filter_enable: Whether to use speckle filter
-        stereo_speckle_filter_range: Speckle filter range
-        stereo_temporal_filter_enable: Whether to use temporal filter
-        stereo_spatial_filter_enable: Whether to use spatial filter
-        stereo_spatial_filter_radius: Spatial filter radius
-        stereo_spatial_filter_num_iterations: Spatial filter number of iterations
-        stereo_threshold_filter_min_range: Threshold filter minimum range
-        stereo_threshold_filter_max_range: Threshold filter maximum range
-        stereo_decimation_filter_factor: Decimation filter factor. Options are 1, 2
-        enable_imu: Whether to enable the IMU
-        imu_batch_report_threshold: IMU batch report threshold
-        imu_max_batch_reports: IMU maximum report batches
-        imu_accelerometer_refresh_rate: IMU accelerometer refresh rate
-        imu_gyroscope_refresh_rate: IMU gyroscope refresh rate
-    """
-
-    def __init__(
-        self,
-        rgb_size: str = "1080p",
-        enable_rgb: bool = True,
-        mono_size: str = "400p",
-        enable_mono: bool = True,
-        rgb_fps: int = 30,
-        mono_fps: int = 60,
-        primary_mono_left: bool = True,
-        use_cv2_Q_matrix: bool = True,
-        compute_im3d_on_demand: bool = True,
-        compute_point_cloud_on_demand: bool = True,
-        display_size: Tuple[int, int] = (640, 400),
-        display_rgb: bool = False,
-        display_mono: bool = False,
-        display_depth: bool = False,
-        display_disparity: bool = True,
-        display_rectified: bool = False,
-        display_point_cloud: bool = False,
-        extended_disparity: bool = True,
-        subpixel: bool = False,
-        lr_check: bool = True,
-        median_filter: Optional[int] = 7,
-        stereo_confidence_threshold: int = 200,
-        stereo_speckle_filter_enable: bool = False,
-        stereo_speckle_filter_range: int = 60,
-        stereo_temporal_filter_enable: bool = True,
-        stereo_spatial_filter_enable: bool = True,
-        stereo_spatial_filter_radius: int = 2,
-        stereo_spatial_filter_num_iterations: int = 1,
-        stereo_threshold_filter_min_range: int = 200,
-        stereo_threshold_filter_max_range: int = 20000,
-        stereo_decimation_filter_factor: int = 1,
-        enable_imu: bool = False,
-        imu_batch_report_threshold: int = 20,
-        imu_max_batch_reports: int = 20,
-        imu_accelerometer_refresh_rate: int = 400,
-        imu_gyroscope_refresh_rate: int = 400,
-    ):
-        self._enable_rgb = enable_rgb
-        self._enable_mono = enable_mono
-        self._enable_imu = enable_imu
-
-        self._rgb_fps = rgb_fps
-        self._mono_fps = mono_fps
-
-        self._primary_mono_left = primary_mono_left
-        self._use_cv2_Q_matrix = use_cv2_Q_matrix
-
-        self._display_size = display_size
-        self._display_rgb = display_rgb
-        self._display_mono = display_mono
-        self._display_depth = display_depth
-        self._display_disparity = display_disparity
-        self._display_rectified = display_rectified
-        self._display_point_cloud = display_point_cloud
-
-        self._extended_disparity = extended_disparity
-        self._subpixel = subpixel
-        self._lr_check = lr_check
-
-        self._stereo_confidence_threshold = stereo_confidence_threshold
-        self._stereo_speckle_filter_enable = stereo_speckle_filter_enable
-        self._stereo_speckle_filter_range = stereo_speckle_filter_range
-        self._stereo_temporal_filter_enable = stereo_temporal_filter_enable
-        self._stereo_spatial_filter_enable = stereo_spatial_filter_enable
-        self._stereo_spatial_filter_radius = stereo_spatial_filter_radius
-        self._stereo_spatial_filter_num_iterations = (
-            stereo_spatial_filter_num_iterations
-        )
-        self._stereo_threshold_filter_min_range = stereo_threshold_filter_min_range
-        self._stereo_threshold_filter_max_range = stereo_threshold_filter_max_range
-        self._stereo_decimation_filter_factor = stereo_decimation_filter_factor
-
-        if rgb_size not in ["4k", "1080p"]:
-            raise ValueError('rgb_size must be one of "1080p" or "4k"')
-        else:
-            if rgb_size == "4k":
-                self._rgb_size = (
-                    3840,
-                    2160,
-                    dai.ColorCameraProperties.SensorResolution.THE_4_K,
-                )
-            elif rgb_size == "1080p":
-                self._rgb_size = (
-                    1920,
-                    1080,
-                    dai.ColorCameraProperties.SensorResolution.THE_1080_P,
-                )
-
-        if mono_size not in ["720p", "480p", "400p"]:
-            raise ValueError('mono_size must be one of "720p", "480p", or "400p"')
-        else:
-            if mono_size == "720p":
-                self._mono_size = (
-                    1280,
-                    720,
-                    dai.MonoCameraProperties.SensorResolution.THE_720_P,
-                )
-            elif mono_size == "480p":
-                self._mono_size = (
-                    640,
-                    480,
-                    dai.MonoCameraProperties.SensorResolution.THE_480_P,
-                )
-            elif mono_size == "400p":
-                self._mono_size = (
-                    640,
-                    400,
-                    dai.MonoCameraProperties.SensorResolution.THE_400_P,
-                )
-
-        if self._stereo_decimation_filter_factor == 2:
-            # need to divide the mono height by 2
-            self._mono_size = (
-                self._mono_size[0],
-                self._mono_size[1] // 2,
-                self._mono_size[2],
-            )
-
-        if median_filter not in [0, 3, 5, 7] and median_filter is not None:
-            raise ValueError("Unsupported median filter size, use 0, 3, 5, 7, or None")
-        else:
-            self._median_filter = median_filter
-            if self._median_filter == 3:
-                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_3x3
-            elif self._median_filter == 5:
-                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_5x5
-            elif self._median_filter == 7:
-                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_7x7
-            else:
-                self._median_filter = dai.StereoDepthProperties.MedianFilter.MEDIAN_OFF
-
-        self._calibration: CalibrationData = create_camera_calibration(
-            (self._rgb_size[0], self._rgb_size[1]),
-            (self._mono_size[0], self._mono_size[1]),
-            self._primary_mono_left,
-        )
-        self._Q = (
-            self._calibration.stereo.cv2_Q
-            if self._use_cv2_Q_matrix
-            else self._calibration.stereo.Q_primary
-        )
-
-        # pipeline
-        self._pipeline: dai.Pipeline = dai.Pipeline()
-        # storage for the nodes
-        self._nodes: List[str] = []
-        # stop condition
-        self._stopped: bool = False
-        # thread for the camera
-        self._cam_thread = Thread(target=self._target)
-
-        self._rgb_frame: Optional[np.ndarray] = None
-        self._rectified_rgb_frame: Optional[np.ndarray] = None
-        self._disparity: Optional[np.ndarray] = None
-        self._depth: Optional[np.ndarray] = None
-        self._left_frame: Optional[np.ndarray] = None
-        self._right_frame: Optional[np.ndarray] = None
-        self._left_rect_frame: Optional[np.ndarray] = None
-        self._right_rect_frame: Optional[np.ndarray] = None
-        self._primary_rect_frame: Optional[np.ndarray] = None
-
-        self._im3d: Optional[np.ndarray] = None
-        self._compute_im3d_on_demand = compute_im3d_on_demand
-        self._im3d_current = False
-
-        self._point_cloud: Optional[o3d.geometry.PointCloud] = None
-        self._compute_point_cloud_on_demand = compute_point_cloud_on_demand
-        self._point_cloud_vis = PointCloudVisualizer()
-
-        # imu information
-        self._imu_packet: Optional[np.ndarray] = None
-        self._imu_batch_report_threshold: int = imu_batch_report_threshold
-        self._imu_max_batch_reports: int = imu_max_batch_reports
-        self._imu_accelerometer_refresh_rate: float = imu_accelerometer_refresh_rate
-        self._imu_gyroscope_refresh_rate: float = imu_gyroscope_refresh_rate
-        self._imu_pose: List[float] = [0, 0, 0]
-        self._imu_rotation: List[float] = [0, 0, 0]
-
-        # packet for compute_3d
-        self._3d_packet: Tuple[
-            Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]
-        ] = (None, None, None)
-
-        # display information
-        self._display_thread = Thread(target=self._display)
-        self._display_stopped = False
-
-        # Condition for data
-        self._data_condition = Condition()
-
-        # set atexit methods
-        atexit.register(self.stop)
-
-    @property
-    def calibration(self) -> CalibrationData:
-        """
-        Gets the calibration data
-        """
-        return self._calibration
-
-    @property
-    def rgb(self) -> Optional[np.ndarray]:
-        """
-        Get the rgb color frame
-        """
-        return self._rgb_frame
-
-    @property
-    def rectified_rgb(self) -> Optional[np.ndarray]:
-        """
-        Get the rectified rgb color frame
-        """
-        return self._rectified_rgb_frame
-
-    @property
-    def disparity(self) -> Optional[np.ndarray]:
-        """
-        Gets the disparity frame
-        """
-        return self._disparity
-
-    @property
-    def depth(self) -> Optional[np.ndarray]:
-        """
-        Gets the depth frame
-        """
-        return self._depth
-
-    @property
-    def left(self) -> Optional[np.ndarray]:
-        """
-        Gets the left frame
-        """
-        return self._left_frame
-
-    @property
-    def right(self) -> Optional[np.ndarray]:
-        """
-        Gets the right frame
-        """
-        return self._right_frame
-
-    @property
-    def rectified_left_frame(self) -> Optional[np.ndarray]:
-        """
-        Gets the rectified left frame
-        """
-        return self._left_rect_frame
-
-    @property
-    def rectified_right_frame(self) -> Optional[np.ndarray]:
-        """
-        Gets the rectified right frame
-        """
-        return self._right_rect_frame
-
-    @property
-    def im3d(self) -> Optional[np.ndarray]:
-        """
-        Gets the 3d image
-        """
-        return self._im3d
-
-    @property
-    def point_cloud(self) -> Optional[o3d.geometry.PointCloud]:
-        """
-        Gets the point cloud
-        """
-        return self._point_cloud
-
-    @property
-    def imu_pose(self) -> List[float]:
-        """
-        Gets the imu pose (in meters)
-        """
-        return self._imu_pose
-
-    @property
-    def imu_rotation(self) -> List[float]:
-        """
-        Gets the imu rotation (in radians)
-        """
-        return self._imu_rotation
-
-    @property
-    def started(self) -> bool:
-        """
-        Returns true if the camera is started
-        """
-        return self._cam_thread.is_alive()
-
-    def start(self, block=True) -> None:
-        """
-        Starts the camera
-        """
-        self._cam_thread.start()
-        if block:
-            self.wait_for_data()
-
-    def stop(self) -> None:
-        """
-        Stops the camera
-        """
-        self._stopped = True
-        try:
-            self._cam_thread.join()
-        except RuntimeError:
-            pass
-
-        # stop the displays
-        self._display_stopped = True
-        try:
-            self._display_thread.join()
-        except RuntimeError:
-            pass
-
-        # close displays
-        cv2.destroyAllWindows()
-
-    def wait_for_data(self) -> None:
-        """
-        Blocks until a full set of data has arrived from the camera
-        """
-        with self._data_condition:
-            self._data_condition.wait()
-
-    def _display(self) -> None:
-        with self._data_condition:
-            self._data_condition.wait()
-        while not self._display_stopped:
-            if self._rgb_frame is not None and self._display_rgb:
-                cv2.imshow("rgb", cv2.resize(self._rgb_frame, self._display_size))
-            if self._disparity is not None and self._display_disparity:
-                frame = (
-                    self._disparity * (255 / self._stereo_confidence_threshold)
-                ).astype(np.uint8)
-                frame = cv2.resize(frame, self._display_size)
-                cv2.imshow("disparity-gray", frame)
-                frame = cv2.applyColorMap(frame, cv2.COLORMAP_JET)
-                cv2.imshow("disparity-color", frame)
-            if self._depth is not None and self._display_depth:
-                cv2.imshow("depth", cv2.resize(self._depth, self._display_size))
-            if self._left_frame is not None and self._display_mono:
-                cv2.imshow("left", cv2.resize(self._left_frame, self._display_size))
-            if self._right_frame is not None and self._display_mono:
-                cv2.imshow("right", cv2.resize(self._right_frame, self._display_size))
-            if self._left_rect_frame is not None and self._display_rectified:
-                cv2.imshow(
-                    "rectified left",
-                    cv2.resize(self._left_rect_frame, self._display_size),
-                )
-            if self._right_rect_frame is not None and self._display_rectified:
-                cv2.imshow(
-                    "rectified right",
-                    cv2.resize(self._right_rect_frame, self._display_size),
-                )
-            if self._point_cloud is not None and self._display_point_cloud:
-                self._point_cloud_vis.update(self._point_cloud)
-            cv2.waitKey(50)
-        self._point_cloud_vis.stop()
-
-    def start_display(self) -> None:
-        """
-        Starts the display thread
-        """
-        self._display_thread.start()
-
-    def stop_display(self) -> None:
-        """
-        Stops the display thread
-        """
-        self._display_stopped = True
-        self._display_thread.join()
-
-    def _create_cam_rgb(self) -> None:
-        cam = self._pipeline.create(dai.node.ColorCamera)
-        xout_video = self._pipeline.create(dai.node.XLinkOut)
-
-        cam.setBoardSocket(dai.CameraBoardSocket.RGB)
-        cam.setResolution(self._rgb_size[2])
-        cam.setInterleaved(False)
-        cam.setFps(self._rgb_fps)
-
-        xout_video.setStreamName("rgb")
-        cam.video.link(xout_video.input)
-
-        self._nodes.extend(["rgb"])
-
-    def _create_stereo(self) -> None:
-        left = self._pipeline.create(dai.node.MonoCamera)
-        right = self._pipeline.create(dai.node.MonoCamera)
-        stereo = self._pipeline.create(dai.node.StereoDepth)
-        stereo.setDefaultProfilePreset(dai.node.StereoDepth.PresetMode.HIGH_ACCURACY)
-        xout_left = self._pipeline.create(dai.node.XLinkOut)
-        xout_right = self._pipeline.create(dai.node.XLinkOut)
-        xout_depth = self._pipeline.create(dai.node.XLinkOut)
-        xout_disparity = self._pipeline.create(dai.node.XLinkOut)
-        xout_rect_left = self._pipeline.create(dai.node.XLinkOut)
-        xout_rect_right = self._pipeline.create(dai.node.XLinkOut)
-
-        left.setBoardSocket(dai.CameraBoardSocket.LEFT)
-        right.setBoardSocket(dai.CameraBoardSocket.RIGHT)
-        for cam in [left, right]:
-            cam.setFps(self._mono_fps)
-            cam.setResolution(self._mono_size[2])
-
-        stereo.initialConfig.setConfidenceThreshold(self._stereo_confidence_threshold)
-        stereo.setRectifyEdgeFillColor(0)
-        stereo.initialConfig.setMedianFilter(self._median_filter)
-        stereo.setLeftRightCheck(self._lr_check)
-        stereo.setExtendedDisparity(self._extended_disparity)
-        stereo.setSubpixel(self._subpixel)
-
-        config = stereo.initialConfig.get()
-        config.postProcessing.speckleFilter.enable = self._stereo_speckle_filter_enable
-        config.postProcessing.speckleFilter.speckleRange = (
-            self._stereo_speckle_filter_range
-        )
-        config.postProcessing.temporalFilter.enable = (
-            self._stereo_temporal_filter_enable
-        )
-        config.postProcessing.spatialFilter.enable = self._stereo_spatial_filter_enable
-        config.postProcessing.spatialFilter.holeFillingRadius = (
-            self._stereo_spatial_filter_radius
-        )
-        config.postProcessing.spatialFilter.numIterations = (
-            self._stereo_spatial_filter_num_iterations
-        )
-        config.postProcessing.thresholdFilter.minRange = (
-            self._stereo_threshold_filter_min_range
-        )
-        config.postProcessing.thresholdFilter.maxRange = (
-            self._stereo_threshold_filter_max_range
-        )
-        config.postProcessing.decimationFilter.decimationFactor = (
-            self._stereo_decimation_filter_factor
-        )
-        stereo.initialConfig.set(config)
-
-        xout_left.setStreamName("left")
-        xout_right.setStreamName("right")
-        xout_depth.setStreamName("depth")
-        xout_disparity.setStreamName("disparity")
-        xout_rect_left.setStreamName("rectified_left")
-        xout_rect_right.setStreamName("rectified_right")
-
-        left.out.link(stereo.left)
-        right.out.link(stereo.right)
-        stereo.syncedLeft.link(xout_left.input)
-        stereo.syncedRight.link(xout_right.input)
-        stereo.depth.link(xout_depth.input)
-        stereo.disparity.link(xout_disparity.input)
-        stereo.rectifiedLeft.link(xout_rect_left.input)
-        stereo.rectifiedRight.link(xout_rect_right.input)
-
-        self._nodes.extend(
-            ["left", "right", "depth", "disparity", "rectified_left", "rectified_right"]
-        )
-
-    def _create_imu(self) -> None:
-        imu = self._pipeline.create(dai.node.IMU)
-        xout_imu = self._pipeline.create(dai.node.XLinkOut)
-
-        imu.enableIMUSensor(dai.IMUSensor.GRAVITY, self._imu_accelerometer_refresh_rate)
-        imu.enableIMUSensor(
-            dai.IMUSensor.GYROSCOPE_CALIBRATED, self._imu_gyroscope_refresh_rate
-        )
-        imu.setBatchReportThreshold(self._imu_batch_report_threshold)
-        imu.setMaxBatchReports(self._imu_max_batch_reports)
-
-        xout_imu.setStreamName("imu")
-
-        imu.out.link(xout_imu.input)
-
-        self._nodes.extend(["imu"])
-
-    def _update_point_cloud(self) -> None:
-        pcd = get_point_cloud_from_rgb_depth_image(
-            self._rgb_frame, self._depth, self._calibration.primary.pinhole
-        )
-
-        pcd = filter_point_cloud(
-            pcd, voxel_size=None, nb_neighbors=30, std_ratio=0.1, downsample_first=True
-        )
-
-        if self._point_cloud is None:
-            self._point_cloud = pcd
-        else:
-            self._point_cloud.points = pcd.points
-            self._point_cloud.colors = pcd.colors
-
-    def _update_im3d(self) -> None:
-        self._im3d = cv2.reprojectImageTo3D(self._disparity, self._Q)
-
-    def _target(self) -> None:
-        if self._enable_rgb:
-            self._create_cam_rgb()
-        if self._enable_mono:
-            self._create_stereo()
-        if self._enable_imu:
-            self._create_imu()
-        with dai.Device(self._pipeline) as device:
-            queues = {}
-            for stream in self._nodes:
-                queues[stream] = device.getOutputQueue(
-                    name=stream, maxSize=1, blocking=False
-                )
-
-            base_accel_timestamp = None
-            base_gyro_timestamp = None
-            while not self._stopped:
-                for name, queue in queues.items():
-                    if queue is not None:
-                        data = queue.get()
-                        if name == "rgb":
-                            self._rgb_frame = data.getCvFrame()
-                            self._rectified_rgb_frame = cv2.remap(
-                                self._rgb_frame,
-                                self._calibration.rgb.map_1,
-                                self._calibration.rgb.map_2,
-                                cv2.INTER_LINEAR,
-                            )
-                        elif name == "left":
-                            self._left_frame = data.getCvFrame()
-                        elif name == "right":
-                            self._right_frame = data.getCvFrame()
-                        elif name == "depth":
-                            self._depth = data.getCvFrame()
-                        elif name == "disparity":
-                            self._disparity = data.getCvFrame()
-                        elif name == "rectified_left":
-                            self._left_rect_frame = data.getCvFrame()
-                        elif name == "rectified_right":
-                            self._right_rect_frame = data.getCvFrame()
-                        elif name == "imu":
-                            packets = data.packets
-                            for imuPacket in packets:
-                                acceleroValues = imuPacket.acceleroMeter
-                                gyroValues = imuPacket.gyroscope
-
-                                acclero_ts_device = acceleroValues.getTimestampDevice()
-                                gyro_ts_device = gyroValues.getTimestampDevice()
-
-                                if base_accel_timestamp is None:
-                                    base_accel_timestamp = acclero_ts_device
-                                if base_gyro_timestamp is None:
-                                    base_gyro_timestamp = gyro_ts_device
-
-                                accelero_ts = (
-                                    acclero_ts_device - base_accel_timestamp
-                                ).total_seconds()
-                                gyro_ts = (
-                                    gyro_ts_device - base_gyro_timestamp
-                                ).total_seconds()
-
-                                ax, ay, az = (
-                                    acceleroValues.x,
-                                    acceleroValues.y,
-                                    acceleroValues.z,
-                                )
-                                gx, gy, gz = gyroValues.x, gyroValues.y, gyroValues.z
-
-                                # double integrate each ax, ay, az
-                                self._imu_pose[0] += ax * (accelero_ts**2)
-                                self._imu_pose[1] += ay * (accelero_ts**2)
-                                self._imu_pose[2] += az * (accelero_ts**2)
-
-                                # integrate each gx, gy, gz
-                                self._imu_rotation[0] += gx * gyro_ts
-                                self._imu_rotation[1] += gy * gyro_ts
-                                self._imu_rotation[2] += gz * gyro_ts
-
-                                base_accel_timestamp = acclero_ts_device
-                                base_gyro_timestamp = gyro_ts_device
-
-                # handle primary mono camera
-                self._primary_rect_frame = (
-                    self._left_rect_frame
-                    if self._primary_mono_left
-                    else self._right_rect_frame
-                )
-                # handle 3d images and odometry packets
-                if not self._compute_im3d_on_demand:
-                    self._update_im3d()
-                self._3d_packet = (
-                    self._im3d,
-                    self._disparity,
-                    self._primary_rect_frame,
-                )
-                # handle the point cloud
-                if not self._compute_point_cloud_on_demand:
-                    self._update_point_cloud()
-
-                with self._data_condition:
-                    self._data_condition.notify_all()
-
-    def _crop_to_valid_primary_region(self, img: np.ndarray) -> np.ndarray:
-        return img[
-            self._calibration.primary.valid_region[
-                1
-            ] : self._calibration.primary.valid_region[3],
-            self._calibration.primary.valid_region[
-                0
-            ] : self._calibration.primary.valid_region[2],
-        ]
-
-    def compute_point_cloud(self, block=True) -> Optional[o3d.geometry.PointCloud]:
-        """
-        Compute point cloud from depth map.
-
-        Params:
-            block: bool
-                If True, block until the next data packet is received.
-
-        Returns:
-            Optional[o3d.geometry.PointCloud]: point cloud
-        """
-        if block:
-            with self._data_condition:
-                self._data_condition.wait()
-        if self._rgb_frame is None and self._depth is None:
-            return None
-        if self._compute_point_cloud_on_demand:
-            self._update_point_cloud()
-        return self._point_cloud
-
-    def compute_im3d(
-        self, block=True
-    ) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]:
-        """
-        Compute 3D points from disparity map.
-
-        Params:
-            block: bool
-                If True, block until the next data packet is received.
-
-        Returns:
-            Tuple[np.ndarray, np.ndarray, np.ndarray]: depth map, disparity map, left frame
-        """
-        if block:
-            with self._data_condition:
-                self._data_condition.wait()
-        im3d, disparity, rect = self._3d_packet
-        if im3d is None and disparity is None and rect is None:
-            return None, None, None
-        if self._compute_im3d_on_demand:
-            self._update_im3d()
-            im3d = self._im3d
-        return (
-            self._crop_to_valid_primary_region(im3d),
-            self._crop_to_valid_primary_region(disparity),
-            self._crop_to_valid_primary_region(rect),
-        )
+from threading import Thread, Condition
+from typing import List, Tuple, Optional
+import atexit
+
+import depthai as dai
+import numpy as np
+import cv2
+import open3d as o3d
+
+from .calibration import CalibrationData, get_camera_calibration
+from .point_clouds import (
+    PointCloudVisualizer,
+    get_point_cloud_from_rgb_depth_image,
+    filter_point_cloud,
+)
+from .nodes import (
+    create_color_camera,
+    create_stereo_depth,
+    create_imu,
+)
+
+
+# KNOWN BUGS:
+# - Enabling the speckle filter crashes the camera
+class Camera:
+    """
+    Class for interfacing with the OAK-D camera.
+
+    Attributes
+    ----------
+    calibration : CalibrationData
+        The calibration data for the camera.
+    rgb : Optional[np.ndarray]
+        The most recent RGB image from the camera.
+    rectified_rgb : Optional[np.ndarray]
+        The most recent rectified RGB image from the camera.
+    disparity: Optional[np.ndarray]
+        The most recent disparity image from the camera.
+    depth: Optional[np.ndarray]
+        The most recent depth image from the camera.
+    left: Optional[np.ndarray]
+        The most recent left mono image from the camera.
+    right: Optional[np.ndarray]
+        The most recent right mono image from the camera.
+    rectified_left: Optional[np.ndarray]
+        The most recent rectified left mono image from the camera.
+    rectified_right: Optional[np.ndarray]
+        The most recent rectified right mono image from the camera.
+    im3d: Optional[np.ndarray]
+        The most recent im3d image from the camera.
+    point_cloud: Optional[o3d.geometry.PointCloud]
+        The most recent point cloud from the camera.
+    imu_pose: Optional[List[float]]
+        The most recent IMU pose from the camera.
+    imu_rotation: Optional[List[float]]
+        The most recent IMU rotation from the camera.
+    started: bool
+        Whether or not the camera has been started.
+
+    Methods
+    -------
+    start()
+        Starts the camera.
+    stop()
+        Stops the camera.
+    wait_for_data()
+        Waits for the data packet to be ready.
+    start_display()
+        Starts the display.
+    stop_display()
+        Stops the display.
+    compute_point_cloud(block=True)
+        Computes the point cloud from the depth map.
+    compute_im3d(block=True)
+        Computes the 3D points from the disparity map.
+    """
+
+    def __init__(
+        self,
+        rgb_size: str = "1080p",
+        enable_rgb: bool = True,
+        mono_size: str = "400p",
+        enable_mono: bool = True,
+        rgb_fps: int = 30,
+        mono_fps: int = 60,
+        primary_mono_left: bool = True,
+        use_cv2_Q_matrix: bool = True,
+        compute_im3d_on_demand: bool = True,
+        compute_point_cloud_on_demand: bool = True,
+        display_size: Tuple[int, int] = (640, 400),
+        display_rgb: bool = False,
+        display_mono: bool = False,
+        display_depth: bool = False,
+        display_disparity: bool = True,
+        display_rectified: bool = False,
+        display_point_cloud: bool = False,
+        extended_disparity: bool = True,
+        subpixel: bool = False,
+        lr_check: bool = True,
+        median_filter: Optional[int] = 7,
+        stereo_confidence_threshold: int = 200,
+        stereo_speckle_filter_enable: bool = False,
+        stereo_speckle_filter_range: int = 60,
+        stereo_temporal_filter_enable: bool = True,
+        stereo_spatial_filter_enable: bool = True,
+        stereo_spatial_filter_radius: int = 2,
+        stereo_spatial_filter_num_iterations: int = 1,
+        stereo_threshold_filter_min_range: int = 200,
+        stereo_threshold_filter_max_range: int = 20000,
+        stereo_decimation_filter_factor: int = 1,
+        enable_imu: bool = False,
+        imu_batch_report_threshold: int = 20,
+        imu_max_batch_reports: int = 20,
+        imu_accelerometer_refresh_rate: int = 400,
+        imu_gyroscope_refresh_rate: int = 400,
+    ):
+        """
+        Initializes the camera object.
+
+        Parameters
+        ----------
+        rgb_size : str, optional
+            Size of the RGB image. Options are 1080p, 4K.
+        enable_rgb : bool, optional
+            Whether to enable the RGB camera.
+        mono_size : str, optional
+            Size of the monochrome image. Options are 720p, 480p, 400p.
+        enable_mono : bool, optional
+            Whether to enable the monochrome camera.
+        rgb_fps : int, optional
+            FPS for the RGB camera.
+        mono_fps : int, optional
+            FPS for the monochrome camera.
+        primary_mono_left : bool, optional
+            Whether the primary monochrome image is the left image or the right image.
+        use_cv2_Q_matrix : bool, optional
+            Whether to use the cv2.Q matrix for disparity to depth conversion.
+        compute_im3d_on_demand : bool, optional
+            Whether to compute the IM3D on update.
+        compute_point_cloud_on_demand : bool, optional
+            Whether to compute the point cloud on update.
+        display_size : tuple[int, int], optional
+            Size of the display window.
+        display_rgb : bool, optional
+            Whether to display the RGB image.
+        display_mono : bool, optional
+            Whether to display the monochrome image.
+        display_depth : bool, optional
+            Whether to display the depth image.
+        display_disparity : bool, optional
+            Whether to display the disparity image.
+        display_rectified : bool, optional
+            Whether to display the rectified image.
+        display_point_cloud : bool, optional
+            Whether to display the point cloud.
+        extended_disparity : bool, optional
+            Whether to use extended disparity.
+        subpixel : bool, optional
+            Whether to use subpixel.
+        lr_check : bool, optional
+            Whether to use left-right check.
+        median_filter : int or None, optional
+            Whether to use median filter. If so, what size.
+        stereo_confidence_threshold : int, optional
+            Confidence threshold for stereo matching.
+        stereo_speckle_filter_enable : bool, optional
+            Whether to use speckle filter.
+        stereo_speckle_filter_range : int, optional
+            Speckle filter range.
+        stereo_temporal_filter_enable : bool, optional
+            Whether to use temporal filter.
+        stereo_spatial_filter_enable : bool, optional
+            Whether to use spatial filter.
+        stereo_spatial_filter_radius : int, optional
+            Spatial filter radius.
+        stereo_spatial_filter_num_iterations : int, optional
+            Spatial filter number of iterations.
+        stereo_threshold_filter_min_range : int, optional
+            Threshold filter minimum range.
+        stereo_threshold_filter_max_range : int, optional
+            Threshold filter maximum range.
+        stereo_decimation_filter_factor : int, optional
+            Decimation filter factor. Options are 1, 2.
+        enable_imu : bool, optional
+            Whether to enable the IMU.
+        imu_batch_report_threshold : int, optional
+            IMU batch report threshold.
+        imu_max_batch_reports : int, optional
+            IMU maximum report batches.
+        imu_accelerometer_refresh_rate : int, optional
+            IMU accelerometer refresh rate.
+        imu_gyroscope_refresh_rate : int, optional
+            IMU gyroscope refresh rate.
+        """
+        self._primary_mono_left = primary_mono_left
+        self._use_cv2_Q_matrix = use_cv2_Q_matrix
+
+        self._display_size = display_size
+        self._display_rgb = display_rgb
+        self._display_mono = display_mono
+        self._display_depth = display_depth
+        self._display_disparity = display_disparity
+        self._display_rectified = display_rectified
+        self._display_point_cloud = display_point_cloud
+
+        self._stereo_confidence_threshold = stereo_confidence_threshold
+
+        if rgb_size not in ["4k", "1080p"]:
+            raise ValueError('rgb_size must be one of "1080p" or "4k"')
+        else:
+            if rgb_size == "4k":
+                self._rgb_size = (
+                    3840,
+                    2160,
+                    dai.ColorCameraProperties.SensorResolution.THE_4_K,
+                )
+            elif rgb_size == "1080p":
+                self._rgb_size = (
+                    1920,
+                    1080,
+                    dai.ColorCameraProperties.SensorResolution.THE_1080_P,
+                )
+
+        if mono_size not in ["720p", "480p", "400p"]:
+            raise ValueError('mono_size must be one of "720p", "480p", or "400p"')
+        else:
+            if mono_size == "720p":
+                self._mono_size = (
+                    1280,
+                    720,
+                    dai.MonoCameraProperties.SensorResolution.THE_720_P,
+                )
+            elif mono_size == "480p":
+                self._mono_size = (
+                    640,
+                    480,
+                    dai.MonoCameraProperties.SensorResolution.THE_480_P,
+                )
+            elif mono_size == "400p":
+                self._mono_size = (
+                    640,
+                    400,
+                    dai.MonoCameraProperties.SensorResolution.THE_400_P,
+                )
+
+        if stereo_decimation_filter_factor == 2:
+            # need to divide the mono height by 2
+            self._mono_size = (
+                self._mono_size[0],
+                self._mono_size[1] // 2,
+                self._mono_size[2],
+            )
+
+        if median_filter not in [0, 3, 5, 7] and median_filter is not None:
+            raise ValueError("Unsupported median filter size, use 0, 3, 5, 7, or None")
+        else:
+            self._median_filter = median_filter
+            if self._median_filter == 3:
+                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_3x3
+            elif self._median_filter == 5:
+                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_5x5
+            elif self._median_filter == 7:
+                self._median_filter = dai.StereoDepthProperties.MedianFilter.KERNEL_7x7
+            else:
+                self._median_filter = dai.StereoDepthProperties.MedianFilter.MEDIAN_OFF
+
+        self._calibration: CalibrationData = get_camera_calibration(
+            (self._rgb_size[0], self._rgb_size[1]),
+            (self._mono_size[0], self._mono_size[1]),
+            self._primary_mono_left,
+        )
+        self._Q = (
+            self._calibration.stereo.cv2_Q
+            if self._use_cv2_Q_matrix
+            else self._calibration.stereo.Q_primary
+        )
+
+        # pipeline
+        self._pipeline: dai.Pipeline = dai.Pipeline()
+        # storage for the nodes
+        self._streams: List[str] = []
+        # stop condition
+        self._stopped: bool = False
+        # thread for the camera
+        self._cam_thread = Thread(target=self._target)
+
+        self._rgb_frame: Optional[np.ndarray] = None
+        self._rectified_rgb_frame: Optional[np.ndarray] = None
+        self._disparity: Optional[np.ndarray] = None
+        self._depth: Optional[np.ndarray] = None
+        self._left_frame: Optional[np.ndarray] = None
+        self._right_frame: Optional[np.ndarray] = None
+        self._left_rect_frame: Optional[np.ndarray] = None
+        self._right_rect_frame: Optional[np.ndarray] = None
+        self._primary_rect_frame: Optional[np.ndarray] = None
+
+        self._im3d: Optional[np.ndarray] = None
+        self._compute_im3d_on_demand = compute_im3d_on_demand
+        self._im3d_current = False
+
+        self._point_cloud: Optional[o3d.geometry.PointCloud] = None
+        self._compute_point_cloud_on_demand = compute_point_cloud_on_demand
+        self._point_cloud_vis = PointCloudVisualizer()
+
+        # imu information
+        self._imu_packet: Optional[np.ndarray] = None
+        self._imu_batch_report_threshold: int = imu_batch_report_threshold
+        self._imu_max_batch_reports: int = imu_max_batch_reports
+        self._imu_accelerometer_refresh_rate: float = imu_accelerometer_refresh_rate
+        self._imu_gyroscope_refresh_rate: float = imu_gyroscope_refresh_rate
+        self._imu_pose: List[float] = [0, 0, 0]
+        self._imu_rotation: List[float] = [0, 0, 0]
+
+        # packet for compute_3d
+        self._3d_packet: Tuple[
+            Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]
+        ] = (None, None, None)
+
+        # display information
+        self._display_thread = Thread(target=self._display)
+        self._display_stopped = False
+
+        # Condition for data
+        self._data_condition = Condition()
+
+        # creaate the nodes on the pipeline
+        if enable_rgb:
+            cam = create_color_camera(
+                pipeline=self._pipeline,
+                resolution=self._rgb_size[2],
+                fps=rgb_fps,
+            )
+            xout_rgb = self._pipeline.create(dai.node.XLinkOut)
+            xout_rgb.setStreamName("rgb")
+            cam.video.link(xout_rgb.input)
+
+            self._streams.extend(["rgb"])
+        if enable_mono:
+            align_socket = (
+                dai.CameraBoardSocket.LEFT
+                if self._primary_mono_left
+                else dai.CameraBoardSocket.RIGHT
+            )
+            (
+                stereo,
+                left,
+                right,
+                xout_left,
+                xout_right,
+                xout_depth,
+                xout_disparity,
+                xout_rect_left,
+                xout_rect_right,
+            ) = create_stereo_depth(
+                pipeline=self._pipeline,
+                resolution=self._mono_size[2],
+                fps=mono_fps,
+                align_socket=align_socket,
+                confidence_threshold=stereo_confidence_threshold,
+                median_filter=self._median_filter,
+                lr_check=lr_check,
+                extended_disparity=extended_disparity,
+                subpixel=subpixel,
+                decimation_factor=stereo_decimation_filter_factor,
+                enable_spatial_filter=stereo_spatial_filter_enable,
+                enable_speckle_filter=stereo_speckle_filter_enable,
+                enable_temporal_filter=stereo_temporal_filter_enable,
+                speckle_range=stereo_speckle_filter_range,
+                spatial_radius=stereo_spatial_filter_radius,
+                spatial_iterations=stereo_spatial_filter_num_iterations,
+                threshold_min_range=stereo_threshold_filter_min_range,
+                threshold_max_range=stereo_threshold_filter_max_range,
+            )
+
+            self._streams.extend(
+                [
+                    "left",
+                    "right",
+                    "depth",
+                    "disparity",
+                    "rectified_left",
+                    "rectified_right",
+                ]
+            )
+        if enable_imu:
+            imu, xout_imu = create_imu(
+                pipeline=self._pipeline,
+                accel_range=self._imu_accelerometer_refresh_rate,
+                gyroscope_rate=self._imu_gyroscope_refresh_rate,
+                batch_report_threshold=self._imu_batch_report_threshold,
+                max_batch_reports=self._imu_max_batch_reports,
+                enable_accelerometer_raw=True,
+                enable_gyroscope_raw=True,
+            )
+
+            self._streams.extend(["imu"])
+
+        # set atexit methods
+        atexit.register(self.stop)
+
+    @property
+    def calibration(self) -> CalibrationData:
+        """
+        Gets the calibration data.
+
+        Returns
+        -------
+        np.ndarray
+            The calibration data.
+        """
+        return self._calibration
+
+    @property
+    def rgb(self) -> Optional[np.ndarray]:
+        """
+        Get the rectified RGB color frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The rectified RGB color frame, or None if the frame is not available.
+        """
+        return self._rgb_frame
+
+    @property
+    def rectified_rgb(self) -> Optional[np.ndarray]:
+        """
+        Get the rectified RGB color frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The rectified RGB color frame, or None if the frame is not available.
+        """
+        return self._rectified_rgb_frame
+
+    @property
+    def disparity(self) -> Optional[np.ndarray]:
+        """
+        Get the disparity frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The disparity frame, or None if the frame is not available.
+        """
+        return self._disparity
+
+    @property
+    def depth(self) -> Optional[np.ndarray]:
+        """
+        Get the depth frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The depth frame, or None if the frame is not available.
+        """
+        return self._depth
+
+    @property
+    def left(self) -> Optional[np.ndarray]:
+        """
+        Get the left frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The left frame, or None if the frame is not available.
+        """
+        return self._left_frame
+
+    @property
+    def right(self) -> Optional[np.ndarray]:
+        """
+        Get the right frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The right frame, or None if the frame is not available.
+        """
+        return self._right_frame
+
+    @property
+    def rectified_left(self) -> Optional[np.ndarray]:
+        """
+        Gets the rectified left frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The rectified left frame, or None if the frame is not available.
+        """
+        return self._left_rect_frame
+
+    @property
+    def rectified_right(self) -> Optional[np.ndarray]:
+        """
+        Gets the rectified right frame.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The rectified right frame, or None if the frame is not available.
+        """
+        return self._right_rect_frame
+
+    @property
+    def im3d(self) -> Optional[np.ndarray]:
+        """
+        Gets the 3D image.
+
+        Returns
+        -------
+        Optional[np.ndarray]
+            The 3D image, or None if it is not available.
+        """
+        return self._im3d
+
+    @property
+    def point_cloud(self) -> Optional[o3d.geometry.PointCloud]:
+        """
+        Gets the point cloud.
+
+        Returns
+        -------
+        Optional[o3d.geometry.PointCloud]
+            The point cloud, or None if it is not available.
+        """
+        return self._point_cloud
+
+    @property
+    def imu_pose(self) -> List[float]:
+        """
+        Gets the IMU pose in meters.
+
+        Returns
+        -------
+        List[float]
+            The IMU pose as a list of floats.
+        """
+        return self._imu_pose
+
+    @property
+    def imu_rotation(self) -> List[float]:
+        """
+        Gets the IMU rotation in radians.
+
+        Returns
+        -------
+        List[float]
+            The IMU rotation as a list of floats.
+        """
+        return self._imu_rotation
+
+    @property
+    def started(self) -> bool:
+        """
+        Returns True if the camera is started.
+
+        Returns
+        -------
+        bool
+            True if the camera is started, False otherwise.
+        """
+        return self._cam_thread.is_alive()
+
+    def start(self, block=True) -> None:
+        """
+        Starts the camera.
+
+        Parameters
+        ----------
+        block : bool, optional
+            If True, blocks until the first set of data arrives. Defaults to False.
+        """
+        self._cam_thread.start()
+        if block:
+            self.wait_for_data()
+
+    def stop(self) -> None:
+        """
+        Stops the camera
+        """
+        self._stopped = True
+        try:
+            self._cam_thread.join()
+        except RuntimeError:
+            pass
+
+        # stop the displays
+        self._display_stopped = True
+        try:
+            self._display_thread.join()
+        except RuntimeError:
+            pass
+
+        # close displays
+        cv2.destroyAllWindows()
+
+    def wait_for_data(self) -> None:
+        """
+        Blocks until a full set of data has arrived from the camera
+        """
+        with self._data_condition:
+            self._data_condition.wait()
+
+    def _display(self) -> None:
+        with self._data_condition:
+            self._data_condition.wait()
+        while not self._display_stopped:
+            if self._rgb_frame is not None and self._display_rgb:
+                cv2.imshow("rgb", cv2.resize(self._rgb_frame, self._display_size))
+            if self._disparity is not None and self._display_disparity:
+                frame = (
+                    self._disparity * (255 / self._stereo_confidence_threshold)
+                ).astype(np.uint8)
+                frame = cv2.resize(frame, self._display_size)
+                cv2.imshow("disparity-gray", frame)
+                frame = cv2.applyColorMap(frame, cv2.COLORMAP_JET)
+                cv2.imshow("disparity-color", frame)
+            if self._depth is not None and self._display_depth:
+                cv2.imshow("depth", cv2.resize(self._depth, self._display_size))
+            if self._left_frame is not None and self._display_mono:
+                cv2.imshow("left", cv2.resize(self._left_frame, self._display_size))
+            if self._right_frame is not None and self._display_mono:
+                cv2.imshow("right", cv2.resize(self._right_frame, self._display_size))
+            if self._left_rect_frame is not None and self._display_rectified:
+                cv2.imshow(
+                    "rectified left",
+                    cv2.resize(self._left_rect_frame, self._display_size),
+                )
+            if self._right_rect_frame is not None and self._display_rectified:
+                cv2.imshow(
+                    "rectified right",
+                    cv2.resize(self._right_rect_frame, self._display_size),
+                )
+            if self._point_cloud is not None and self._display_point_cloud:
+                self._point_cloud_vis.update(self._point_cloud)
+            cv2.waitKey(50)
+        self._point_cloud_vis.stop()
+
+    def start_display(self) -> None:
+        """
+        Starts the display thread
+        """
+        self._display_thread.start()
+
+    def stop_display(self) -> None:
+        """
+        Stops the display thread
+        """
+        self._display_stopped = True
+        self._display_thread.join()
+
+    def _update_point_cloud(self) -> None:
+        pcd = get_point_cloud_from_rgb_depth_image(
+            self._rgb_frame, self._depth, self._calibration.primary.pinhole
+        )
+
+        pcd = filter_point_cloud(
+            pcd, voxel_size=None, nb_neighbors=30, std_ratio=0.1, downsample_first=True
+        )
+
+        if self._point_cloud is None:
+            self._point_cloud = pcd
+        else:
+            self._point_cloud.points = pcd.points
+            self._point_cloud.colors = pcd.colors
+
+    def _update_im3d(self) -> None:
+        self._im3d = cv2.reprojectImageTo3D(self._disparity, self._Q)
+
+    def _target(self) -> None:
+        with dai.Device(self._pipeline) as device:
+            queues = {}
+            for stream in self._streams:
+                queues[stream] = device.getOutputQueue(
+                    name=stream, maxSize=1, blocking=False
+                )
+
+            base_accel_timestamp = None
+            base_gyro_timestamp = None
+            while not self._stopped:
+                for name, queue in queues.items():
+                    if queue is not None:
+                        data = queue.get()
+                        if name == "rgb":
+                            self._rgb_frame = data.getCvFrame()
+                            self._rectified_rgb_frame = cv2.remap(
+                                self._rgb_frame,
+                                self._calibration.rgb.map_1,
+                                self._calibration.rgb.map_2,
+                                cv2.INTER_LINEAR,
+                            )
+                        elif name == "left":
+                            self._left_frame = data.getCvFrame()
+                        elif name == "right":
+                            self._right_frame = data.getCvFrame()
+                        elif name == "depth":
+                            self._depth = data.getCvFrame()
+                        elif name == "disparity":
+                            self._disparity = data.getCvFrame()
+                        elif name == "rectified_left":
+                            self._left_rect_frame = data.getCvFrame()
+                        elif name == "rectified_right":
+                            self._right_rect_frame = data.getCvFrame()
+                        elif name == "imu":
+                            packets = data.packets
+                            for imuPacket in packets:
+                                acceleroValues = imuPacket.acceleroMeter
+                                gyroValues = imuPacket.gyroscope
+
+                                acclero_ts_device = acceleroValues.getTimestampDevice()
+                                gyro_ts_device = gyroValues.getTimestampDevice()
+
+                                if base_accel_timestamp is None:
+                                    base_accel_timestamp = acclero_ts_device
+                                if base_gyro_timestamp is None:
+                                    base_gyro_timestamp = gyro_ts_device
+
+                                accelero_ts = (
+                                    acclero_ts_device - base_accel_timestamp
+                                ).total_seconds()
+                                gyro_ts = (
+                                    gyro_ts_device - base_gyro_timestamp
+                                ).total_seconds()
+
+                                ax, ay, az = (
+                                    acceleroValues.x,
+                                    acceleroValues.y,
+                                    acceleroValues.z,
+                                )
+                                gx, gy, gz = gyroValues.x, gyroValues.y, gyroValues.z
+
+                                # double integrate each ax, ay, az
+                                self._imu_pose[0] += ax * (accelero_ts**2)
+                                self._imu_pose[1] += ay * (accelero_ts**2)
+                                self._imu_pose[2] += az * (accelero_ts**2)
+
+                                # integrate each gx, gy, gz
+                                self._imu_rotation[0] += gx * gyro_ts
+                                self._imu_rotation[1] += gy * gyro_ts
+                                self._imu_rotation[2] += gz * gyro_ts
+
+                                base_accel_timestamp = acclero_ts_device
+                                base_gyro_timestamp = gyro_ts_device
+
+                # handle primary mono camera
+                self._primary_rect_frame = (
+                    self._left_rect_frame
+                    if self._primary_mono_left
+                    else self._right_rect_frame
+                )
+                # handle 3d images and odometry packets
+                if not self._compute_im3d_on_demand:
+                    self._update_im3d()
+                self._3d_packet = (
+                    self._im3d,
+                    self._disparity,
+                    self._primary_rect_frame,
+                )
+                # handle the point cloud
+                if not self._compute_point_cloud_on_demand:
+                    self._update_point_cloud()
+
+                with self._data_condition:
+                    self._data_condition.notify_all()
+
+    def _crop_to_valid_primary_region(self, img: np.ndarray) -> np.ndarray:
+        return img[
+            self._calibration.primary.valid_region[
+                1
+            ] : self._calibration.primary.valid_region[3],
+            self._calibration.primary.valid_region[
+                0
+            ] : self._calibration.primary.valid_region[2],
+        ]
+
+    def compute_point_cloud(self, block=True) -> Optional[o3d.geometry.PointCloud]:
+        """
+        Compute a point cloud from the depth map.
+
+        Parameters
+        ----------
+        block : bool, optional
+            If True, blocks until the next data packet is received. Defaults to True.
+
+        Returns
+        -------
+        Optional[o3d.geometry.PointCloud]
+            The computed point cloud, or None if no data is available.
+        """
+        if block:
+            with self._data_condition:
+                self._data_condition.wait()
+        if self._rgb_frame is None and self._depth is None:
+            return None
+        if self._compute_point_cloud_on_demand:
+            self._update_point_cloud()
+        return self._point_cloud
+
+    def compute_im3d(
+        self, block=True
+    ) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]:
+        """
+        Compute 3D points from the disparity map.
+
+        Parameters
+        ----------
+        block : bool, optional
+            If True, blocks until the next data packet is received. Defaults to True.
+
+        Returns
+        -------
+        Tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]
+            A tuple containing the depth map, disparity map, and left frame (if available).
+        """
+        if block:
+            with self._data_condition:
+                self._data_condition.wait()
+        im3d, disparity, rect = self._3d_packet
+        if im3d is None and disparity is None and rect is None:
+            return None, None, None
+        if self._compute_im3d_on_demand:
+            self._update_im3d()
+            im3d = self._im3d
+        return (
+            self._crop_to_valid_primary_region(im3d),
+            self._crop_to_valid_primary_region(disparity),
+            self._crop_to_valid_primary_region(rect),
+        )
```

### Comparing `oakutils-0.0.2/LICENSE` & `oakutils-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `oakutils-0.0.2/pyproject.toml` & `oakutils-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,76 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "oakutils"
-version = "0.0.2"
-authors = [
-  {name="Justin Davis", email="davisjustin302@gmail.com"},
-]
-maintainers = [
-  {name="Justin Davis", email="davisjustin302@gmail.com"},
-]
-readme = "README.md"
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS",
-    "Natural Language :: English",
-    "Topic :: System :: Hardware",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Software Development",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "Intended Audience :: Education",
-    "Intended Audience :: Information Technology",
-    "Typing :: Typed",
-]
-requires-python=">=3.8"
-dependencies = [
-    "depthai>=2.20",
-    "numpy>=1.20",
-    "open3d>=0.16",
-    "opencv-python>=4.5",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/justincdavis/oakutils"
-"Bug Tracker" = "https://github.com/justincdavis/oakutils/issues"
-
-[project.optional-dependencies]
-dev = [
-    "black",
-    "pylint",
-    "mypy",
-    "twine",
-    "wheel",
-    "bumpver",
-]
-
-[tool.bumpver]
-current_version = "0.0.2"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message  = "Bump version {old_version} -> {new_version}"
-commit          = true
-tag             = true
-push            = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/oakutils/__init__.py" = ["{version}"]
-
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "oakutils"
+version = "0.0.3"
+authors = [
+  {name="Justin Davis", email="davisjustin302@gmail.com"},
+]
+maintainers = [
+  {name="Justin Davis", email="davisjustin302@gmail.com"},
+]
+readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS",
+    "Natural Language :: English",
+    "Topic :: System :: Hardware",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Education",
+    "Intended Audience :: Information Technology",
+    "Typing :: Typed",
+]
+requires-python=">=3.8"
+dependencies = [
+    "depthai>=2.20",
+    "numpy>=1.20",
+    "open3d>=0.16",
+    "opencv-python>=4.5",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/justincdavis/oakutils"
+"Bug Tracker" = "https://github.com/justincdavis/oakutils/issues"
+
+[project.optional-dependencies]
+dev = [
+    "black",
+    "pylint",
+    "mypy",
+    "twine",
+    "wheel",
+    "bumpver",
+    "kornia",
+    "torch",
+    "sphinx",
+    "sphinx-rtd-theme",
+]
+
+[tool.bumpver]
+current_version = "0.0.3"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message  = "Bump version {old_version} -> {new_version}"
+commit          = true
+tag             = true
+push            = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"src/oakutils/__init__.py" = ["{version}"]
+"docs/conf.py" = ["{version}"]
+
```

