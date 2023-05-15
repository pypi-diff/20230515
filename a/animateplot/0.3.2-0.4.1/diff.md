# Comparing `tmp/animateplot-0.3.2-py3-none-any.whl.zip` & `tmp/animateplot-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18393 bytes, number of entries: 12
+Zip file size: 18252 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       37 b- defN 23-May-14 02:31 animateplot/__init__.py
--rw-rw-r--  2.0 unx     3269 b- defN 23-May-14 02:31 animateplot/animat_plot.py
+-rw-rw-r--  2.0 unx     3264 b- defN 23-May-14 04:14 animateplot/animat_plot.py
 -rw-rw-r--  2.0 unx       47 b- defN 23-Mar-06 03:21 animateplot/video/__init__.py
 -rw-rw-r--  2.0 unx      138 b- defN 23-Mar-06 03:02 animateplot/video/exceptions_animateplot.py
--rw-rw-r--  2.0 unx     2122 b- defN 23-Mar-06 03:51 animateplot/video/video.py
+-rw-rw-r--  2.0 unx     2319 b- defN 23-May-14 04:29 animateplot/video/video.py
 -rw-rw-r--  2.0 unx       35 b- defN 23-Mar-04 00:27 animatplot/__init__.py
 -rw-rw-r--  2.0 unx     2321 b- defN 23-Mar-04 05:05 animatplot/animat_plot.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2180 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      993 b- defN 23-May-14 02:40 animateplot-0.3.2.dist-info/RECORD
-12 files, 46395 bytes uncompressed, 16713 bytes compressed:  64.0%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-May-15 05:22 animateplot-0.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1849 b- defN 23-May-15 05:22 animateplot-0.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-15 05:22 animateplot-0.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-15 05:22 animateplot-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      993 b- defN 23-May-15 05:22 animateplot-0.4.1.dist-info/RECORD
+12 files, 46256 bytes uncompressed, 16572 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: animatplot/__init__.py
 Comment: 
 
 Filename: animatplot/animat_plot.py
 Comment: 
 
-Filename: animateplot-0.3.2.dist-info/LICENSE
+Filename: animateplot-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: animateplot-0.3.2.dist-info/METADATA
+Filename: animateplot-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: animateplot-0.3.2.dist-info/WHEEL
+Filename: animateplot-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: animateplot-0.3.2.dist-info/top_level.txt
+Filename: animateplot-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: animateplot-0.3.2.dist-info/RECORD
+Filename: animateplot-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## animateplot/animat_plot.py

```diff
@@ -83,15 +83,15 @@
           imgs_imread.append(imageio.imread(img))
         imageio.mimsave(path,imgs_imread,fps=fps)
     ping_total = time.time() - time_init
     print(f'{path} saved in {ping_total:.1f}s')
 
   
   def render_mp4(self,path_video,fps=8.7):
-    render_video = RenderVideo(self.pattern_dir,fps=fps)
+    render_video = RenderVideo(self.images,fps=fps)
     render_video.render_mp4(path_video)
 
 
 
   def __pattern_dir_check(self):
     if not os.path.isdir(self.pattern_dir):
       os.mkdir(self.pattern_dir)
```

## animateplot/video/video.py

```diff
@@ -5,22 +5,25 @@
 
 
 
 class RenderVideo:
     __dir_pattern_imgs = '.data'
     
     
-    def __init__(self,dir:str,fps:int=8.7) -> None:
-        if os.path.isdir(dir):
-            self.__dir_pattern_imgs = dir
-            self.__fps = fps
-            self.__images = [file for file in glob.glob(self.__dir_pattern_imgs+'/*.png')]
-            self.__images.sort(key=os.path.getmtime)
-        else:
-            raise DirectoryNotExists(f'the pathDir {dir} not exist or not is a directory',dir)
+    def __init__(self,list_images:list,fps:int=8.7) -> None:
+        self.__images = list_images
+        self.__fps = fps# [file for file in glob.glob(self.__dir_pattern_imgs+'/*.png')]
+        self.__images.sort(key=os.path.getmtime)
+        # if os.path.isdir(dir):
+        #     self.__dir_pattern_imgs = dir
+        #     self.__fps = fps
+        #     self.__images = [file for file in glob.glob(self.__dir_pattern_imgs+'/*.png')]
+        #     self.__images.sort(key=os.path.getmtime)
+        # else:
+        #     raise DirectoryNotExists(f'the pathDir {dir} not exist or not is a directory',dir)
     
     
     def render_mp4(self,path_video:str):
         first_img = cv2.imread(self.__images[0])#os.path.join(self.__dir_pattern_imgs,self.__images[0]))
         y,x,_ = first_img.shape
         
         video = cv2.VideoWriter(path_video,cv2.VideoWriter_fourcc(*'mp4v'),self.__fps,(x,y))
```

## Comparing `animateplot-0.3.2.dist-info/LICENSE` & `animateplot-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `animateplot-0.3.2.dist-info/METADATA` & `animateplot-0.4.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animateplot
-Version: 0.3.2
+Version: 0.4.1
 Summary: Library for generate gif or video from plots
 Home-page: https://github.com/reinanbr/dreams
 Author: Reinan Br
 Author-email: slimchatuba@gmail.com
 License: BSD v3
 Keywords: gif video plot
 Description-Content-Type: text/markdown
