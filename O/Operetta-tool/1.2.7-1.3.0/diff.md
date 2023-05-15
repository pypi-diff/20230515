# Comparing `tmp/Operetta_tool-1.2.7.tar.gz` & `tmp/Operetta_tool-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.2.7.tar", last modified: Mon Mar 20 21:06:47 2023, max compression
+gzip compressed data, was "Operetta_tool-1.3.0.tar", last modified: Mon May 15 20:44:10 2023, max compression
```

## Comparing `Operetta_tool-1.2.7.tar` & `Operetta_tool-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.345867 Operetta_tool-1.2.7/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.2.7/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.2.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.334081 Operetta_tool-1.2.7/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-03-20 21:06:47.345867 Operetta_tool-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.344866 Operetta_tool-1.2.7/operetta/
--rw-rw-rw-   0        0        0      153 2023-03-20 21:02:36.000000 Operetta_tool-1.2.7/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.2.7/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    31809 2023-03-20 21:02:20.000000 Operetta_tool-1.2.7/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-03-20 21:06:47.346867 Operetta_tool-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-03-20 21:02:40.000000 Operetta_tool-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 20:44:10.660038 Operetta_tool-1.3.0/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-15 20:44:10.650637 Operetta_tool-1.3.0/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-05-15 20:44:09.000000 Operetta_tool-1.3.0/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-15 20:44:10.000000 Operetta_tool-1.3.0/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 20:44:09.000000 Operetta_tool-1.3.0/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-15 20:44:09.000000 Operetta_tool-1.3.0/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 20:44:09.000000 Operetta_tool-1.3.0/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-05-15 20:44:10.660038 Operetta_tool-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 20:44:10.659043 Operetta_tool-1.3.0/operetta/
+-rw-rw-rw-   0        0        0      153 2023-05-15 20:41:56.000000 Operetta_tool-1.3.0/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.0/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    47602 2023-05-15 20:38:05.000000 Operetta_tool-1.3.0/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-05-15 20:44:10.661042 Operetta_tool-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-05-15 20:41:24.000000 Operetta_tool-1.3.0/setup.py
```

### Comparing `Operetta_tool-1.2.7/LICENSE` & `Operetta_tool-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.3.0/Operetta_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.2.7
+Version: 1.3.0
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.2.7/PKG-INFO` & `Operetta_tool-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.2.7
+Version: 1.3.0
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.2.7/README.md` & `Operetta_tool-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/operetta/jbsicon.ico` & `Operetta_tool-1.3.0/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/operetta/operetta_annotation.py` & `Operetta_tool-1.3.0/operetta/operetta_annotation.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,399 +13,458 @@
 from tqdm import tqdm
 import tifffile as tiff
 from joblib import Parallel, delayed
 import math
 import gc
 import warnings
 import tkinter as tk 
-from tkinter import ttk
+from tkinter import ttk, Text
 from skimage import io, filters
 import pkg_resources
 
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
     
 def split_chanels(path_to_images:str, path_to_save:str):
     
+    try:
     
-    
-    chanels=os.listdir(path_to_images)
-    chanels=[re.sub('.*-','',x)  for x in chanels if 'tiff' in x]
-    chanels=[re.sub('sk.*','',x)  for x in chanels if 'tiff' in x]
-    
-    chanels = np.unique(chanels).tolist()
-    
-    for ch in chanels:
-            
+        chanels=os.listdir(path_to_images)
+        chanels=[re.sub('.*-','',x)  for x in chanels if 'tiff' in x]
+        chanels=[re.sub('sk.*','',x)  for x in chanels if 'tiff' in x]
         
-        if not os.path.exists(os.path.join(path_to_save, str(ch))):
-            os.mkdir(os.path.join(path_to_save, str(ch)))
-    
-  
+        chanels = np.unique(chanels).tolist()
         
-        images_list=os.listdir(path_to_images)
-    
-        images_list=[x for x in images_list if str(ch) in x]
-        images_list = images_list + ['Index.idx.xml']
+        for ch in chanels:
+                
+            
+            if not os.path.exists(os.path.join(path_to_save, str(ch))):
+                os.mkdir(os.path.join(path_to_save, str(ch)))
+        
+      
+            
+            images_list=os.listdir(path_to_images)
         
-        if not os.path.exists(os.path.join(path_to_save, str(ch))):
-            os.mkdir(os.path.join(path_to_save, str(ch)))
+            images_list=[x for x in images_list if str(ch) in x]
+            images_list = images_list + ['Index.idx.xml']
             
-        for image in images_list:
-            shutil.copy(os.path.join(path_to_images,image),os.path.join(os.path.join(path_to_save, str(ch))))
+            if not os.path.exists(os.path.join(path_to_save, str(ch))):
+                os.mkdir(os.path.join(path_to_save, str(ch)))
+                
+            for image in images_list:
+                shutil.copy(os.path.join(path_to_images,image),os.path.join(os.path.join(path_to_save, str(ch))))
+                
+    except:
+        print("Something went wrong. Check the function input data and try again!")
     
     
+def xml_load(path_to_opera_xml:str):
     
+    try:
     
+        name = []
+        x = []
+        y = []
+        x_res = []
+        y_res = []
+        channel_num = []
+        channel_name = []
+        max_intensity = []
+        z_spacing = []
+        excitation_wavelength = []
+        emissio_wavelength = []
+        magnification = []
+        
+        df = {'name':name, 'x':x, 'y':y}
+        
+        
+        with open(path_to_opera_xml) as topo_file:
+            for line in topo_file:
+               if line.startswith('    <Image Version="1">'):
+                   break
+            topo_file= topo_file.readlines()
+            
+            for line in topo_file:
+                if str('PositionX') in line:
+                    df['x'].append(float(re.sub('<PositionX Unit="m">','', re.sub('</PositionX>','',line)).replace(' ', '')))
+                elif str('PositionY') in line:
+                    df['y'].append(float(re.sub('<PositionY Unit="m">','', re.sub('</PositionY>','',line)).replace(' ', '')))
+                elif str('URL') in line:
+                    df['name'].append(re.sub('</URL>','', re.sub('<URL>','',line)).replace(' ', ''))
+                elif str('<ImageResolutionX Unit="m">') in line and float(re.sub('</ImageResolutionX>','', re.sub('<ImageResolutionX Unit="m">','',line)).replace(' ', '')) not in x_res:
+                    x_res.append(float(re.sub('</ImageResolutionX>','', re.sub('<ImageResolutionX Unit="m">','',line)).replace(' ', '')))
+                elif str('<ImageResolutionY Unit="m">') in line and float(re.sub('</ImageResolutionY>','', re.sub('<ImageResolutionY Unit="m">','',line)).replace(' ', '')) not in y_res:
+                    y_res.append(float(re.sub('</ImageResolutionY>','', re.sub('<ImageResolutionY Unit="m">','',line)).replace(' ', '')))
+                elif str('<ChannelID>') in line and re.sub('</ChannelID>','', re.sub('<ChannelID>','',line)).replace(' ', '') not in channel_num:
+                    channel_num.append(re.sub('</ChannelID>','', re.sub('<ChannelID>','',line)).replace(' ', ''))
+                elif str('<ChannelName>') in line and re.sub('</ChannelName>','', re.sub('<ChannelName>','',line)).replace(' ', '') not in channel_name:
+                    channel_name.append(re.sub('</ChannelName>','', re.sub('<ChannelName>','',line)).replace(' ', ''))
+                elif str('<MaxIntensity>') in line and int(re.sub('</MaxIntensity>','', re.sub('<MaxIntensity>','',line)).replace(' ', '')) not in max_intensity:
+                    max_intensity.append(int(re.sub('</MaxIntensity>','', re.sub('<MaxIntensity>','',line)).replace(' ', '')))
+                elif str('<AbsPositionZ Unit="m">') in line and float(re.sub('</AbsPositionZ>','', re.sub('<AbsPositionZ Unit="m">','',line)).replace(' ', '')) not in z_spacing:
+                    z_spacing.append(float(re.sub('</AbsPositionZ>','', re.sub('<AbsPositionZ Unit="m">','',line)).replace(' ', '')))
+                elif str('<MainExcitationWavelength Unit="nm">') in line and int(re.sub('</MainExcitationWavelength>','', re.sub('<MainExcitationWavelength Unit="nm">','',line)).replace(' ', '')) not in excitation_wavelength:
+                    excitation_wavelength.append(int(re.sub('</MainExcitationWavelength>','', re.sub('<MainExcitationWavelength Unit="nm">','',line)).replace(' ', '')))
+                elif str('<MainEmissionWavelength Unit="nm">') in line and int(re.sub('</MainEmissionWavelength>','', re.sub('<MainEmissionWavelength Unit="nm">','',line)).replace(' ', '')) not in emissio_wavelength:
+                    emissio_wavelength.append(int(re.sub('</MainEmissionWavelength>','', re.sub('<MainEmissionWavelength Unit="nm">','',line)).replace(' ', '')))
+                elif str('<ObjectiveMagnification Unit="">') in line and int(re.sub('</ObjectiveMagnification>','', re.sub('<ObjectiveMagnification Unit="">','',line)).replace(' ', '')) not in magnification:
+                    magnification.append(int(re.sub('</ObjectiveMagnification>','', re.sub('<ObjectiveMagnification Unit="">','',line)).replace(' ', '')))
+           
+            
+           
+                    
+        
+        df = pd.DataFrame(df)
+        df['name'] = [re.sub('p.*', '', x) for x in df['name']]
+        
+        df['y'] = df['y']*-1
+        
+        
+        df = df.drop_duplicates()
+        df['num'] = range(1,len(df['name'])+1)
+        
+        df = df.reset_index(drop = True)
+        
     
-
-def xml_load(path_to_opera_xml:str):
+        metadata = {'chanel_name':channel_name, 'chanel_number':channel_num, 'X_resolution[m]': x_res, 'Y_resolution[m]': y_res, 'max_intensity[nm]':max_intensity, 'z_spacing':np.mean(z_spacing), 'excitation_wavelength[nm]':excitation_wavelength, 'emissio_wavelength[nm]':emissio_wavelength, 'magnification[x]':magnification}
+        
+        
+        return df, metadata  
     
-    name = []
-    x = []
-    y = []
+    except:
+        print("Something went wrong. Check the function input data and try again!")
     
-    df = {'name':name, 'x':x, 'y':y}
     
+
+
+
+
+def detect_outlires(xml_file:pd.DataFrame, list_of_out:list = []):
     
-    with open(path_to_opera_xml) as topo_file:
-        for line in topo_file:
-           if line.startswith('    <Image Version="1">'):
-               break
-        topo_file= topo_file.readlines()
+    try:
+        
+        if len(list_of_out) != 0:
+            xml_file = xml_file[~xml_file.index.isin(list_of_out)]
         
-        for line in topo_file:
-            if str('PositionX') in line:
-                df['x'].append(float(re.sub('<PositionX Unit="m">','', re.sub('</PositionX>','',line)).replace(' ', '')))
-            elif str('PositionY') in line:
-                df['y'].append(float(re.sub('<PositionY Unit="m">','', re.sub('</PositionY>','',line)).replace(' ', '')))
-            elif str('URL') in line:
-                df['name'].append(re.sub('</URL>','', re.sub('<URL>','',line)).replace(' ', ''))
+        def outlires_image_detect(xml_file):
+               
+            x  = np.interp(xml_file['x'], (min(xml_file['x']), max(xml_file['x'])), (0, 100))
+            y = np.interp(xml_file['y'], (min(xml_file['y']), max(xml_file['y'])), (0, 100))
+            
+            
+            fig, ax = plt.subplots(figsize=(30, 30))
+            ax.scatter(x , y , s= 700, c='red', alpha=0.7, marker = 's',  edgecolor="none")
+            
+            ax.set_axis_off()
+            ax.invert_yaxis()
+    
+            for n, i in enumerate(xml_file.index):
+                ax.annotate(i, (x[n] , y[n] ), xytext=(0, 0), textcoords="offset pixels", ha='center', va='center',
+                     fontsize=8, fontweight='bold', color='yellow')
+                
                 
+            physical_size = (16, 14)  # Example size in inches
+            pixels_per_inch = 300  # Example DPI of display device
+            pixel_size = tuple(int(physical_size[i] * pixels_per_inch) for i in (1, 0))
                 
+            fig.set_size_inches(*physical_size)
+            fig.set_dpi(pixels_per_inch)
+            
+            canvas = FigureCanvas(fig)
+            canvas.draw()
+            image = np.array(canvas.renderer.buffer_rgba())
     
-    df = pd.DataFrame(df)
-    df['name'] = [re.sub('p.*', '', x) for x in df['name']]
     
-    df['y'] = df['y']*-1
+            cv2.namedWindow('Image', cv2.WINDOW_NORMAL)
     
+                
+            cv2.resizeWindow('Image', *pixel_size)
+            cv2.imshow('Image', image)
+            
     