@@ -12,18 +12,18 @@
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: imageio
 Requires-Dist: opencv-python
 
 <div align='center'>
 
-<img height='200'  width='200' src='imgs/logo.png'>
+<img height='200'  width='200' src='https://raw.githubusercontent.com/reinanbr/animatPlot/main/imgs/logo.png'>
 <h2>AnimatePlot</h2>
 
-<p> Making video/gif from plot's</p>
+<p> Making video from plot's</p>
 <a href='#'><img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/reinanbr/animatPlot?logo=codefactor">
 </a><img alt="CircleCI" src="https://img.shields.io/circleci/build/github/reinanbr/animatPlot">
 <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/reinanbr/animatPlot">
 
 <br/>
 <a href='https://pypi.org/project/animateplot/'><img src='https://img.shields.io/pypi/v/animateplot'></a>
 <a href='#'><img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/animateplot"></a>
@@ -35,58 +35,40 @@
 </div>
 
 
 
 ### Examples 
 
 
-#### Gif 
+#### sigmoid function
 
 ```py
+import matplotlib.pyplot as plt
+from animateplot import AnimatePlot as Ap
 import numpy as np
-import matplotlib.pyplot as ply
-from animateplot import AnimatPlot # import AnimatPlot
 
-
-x = np.linspace(-10,10,200)
-np.seterr(all="ignore")
+plt.style.use('seaborn')
 
 def sig(x):
   return 1/(1+np.exp(-x))
 
 def call_plt(plt,y,x):
-  plt.style.use('seaborn')
   plt.plot(x,y)
   plt.title('sigmoid function')
   plt.xlabel('x')
   plt.ylabel('y')
   plt.xlim(-10,10)
   plt.ylim(0,1)
   return plt
 
+anime = Ap(erf,x,callback_plot=callback_plot)
 
-def test_render_gif():
-    anime = AnimatPlot(sig,x,callback_plot=call_plt)
-    anime.delete_cache()
-    anime.render_cache()
-    anime.render_gif('tests/gifs/sigmoid.gif')
-
-
+anime.render_cache()
+anime.render_mp4('sigmoid.mp4',fps=10)
 
-test_render_gif()
-```
-```sh
-logs:
-ended saved cache images! 
-[200 images saved in 30.9s | speed: 6.5/img/s | ping: 15.5ms]
-[Figure size 576x396 with 0 Axes]
-```
-saving the files from cache:
-```py
-anime.render_gif(path='plot.gif',fps=8.7)
 ```
-```sh
-logs: plot.gif saved in 6.8s
-```
-<img src='https://github.com/reinanbr/animatPlot/blob/main/imgs/plot%20(9).gif?raw=true'>
 
+results:
 
+<br/>
+
+<img src='https://github.com/reinanbr/animatPlot/blob/main/imgs/plot%20(9).gif?raw=true'>
```

## Comparing `animateplot-0.3.2.dist-info/RECORD` & `animateplot-0.4.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 animateplot/__init__.py,sha256=rha9Po1LeuTNRcNSS2pmF70S4xi2NF68ZYxrVDp_ryQ,37
-animateplot/animat_plot.py,sha256=bHmw4F_f2O-FgBxAevFsW5I01REvkPD9trK0fJ9IuL4,3269
+animateplot/animat_plot.py,sha256=urPYXwD0bNld5LMVq-WyRUsiiZor2eKrGaNt-V4Pt70,3264
 animateplot/video/__init__.py,sha256=lU7hqVr9gzCc9pTI1sBbWsYTUTIbBXfFw1ZP-p-iRM0,47
 animateplot/video/exceptions_animateplot.py,sha256=1EiEDXmQCLsn1chxIfncysmNTbq4r81487KFt5Q62Yk,138
-animateplot/video/video.py,sha256=BBk3eJ4yZqXfVt99vKRWsewXcjWxS1D9HJwTRX_HzmM,2122
+animateplot/video/video.py,sha256=3QvPLOLH8a5aeWW7xdemTrTJ8AdBvtWFstuT8FpNBoY,2319
 animatplot/__init__.py,sha256=P-8fjpAfXPCf4ONnEmO9HL_pxFhqmFa1qH961fH45Bs,35
 animatplot/animat_plot.py,sha256=sEG55Z_yeTSK8WsQtdN50R6CZhgp72wcIRFZzz3K_5g,2321
-animateplot-0.3.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-animateplot-0.3.2.dist-info/METADATA,sha256=6vEZxN_n-UtzzATwRfLiF5ZKYqH1SZ5nT-uf9P9be0w,2180
-animateplot-0.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-animateplot-0.3.2.dist-info/top_level.txt,sha256=Q3eAcf4CPjJRiYa7ZsW-n520lYXLpdLh8bTAa7kNXtk,12
-animateplot-0.3.2.dist-info/RECORD,,
+animateplot-0.4.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+animateplot-0.4.1.dist-info/METADATA,sha256=9hpAue3_H5_awGxrksAcEe4Gi1uqO-Ky0Bk4IAmQdQc,1849
+animateplot-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+animateplot-0.4.1.dist-info/top_level.txt,sha256=Q3eAcf4CPjJRiYa7ZsW-n520lYXLpdLh8bTAa7kNXtk,12
+animateplot-0.4.1.dist-info/RECORD,,
```