-    df = df.drop_duplicates()
-    df['num'] = range(1,len(df['name'])+1)
+            
+            cv2.waitKey(0)
+            
+            
+            cv2.destroyAllWindows()
+            
+            return fig
+    
+        fig = outlires_image_detect(xml_file)
+        
+        return xml_file, fig
     
-    df = df.reset_index(drop = True)
+    except:
+        print("Something went wrong. Check the function input data and try again!")
     
-    return df
-
 
 
-def detect_outlires(xml_file:pd.DataFrame, list_of_out:list = []):
-    if len(list_of_out) != 0:
-        xml_file = xml_file[~xml_file.index.isin(list_of_out)]
-    
-    def outlires_image_detect(xml_file):
+def repair_blanks(xml_file:pd.DataFrame):
+   
+    try:
+   
+        x = np.unique(xml_file['x'])
+        
+        y = np.unique(xml_file['y'])
+        
+        
+        
+        #
+        x_n = []
+        for ix in x:
+           x_n.append(len(xml_file['x'][xml_file['x'] == ix]))
+           
+        mfqx = [abs(xv) for xv in x_n]
+           
+        mfqx = max(set(mfqx),key = mfqx.count)
+        
            
-        x  = np.interp(xml_file['x'], (min(xml_file['x']), max(xml_file['x'])), (0, 100))
-        y = np.interp(xml_file['y'], (min(xml_file['y']), max(xml_file['y'])), (0, 100))
+        df_x = pd.DataFrame({'x':x, 'n': x_n})
+        #
         
         
-        fig, ax = plt.subplots(figsize=(30, 30))
-        ax.scatter(x , y , s= 700, c='red', alpha=0.7, marker = 's',  edgecolor="none")
         
-        ax.set_axis_off()
-        ax.invert_yaxis()
-
-        for n, i in enumerate(xml_file.index):
-            ax.annotate(i, (x[n] , y[n] ), xytext=(0, 0), textcoords="offset pixels", ha='center', va='center',
-                 fontsize=8, fontweight='bold', color='yellow')
-            
-            
-        physical_size = (16, 14)  # Example size in inches
-        pixels_per_inch = 300  # Example DPI of display device
-        pixel_size = tuple(int(physical_size[i] * pixels_per_inch) for i in (1, 0))
-            
-        fig.set_size_inches(*physical_size)
-        fig.set_dpi(pixels_per_inch)
+        #
+        y_n = []
+        for iy in y:
+           y_n.append(len(xml_file['y'][xml_file['y'] == iy]))
         
-        canvas = FigureCanvas(fig)
-        canvas.draw()
-        image = np.array(canvas.renderer.buffer_rgba())
-
-
-        cv2.namedWindow('Image', cv2.WINDOW_NORMAL)
-
-            
-        cv2.resizeWindow('Image', *pixel_size)
-        cv2.imshow('Image', image)
         
-
+        mfqy = [abs(xy) for xy in y_n]
+           
+        mfqy = max(set(mfqy),key = mfqy.count)
         
-        cv2.waitKey(0)
         
+        df_y = pd.DataFrame({'y':y, 'n': y_n})
         
-        cv2.destroyAllWindows()
+        #
         
-        return fig
-
-    fig = outlires_image_detect(xml_file)
+        df_x = df_x[df_x['n'] < mfqx]
+        
+        df_y = df_y[df_y['n'] < mfqy]
+        
+        xtml = xml_file.copy()
+        
+        xtml['XY'] = xtml['x'].astype(str) + xtml['y'].astype(str)
+        
+        b = 0
+        for xi in df_x['x']:
+            for yi in df_y['y']:
+                if str(str(xi)+str(yi)) not in list(xtml['XY']):
+                    b += 1
+                    new_row = {'name' : 'blank' + str(b), 'x': float(xi) , 'y': float(yi), 'num': 'NULL'}
+                    xml_file = xml_file.append(new_row, ignore_index=True)
     
-    return xml_file, fig
+                
+        
+        
+        
+        def outlires_image_detect(xml_file):
+               
+            x  = np.interp(xml_file['x'], (min(xml_file['x']), max(xml_file['x'])), (0, 100))
+            y = np.interp(xml_file['y'], (min(xml_file['y']), max(xml_file['y'])), (0, 100))
+            
+            
+            fig, ax = plt.subplots(figsize=(30, 30))
+            ax.scatter(x , y , s= 700, c='red', alpha=0.7, marker = 's',  edgecolor="none")
+            
+            ax.set_axis_off()
+            ax.invert_yaxis()
     
-
-
-def repair_blanks(xml_file:pd.DataFrame):
-   
-   
-    x = np.unique(xml_file['x'])
+            for n, i in enumerate(xml_file.index):
+                ax.annotate(i, (x[n] , y[n] ), xytext=(0, 0), textcoords="offset pixels", ha='center', va='center',
+                     fontsize=8, fontweight='bold', color='yellow')
+                
+                
+            physical_size = (16, 14)  
+            pixels_per_inch = 300  
+            pixel_size = tuple(int(physical_size[i] * pixels_per_inch) for i in (1, 0))
+                
+            fig.set_size_inches(*physical_size)
+            fig.set_dpi(pixels_per_inch)
+            
+            canvas = FigureCanvas(fig)
+            canvas.draw()
+            image = np.array(canvas.renderer.buffer_rgba())
     
-    y = np.unique(xml_file['y'])
     
+            cv2.namedWindow('Image', cv2.WINDOW_NORMAL)
     
+                
+            cv2.resizeWindow('Image', *pixel_size)
+            cv2.imshow('Image', image)
+            
     
-    #
-    x_n = []
-    for ix in x:
-       x_n.append(len(xml_file['x'][xml_file['x'] == ix]))
-       
-    mfqx = [abs(xv) for xv in x_n]
-       
-    mfqx = max(set(mfqx),key = mfqx.count)
+            
+            cv2.waitKey(0)
+            
+            
+            cv2.destroyAllWindows()
+            
+            return fig
     
-       
-    df_x = pd.DataFrame({'x':x, 'n': x_n})
-    #
+        fig = outlires_image_detect(xml_file)
+        
+        return xml_file, fig
     
+    except:
+        print("Something went wrong. Check the function input data and try again!")
+
+  
     
+def image_sequences(opera_coordinates:pd.DataFrame):
     
-    #
-    y_n = []
-    for iy in y:
-       y_n.append(len(xml_file['y'][xml_file['y'] == iy]))
+    try:
     
+        y = list(np.unique(opera_coordinates['y']))
+        y.sort()
     
-    mfqy = [abs(xy) for xy in y_n]
-       
-    mfqy = max(set(mfqy),key = mfqy.count)
     
+        queue_images=[]
     
-    df_y = pd.DataFrame({'y':y, 'n': y_n})
+        for table in y:
+            tmp = opera_coordinates[opera_coordinates['y'] == table]
+            tmp = tmp.sort_values(by=['x'])
+            queue_images = queue_images + list(tmp['name'])
     
-    #
+        image_dictinary=pd.DataFrame()
+        image_dictinary['queue']=queue_images
+        image_dictinary['image_num']=range(1,len(image_dictinary['queue'])+1)
+        
+        img_length = len(list(np.unique(opera_coordinates['y'])))
+        img_width = len(list(np.unique(opera_coordinates['x'])))
+        
+        return image_dictinary, img_length, img_width
     
-    df_x = df_x[df_x['n'] < mfqx]
+    except:
+        print("Something went wrong. Check the function input data and try again!")
+
+
+
+def image_concatenate(path_to_images:str, imgs:pd.DataFrame, metadata, img_length:int, img_width:int, overlap:int, chanels:list, n_thread:int):
+     
+    try:
+        
+        for obj in gc.get_objects():   
+            if isinstance(obj, h5py.File):  
+                try:
+                    obj.close()
+                except:
+                    pass 
+                
+                
+        if os.path.exists(os.path.join(path_to_images, 'images.h5')):
+            os.remove(os.path.join(path_to_images,'images.h5'))
+            
+        if os.path.exists(os.path.join(path_to_images,'images2.h5')):
+            os.remove(os.path.join(path_to_images,'images2.h5'))
+        
+        def par_1(q, path_to_images, img_width, imgs, black_img, st, ch, overlap):
+            stop =  img_width * (q+1)
+            start = img_width * q
+            tmp = imgs['queue'][start:stop]
+            
+            list_p = []
+            for t in tmp:
+                if 'blank' in t:
+                    list_p.append(str(t))
+                else:
+                    list_p.append(str([f for f in tmp_img if str(re.sub('\n','', str(t)) + 'p') in f and str('p'+st) in f][0]))
+                
+            data = []
+            for img in list_p:
+                if os.path.exists(os.path.join(path_to_images, img)):
+                    data.append(cv2.imread(os.path.join(path_to_images, img), cv2.IMREAD_ANYDEPTH))
+                else:
+                    data.append(black_img)
+                 
     
-    df_y = df_y[df_y['n'] < mfqy]
     
-    xtml = xml_file.copy()
+            row, col = data[0].shape
+            for n,i in enumerate(data):
+                data[n] = data[n][:, int(col*overlap/2):-int(col*overlap/2)]
+                         
     
-    xtml['XY'] = xtml['x'].astype(str) + xtml['y'].astype(str)
     
-    b = 0
-    for xi in df_x['x']:
-        for yi in df_y['y']:
-            if str(str(xi)+str(yi)) not in list(xtml['XY']):
-                b += 1
-                new_row = {'name' : 'blank' + str(b), 'x': float(xi) , 'y': float(yi), 'num': 'NULL'}
-                xml_file = xml_file.append(new_row, ignore_index=True)
-
             
-    
-    
-    
-    def outlires_image_detect(xml_file):
-           
-        x  = np.interp(xml_file['x'], (min(xml_file['x']), max(xml_file['x'])), (0, 100))
-        y = np.interp(xml_file['y'], (min(xml_file['y']), max(xml_file['y'])), (0, 100))
+            data = np.concatenate(data, axis = 1)
+            images_tmp.create_dataset('lane_' + str(q) + '-deep_' + str(st) + '-chanel_' + str(ch),  data=data)
+            del data
         
         
-        fig, ax = plt.subplots(figsize=(30, 30))
-        ax.scatter(x , y , s= 700, c='red', alpha=0.7, marker = 's',  edgecolor="none")
         
-        ax.set_axis_off()
-        ax.invert_yaxis()
-
-        for n, i in enumerate(xml_file.index):
-            ax.annotate(i, (x[n] , y[n] ), xytext=(0, 0), textcoords="offset pixels", ha='center', va='center',
-                 fontsize=8, fontweight='bold', color='yellow')
-            
-            
-        physical_size = (16, 14)  
-        pixels_per_inch = 300  
-        pixel_size = tuple(int(physical_size[i] * pixels_per_inch) for i in (1, 0))
-            
-        fig.set_size_inches(*physical_size)
-        fig.set_dpi(pixels_per_inch)
+        images_list=os.listdir(path_to_images)
+        deep = np.unique([re.sub('-.*','', re.sub('.*p', '', n)) for n in images_list if '.tiff' in n])
         
-        canvas = FigureCanvas(fig)
-        canvas.draw()
-        image = np.array(canvas.renderer.buffer_rgba())
-
-
-        cv2.namedWindow('Image', cv2.WINDOW_NORMAL)
-
-            
-        cv2.resizeWindow('Image', *pixel_size)
-        cv2.imshow('Image', image)
+       
         
-
+        for ch in chanels:
+            images_tmp2 = h5py.File(os.path.join(path_to_images, 'images2.h5'),   mode = 'a')
         
-        cv2.waitKey(0)
+            tmp_img = [i for i in images_list if ch in i]
+            
+            black_img = cv2.imread(os.path.join(path_to_images, tmp_img[0]), cv2.IMREAD_ANYDEPTH)
+            black_img.fill(0) 
+            for st in tqdm(deep):
+                images_tmp = h5py.File(os.path.join(path_to_images, 'images.h5'),   mode = 'a')
         
+               
+                Parallel(n_jobs=n_thread, prefer="threads")(delayed(par_1)(q, path_to_images, img_width, imgs, black_img, st, ch, overlap) for q in range(0,img_length))
         
-        cv2.destroyAllWindows()
+               
+                    
+                data = []
+                for q in range(0,img_length):
+                    data.append(images_tmp[[f for f in images_tmp.keys() if 'lane_' + str(q) + '-deep' in f][0]][:])
+                  
         
-        return fig
-
-    fig = outlires_image_detect(xml_file)
-    
-    return xml_file, fig
-
-  
-    
-def image_sequences(opera_coordinates:pd.DataFrame):
-    
-    y = list(np.unique(opera_coordinates['y']))
-    y.sort()
-
-
-    queue_images=[]
-
-    for table in y:
-        tmp = opera_coordinates[opera_coordinates['y'] == table]
-        tmp = tmp.sort_values(by=['x'])
-        queue_images = queue_images + list(tmp['name'])
-
-    image_dictinary=pd.DataFrame()
-    image_dictinary['queue']=queue_images
-    image_dictinary['image_num']=range(1,len(image_dictinary['queue'])+1)
-    
-    img_length = len(list(np.unique(opera_coordinates['y'])))
-    img_width = len(list(np.unique(opera_coordinates['x'])))
-    
-    return image_dictinary, img_length, img_width
-
-
-
-
-
-def image_concatenate(path_to_images:str, imgs:pd.DataFrame, img_length:int, img_width:int, overlap:int, chanels:list, n_thread:int):
-     
-    
-    for obj in gc.get_objects():   
-        if isinstance(obj, h5py.File):  
-            try:
-                obj.close()
-            except:
-                pass 
-            
-            
-    if os.path.exists(os.path.join(path_to_images, 'images.h5')):
-        os.remove(os.path.join(path_to_images,'images.h5'))
-        
-    if os.path.exists(os.path.join(path_to_images,'images2.h5')):
-        os.remove(os.path.join(path_to_images,'images2.h5'))
-    
-    def par_1(q, path_to_images, img_width, imgs, black_img, st, ch, overlap):
-        stop =  img_width * (q+1)
-        start = img_width * q
-        tmp = imgs['queue'][start:stop]
-        
-        list_p = []
-        for t in tmp:
-            if 'blank' in t:
-                list_p.append(str(t))
-            else:
-                list_p.append(str([f for f in tmp_img if str(re.sub('\n','', str(t)) + 'p') in f and str('p'+st) in f][0]))
-            
-        data = []
-        for img in list_p:
-            if os.path.exists(os.path.join(path_to_images, img)):
-                data.append(cv2.imread(os.path.join(path_to_images, img), cv2.IMREAD_ANYDEPTH))
-            else:
-                data.append(black_img)
+                images_tmp.close()
+        
+                os.remove(os.path.join(path_to_images, 'images.h5'))
+                
              
-
-
-        row, col = data[0].shape
-        for n,i in enumerate(data):
-            data[n] = data[n][:, int(col*overlap/2):-int(col*overlap/2)]
-                     
-
-
+                    
+                row, col = data[0].shape
+                for n,i in enumerate(data):
+                    data[n] = data[n][int(row*overlap/2):-int(row*overlap/2), :]
+                    
+         
+                    
+            
+                   
+                 
+                data = np.concatenate(data, axis = 0)
+                
+                images_tmp2.create_dataset('deep_' + str(st) + '-chanel_' + str(ch),  data=data)
         
-        data = np.concatenate(data, axis = 1)
-        images_tmp.create_dataset('lane_' + str(q) + '-deep_' + str(st) + '-chanel_' + str(ch),  data=data)
-        del data
-    
+            data = []
+            for q in tqdm(images_tmp2.keys()):
     
     
-    images_list=os.listdir(path_to_images)
-    deep = np.unique([re.sub('-.*','', re.sub('.*p', '', n)) for n in images_list if '.tiff' in n])
     
-   
-    
-    for ch in chanels:
-        images_tmp2 = h5py.File(os.path.join(path_to_images, 'images2.h5'),   mode = 'a')
+          
+                data.append(images_tmp2[q][:])
+                    
     
-        tmp_img = [i for i in images_list if ch in i]
+            data = np.stack(data)
+            
         
-        black_img = cv2.imread(os.path.join(path_to_images, tmp_img[0]), cv2.IMREAD_ANYDEPTH)
-        black_img.fill(0) 
-        for st in tqdm(deep):
-            images_tmp = h5py.File(os.path.join(path_to_images, 'images.h5'),   mode = 'a')
-    
-           
-            Parallel(n_jobs=n_thread, prefer="threads")(delayed(par_1)(q, path_to_images, img_width, imgs, black_img, st, ch, overlap) for q in range(0,img_length))
-    
-           
+            tiff.imsave('chanel_' + str(ch) + '.tiff', data,
+                           imagej=True,
+                           resolution=(metadata['X_resolution[m]'][0]*1000000, metadata['Y_resolution[m]'][0]*1000000),
+                           metadata={'spacing': metadata['z_spacing'], 'unit': 'um'}) 
                 
-            data = []
-            for q in range(0,img_length):
-                data.append(images_tmp[[f for f in images_tmp.keys() if 'lane_' + str(q) + '-deep' in f][0]][:])
-              
-    
-            images_tmp.close()
-    
-            os.remove(os.path.join(path_to_images, 'images.h5'))
+            images_tmp2.close()
             
-         
-                
-            row, col = data[0].shape
-            for n,i in enumerate(data):
-                data[n] = data[n][int(row*overlap/2):-int(row*overlap/2), :]
-                
-     
-                
-        
-               
-             
-            data = np.concatenate(data, axis = 0)
+            del data
             
-            images_tmp2.create_dataset('deep_' + str(st) + '-chanel_' + str(ch),  data=data)
-    
-        data = []
-        for q in tqdm(images_tmp2.keys()):
-
-
-
-      
-            data.append(images_tmp2[q][:])
-                
-
-        data = np.stack(data)
-        
-    
-        tiff.imwrite('chanel_' + str(ch) + '.tiff', data, imagej=True)
+            os.remove(os.path.join(path_to_images, 'images2.h5'))
             
-        images_tmp2.close()
-        
-        del data
-        
-        os.remove(os.path.join(path_to_images, 'images2.h5'))
-
+    except:
+        print("Something went wrong. Check the function input data and try again!")
 
 
 
 
 def z_projection(path_to_tiff:str, stack_check:str):
 
     if not os.path.exists(path_to_tiff):
@@ -439,24 +498,37 @@
             del thresholded_stack
             
             outlier_indices = list(np.where(mean_intensity > np.mean(mean_intensity) + np.std(mean_intensity))[0]) + list(np.where(mean_intensity < np.mean(mean_intensity) - np.std(mean_intensity))[0]) 
             
             stack = np.delete(stack, outlier_indices, axis=0)
             
             del mean_intensity, outlier_indices
+            
+            mean_zstack = np.mean(stack, axis=0)
+            std_zstack = np.std(stack, axis=0)
         
+            # calculate the z-score for each pixel
+            z_score = abs(stack - mean_zstack) / std_zstack
+            
+            del mean_zstack, std_zstack
         
-        
-        for n, d in enumerate(stack):    
-            stack[n] = (stack[n] / np.mean(stack[n])) * 65535/4
+            # identify pixels with z-scores above the threshold
+            stack[(z_score > 2.5) | (z_score < -2.5)] = np.nan
             
-          
-
+            del z_score
+        
+        stack = stack.astype(np.uint64)  
+        
+        for n, d in enumerate(stack):   
+            stack[n] = (stack[n] / np.mean(stack[n])) * (((2**16)-1) /  np.log(np.mean(stack[n])))
+            stack[n][stack[n] > ((2**16)-1)] = ((2**16)-1)
 
-         
+        stack[stack > ((2**16)-1)] = ((2**16)-1)
+        stack = stack.astype(np.uint16)   
+                
        
         window = tk.Tk()
         
         window.geometry("500x800")
         window.title("Z-PROJECTION")
     
         window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
@@ -568,15 +640,15 @@
         
         def active_changes():
                 
                
                 global img_gamma
                 
                 if projections_type.get() == 'avg':
-                    img = np.average(stack, axis=0).astype(np.uint16)      
+                    img = np.nanmean(stack, axis=0).astype(np.uint16)      
                 elif projections_type.get() == 'max':
                     img = np.max(stack, axis=0).astype(np.uint16)    
                 elif projections_type.get() == 'min':
                     img = np.min(stack, axis=0).astype(np.uint16)    
                 elif projections_type.get() == 'std':
                     img = np.std(stack, axis=0).astype(np.uint16)    
                 elif projections_type.get() == 'median':
@@ -616,15 +688,15 @@
                 img = (img * (factor))
                 
                 del img_norm
                 
                 
                 img = (img / np.max(img)) * 65535
 
-                img = img.astype(np.uint16)
+                img = np.round(img).astype(np.uint16)
             
                 
                 img_gamma = np.zeros((img.shape[0], img.shape[1], 3), dtype=np.uint16)
                 
                    
                
                 if color == 'green':
@@ -639,19 +711,19 @@
                     img_gamma[:,:,0] = img
         
                     
                 elif color == 'magenta':
                     img_gamma[:,:,0] = img
                     img_gamma[:,:,2] = img
                     
-                elif color == 'cyan':
+                elif color == 'yellow':
                     img_gamma[:,:,1] = img
                     img_gamma[:,:,2] = img
                 
-                elif color == 'yellow':
+                elif color == 'cyan':
                     img_gamma[:,:,0] = img
                     img_gamma[:,:,1] = img
                  
                 elif color == 'grey':
                     img_gamma = img
             
             
@@ -684,20 +756,20 @@
         display_image()
         
         
         def auto_adjust():
             
             projection = np.average(stack, axis=0)
 
-            tmin = int(np.mean(projection))/2
-            tmax = int(np.quantile(projection, 0.95))
+            tmin = int(np.mean(projection))/1.5
+            tmax = int(np.max(projection))
 
             
-            gamma.set(15)         
-            slider2.set(15)
+            gamma.set(20)         
+            slider2.set(20)
                      
             threshold_min.set(tmin)
             slider3_min.set(tmin)
             
             threshold_max.set(tmax)
             slider3_max.set(tmax)
             
@@ -738,143 +810,143 @@
         return img_gamma
 
 
 
 
 
 
-
-
 def merge_images(image_list:list):
     
-    intensity_factors = []
-    for bt in range(len(image_list)):
-        intensity_factors.append(1)
-        
-    def merge1():
-        global result
-        result = None
-        
-        for i, image in enumerate(image_list):
-            if result is None:
-                result = image.astype(float) * intensity_factors[i]
-            else:
-                result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
-        
-        result = result.astype('uint16')
-        
-        
- 
-       
-  
-    
-    window = tk.Tk()
+    try:
     
-    window.geometry("500x600")
-    window.title("MERGE CHANELS")
-
-    window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
-   
-
-   
-    tk.Label(window, text="").pack()
-    tk.Label(window, text="").pack()
-    
-    
-    label1 = tk.Label(window, text="Size", anchor="w")
-    label1.pack()
-    
-    # Create a slider widget
-    
-    size = tk.DoubleVar()
-    slider1 = tk.Scale(window, from_=0, to=100, orient=tk.HORIZONTAL, length=400, variable=size)
-    slider1.set(50)
-    slider1.pack()
-    
-    def update_slider(event):
-        slider_value = slider1.get()
-        slider_value += event.delta/120 
-        size.set(slider_value)
-    
-    slider1.bind("<MouseWheel>", update_slider)
-    
-    tk.Label(window, text="").pack()
-    
-    label2 = tk.Label(window, text="Images intensity", anchor="w")
-    label2.pack()
-    
-    slider_values = {}
-
-    for bt in range(len(image_list)):
-        slider_values[str('b' + str(bt))] = tk.DoubleVar()
-        tk.Label(window, text="").pack()
-        tk.Label(window, text=str("Img_" + str(bt)), anchor="w").pack()
-        tk.Scale(window, from_=0, to=20, orient=tk.HORIZONTAL, length=400, variable=slider_values[str('b' + str(bt))]).pack()
-        slider_values[str('b' + str(bt))].set(10)
-
-    
-
-
-    tk.Label(window, text="").pack()
-    
-    def merge2():
         intensity_factors = []
         for bt in range(len(image_list)):
-            intensity_factors.append((slider_values[str('b' + str(bt))].get()/10))
+            intensity_factors.append(1)
+            
+        def merge1():
+            global result
+            result = None
+            
+            for i, image in enumerate(image_list):
+                if result is None:
+                    result = image.astype(float) * intensity_factors[i]
+                else:
+                    result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
             
-        global result
-        result = None
+            result = result.astype('uint16')
+            
+    
         
-        for i, image in enumerate(image_list):
-            if result is None:
-                result = image.astype(float) * intensity_factors[i]
-            else:
-                result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
+        window = tk.Tk()
         
-        result = result.astype('uint16')
-    
-    button = tk.Button(window, text="Apply", command=merge2)
-    
-    button.pack()
-    
-    merge1()
-    
+        window.geometry("500x600")
+        window.title("MERGE CHANELS")
     
-    def display_image():
-
-        tmp = result
-        height, width = tmp.shape[:2]
-        resized_image = cv2.resize(tmp, (int(width/(50-size.get()*0.5)), int(height/(50-size.get()*0.5))))
-        cv2.imshow('Image',resized_image)
-        
-        window.after(100, display_image)
+        window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
        
     
-    display_image()
-    
-    
-    def close_window():
-        window.destroy()
-    
-    tk.Label(window, text="").pack()
-    
-    button2 = tk.Button(window, text="Save", command=close_window)
+       
+        tk.Label(window, text="").pack()
+        tk.Label(window, text="").pack()
+        
+        
+        label1 = tk.Label(window, text="Size", anchor="w")
+        label1.pack()
+        
+        # Create a slider widget
+        
+        size = tk.DoubleVar()
+        slider1 = tk.Scale(window, from_=0, to=100, orient=tk.HORIZONTAL, length=400, variable=size)
+        slider1.set(50)
+        slider1.pack()
+        
+        def update_slider(event):
+            slider_value = slider1.get()
+            slider_value += event.delta/120 
+            size.set(slider_value)
+        
+        slider1.bind("<MouseWheel>", update_slider)
+        
+        tk.Label(window, text="").pack()
+        
+        label2 = tk.Label(window, text="Images intensity", anchor="w")
+        label2.pack()
+        
+        slider_values = {}
     
-    button2.pack()
+        for bt in range(len(image_list)):
+            slider_values[str('b' + str(bt))] = tk.DoubleVar()
+            tk.Label(window, text="").pack()
+            tk.Label(window, text=str("Img_" + str(bt)), anchor="w").pack()
+            tk.Scale(window, from_=0, to=20, orient=tk.HORIZONTAL, length=400, variable=slider_values[str('b' + str(bt))]).pack()
+            slider_values[str('b' + str(bt))].set(10)
     
+        
     
     
+        tk.Label(window, text="").pack()
+        
+        def merge2():
+            intensity_factors = []
+            for bt in range(len(image_list)):
+                intensity_factors.append((slider_values[str('b' + str(bt))].get()/10))
+                
+            global result
+            result = None
+            
+            for i, image in enumerate(image_list):
+                if result is None:
+                    result = image.astype(float) * intensity_factors[i]
+                else:
+                    result = cv2.addWeighted(result, 1, image.astype(float) * intensity_factors[i], 1, 0)
+            
+            result = result.astype('uint16')
+        
+        button = tk.Button(window, text="Apply", command=merge2)
+        
+        button.pack()
+        
+        merge1()
+        
+        
+        def display_image():
     
-    window.mainloop()
-
-    cv2.destroyAllWindows()
+            tmp = result
+            height, width = tmp.shape[:2]
+            resized_image = cv2.resize(tmp, (int(width/(50-size.get()*0.5)), int(height/(50-size.get()*0.5))))
+            cv2.imshow('Image',resized_image)
+            
+            window.after(100, display_image)
+           
+        
+        display_image()
+        
+        
+        def close_window():
+            window.destroy()
+        
+        tk.Label(window, text="").pack()
+        
+        button2 = tk.Button(window, text="Save", command=close_window)
+        
+        button2.pack()
+        
+        
+        
+        
+        window.mainloop()
     
-  
+        cv2.destroyAllWindows()
+        
+      
+        
+        return result
     
-    return result
+    except:
+        print("Something went wrong. Check the function input data and try again!")
 
 
 
 
 
 def image_grid(path_to_opera_projection:str, img_length:int, img_width:int):
 
@@ -950,16 +1022,15 @@
         resize_table['height'] =  resize_table['height'] + (resize_table['height'] * resize_table['factor'])/resize_factor
         resize_table['width'] = resize_table['width'] + (resize_table['width'] * resize_table['factor'])/resize_factor
         resize_table['resize_factor'] =  resize_table['resize_factor'] + (resize_table['resize_factor'] * resize_table['factor'])/resize_factor
     
         
         image2 = resize(image, img_length, img_width, resize_factor)
         
-        import tkinter as tk 
-        from tkinter import ttk, Text
+        
         
         window = tk.Tk()
         
         window.geometry("500x600")
         window.title("IMAGE SELECTION")
 
         window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
@@ -1029,39 +1100,282 @@
             window.destroy()
         
         tk.Label(window, text="").pack()
         
         button2 = tk.Button(window, text="Apply", command=close_window)
         
         button2.pack()
-        
-        
-        
+
         
         window.mainloop()
 
         cv2.destroyAllWindows()
    
 
         return image_list
     
     
 
 def select_pictures(image_dictinary:pd.DataFrame, path_to_images:str, path_to_save:str, numbers_of_pictures:list):
     
-    selected = image_dictinary[image_dictinary['image_num'].isin(numbers_of_pictures)]
-    selected = selected.reset_index()
+    try:
     
-    if not os.path.exists(path_to_save):
-        os.mkdir(path_to_save)
+        selected = image_dictinary[image_dictinary['image_num'].isin(numbers_of_pictures)]
+        selected = selected.reset_index()
+        
+        if not os.path.exists(path_to_save):
+            os.mkdir(path_to_save)
+        
+        for n, num in enumerate(selected['image_num']):
+            
+            images_list=os.listdir(path_to_images)
+        
+            images_list=[x for x in images_list if str(re.sub('\n','', (str(selected['queue'][selected['image_num'] == num][n]))) + 'p') in x]
+            
+            if not os.path.exists(os.path.join(path_to_save,'img_' + str(num))):
+                os.mkdir(os.path.join(path_to_save,'img_' + str(num)))
+                
+            for image in images_list:
+                shutil.copy(os.path.join(path_to_images,image),os.path.join(path_to_save,'img_' + str(num)))
+                
+    except:
+        print("Something went wrong. Check the function input data and try again!")
+            
+            
+            
+            
+     
+def add_scalebar(image, metadata):
+
+    try:
+        global image2
+        global met
+        
+        met = metadata.copy()
+
+        image2 = image.copy()
+        
+       
+        window = tk.Tk()
+        
+        window.geometry("500x800")
+        window.title("SCALE-BAR")
     
-    for n, num in enumerate(selected['image_num']):
+        window.iconbitmap(pkg_resources.resource_filename("operetta", "jbsicon.ico"))
+       
         
-        images_list=os.listdir(path_to_images)
+        txt1 = tk.Label(window, text="Scale parameters", anchor="w", justify="left")
+        txt1.pack()
+       
+        tk.Label(window, text="").pack()
+        tk.Label(window, text="").pack()
+        
+        
+        label1 = tk.Label(window, text="Size", anchor="w")
+        label1.pack()
+        
+        # Create a slider widget
+        
+        size = tk.DoubleVar()
+        slider1 = tk.Scale(window, from_=0, to=100, orient=tk.HORIZONTAL, length=400, variable=size)
+        slider1.set(50)
+        slider1.pack()
+        
+        def update_slider(event):
+            slider_value = slider1.get()
+            slider_value += event.delta/120 
+            size.set(slider_value)
+        
+        slider1.bind("<MouseWheel>", update_slider)
+        
+        tk.Label(window, text="").pack()
+        
+        label2 = tk.Label(window, text="Scale length [um]", anchor="w")
+        label2.pack()
+        
+        length = tk.DoubleVar()
+        l = [50, 100, 250, 500, 1000, 1500, 2000, 2500, 3000, 4000, 5000]
+    
+        length = ttk.Combobox(window, values=l)
+        length.current(3)
+        length.pack()
+       
+        
+        tk.Label(window, text="").pack()
+        
+        label3 = tk.Label(window, text="Scalebar thickness[px]", anchor="w")
+        label3.pack()
+        
+        
+        thickness = tk.DoubleVar()
+        items = [10, 15, 25, 30, 35, 50, 75, 100, 125, 150, 200]
+    
+        thickness = ttk.Combobox(window, values=items)
+        thickness.current(2)
+        thickness.pack()
+
+        
+
+        tk.Label(window, text="").pack()
+        label4 = tk.Label(window, text="Color", anchor="w")
+        label4.pack()
+        
+        items = ['white', 'grey', "blue", "green", "red", "magenta", 'yellow', 'cyan', 'black']
     
-        images_list=[x for x in images_list if str(re.sub('\n','', (str(selected['queue'][selected['image_num'] == num][n]))) + 'p') in x]
+        combobox = ttk.Combobox(window, values=items)
         
-        if not os.path.exists(os.path.join(path_to_save,'img_' + str(num))):
-            os.mkdir(os.path.join(path_to_save,'img_' + str(num)))
+        combobox.current(0)
+        
+        combobox.pack()
+        
+        
+        tk.Label(window, text="").pack()
+        label5 = tk.Label(window, text="Font size", anchor="w")
+        label5.pack()
+        
+        fonts = [0.5,1,1.5,2,2.5,3,3.5,4,4.5,5]
+    
+        font = ttk.Combobox(window, values=fonts)
+        
+        font.current(2)
+        
+        font.pack()
+        
+        
+        tk.Label(window, text="").pack()
+        
+        label6 = tk.Label(window, text="Position", anchor="w")
+        label6.pack()
+        
+        position_bar = ["right_bottom", "right_top", "left_top", "left_bottom"]
+    
+        position_type = ttk.Combobox(window, values=position_bar)
+        
+        position_type.current(0)
+        
+        position_type.pack()
+        
+       
+        button_finished = tk.BooleanVar(value=False)
+        
+        def active_changes():
             
-        for image in images_list:
-            shutil.copy(os.path.join(path_to_images,image),os.path.join(path_to_save,'img_' + str(num)))
+
+                scale_color = (65535, 65535, 65535)
+               
+                global image3
+                
+                image3 = image2.copy()
+                
+                # Determine the desired size of the scale bar and convert it to pixels
+                scale_length_um = int(length.get())  # Length of the scale bar in millimeters
+                pixels_per_um = met['X_resolution[m]'][0]*1000000   # Number of pixels equivalent to 1 millimeter
+                scale_length_px = int(scale_length_um * pixels_per_um)
+ 
+                # Calculate the position of the scale bar
+                image_height, image_width, _ = image3.shape
+                
+                scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.96))  # Adjust the position as needed
+
+ 
+                # Draw the scale bar on the image
+                if str(combobox.get()) == 'grey':
+                    scale_color = (32768, 32768, 32768)
+                elif str(combobox.get()) == 'red':
+                    scale_color = (0, 0, 65535)
+                elif str(combobox.get()) == 'green':
+                    scale_color = (0, 65535, 0)
+                elif str(combobox.get()) == 'blue':
+                    scale_color = (65535, 0, 0)
+                elif str(combobox.get()) == 'magenta':
+                    scale_color = (65535, 0, 65535)
+                elif str(combobox.get()) == 'yellow':
+                    scale_color = (0, 65535, 65535)
+                elif str(combobox.get()) == 'cyan':
+                    scale_color = (65535, 65535, 0)
+                elif str(combobox.get()) == 'black':
+                    scale_color = (0, 0, 0)
+                elif str(combobox.get()) == 'white':
+                    scale_color = (65535, 65535, 65535)
+                    
+                
+                scale_thickness = int(thickness.get())  
+                
+                if str(position_type.get()) == 'left_top':
+                    scale_position = (int(image_width*0.04) + scale_length_px, int(image_height*0.04)) 
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
+                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
+     
+
+                elif str(position_type.get()) == 'left_bottom':
+                    scale_position = (int(image_width*0.04) + scale_length_px, int(image_height*0.96))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
+                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
+     
+
+                elif str(position_type.get()) == 'right_top':
+                    scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.04))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
+                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
+     
+                elif str(position_type.get()) == 'right_bottom':
+                    scale_position = (int(image_width*0.96) - scale_length_px, int(image_height*0.96))  
+                    cv2.rectangle(image3, scale_position, (scale_position[0] + scale_length_px, scale_position[1] - 10), scale_color, scale_thickness)
+                    cv2.putText(image3, f'{scale_length_um} um', (scale_position[0], scale_position[1] - 50), cv2.FONT_HERSHEY_SIMPLEX, float(font.get()), scale_color, 3)
+     
+
+            
+
+                
+                button_finished.set(True)
+           
+    
+        
+        tk.Label(window, text="").pack()
+        button = tk.Button(window, text="Apply", command=active_changes)
+        
+        
+        
+        
+        button.pack()
+        
+        
+        
+        def display_image():
+            
+            if button_finished.get():
+                tmp = image3
+                height, width = tmp.shape[:2]
+                resized_image = cv2.resize(tmp, (int(width/(50-size.get()*0.5)), int(height/(50-size.get()*0.5))))
+                cv2.imshow('Image',resized_image)
+                
+            window.after(100, display_image)
+           
+        
+        display_image()
+        
+        
+       
+        
+        def close_window():
+            window.destroy()
+            
+        tk.Label(window, text="").pack()
+        
+        button2 = tk.Button(window, text="Save", command=close_window)
+        
+        button2.pack()
+        
+        
+        
+        active_changes()
+        window.mainloop()
+    
+        cv2.destroyAllWindows()
+    
+        
+        return image3
+
+    except:
+        print("Something went wrong. Check the function input data and try again!")
+        
+
```

### Comparing `Operetta_tool-1.2.7/setup.py` & `Operetta_tool-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.7' 
+VERSION = '1.3.0' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

