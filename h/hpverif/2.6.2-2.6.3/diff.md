# Comparing `tmp/hpverif-2.6.2-py3-none-any.whl.zip` & `tmp/hpverif-2.6.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12578 bytes, number of entries: 15
+Zip file size: 13754 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3046 b- defN 23-May-08 14:15 hpverif/Calibraton.py
 -rw-r--r--  2.0 unx      449 b- defN 23-May-08 15:40 hpverif/Driver.py
 -rw-r--r--  2.0 unx     3961 b- defN 23-May-08 14:15 hpverif/FrameCapture.py
 -rw-r--r--  2.0 unx     2576 b- defN 23-May-08 14:15 hpverif/FrameCapturePLY.py
 -rw-r--r--  2.0 unx     3967 b- defN 23-May-08 14:15 hpverif/PointCloud.py
 -rw-r--r--  2.0 unx     5584 b- defN 23-May-15 15:28 hpverif/Segmentation.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-May-08 14:15 hpverif/ShowFiles.py
--rw-r--r--  2.0 unx     4934 b- defN 23-May-08 14:15 hpverif/Theoretical_distance.py
--rw-r--r--  2.0 unx     1876 b- defN 23-May-11 22:37 hpverif/Verification.py
+-rw-r--r--  2.0 unx     9966 b- defN 23-May-15 15:57 hpverif/Theoretical_distance.py
+-rw-r--r--  2.0 unx     1876 b- defN 23-May-15 15:57 hpverif/Verification.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-08 14:15 hpverif/__init__.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-08 14:15 hpverif/driver.py
--rw-r--r--  2.0 unx      321 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1159 b- defN 23-May-15 15:28 hpverif-2.6.2.dist-info/RECORD
-15 files, 30805 bytes uncompressed, 10678 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx      321 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1159 b- defN 23-May-15 16:01 hpverif-2.6.3.dist-info/RECORD
+15 files, 35837 bytes uncompressed, 11854 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: hpverif/__init__.py
 Comment: 
 
 Filename: hpverif/driver.py
 Comment: 
 
-Filename: hpverif-2.6.2.dist-info/METADATA
+Filename: hpverif-2.6.3.dist-info/METADATA
 Comment: 
 
-Filename: hpverif-2.6.2.dist-info/WHEEL
+Filename: hpverif-2.6.3.dist-info/WHEEL
 Comment: 
 
-Filename: hpverif-2.6.2.dist-info/top_level.txt
+Filename: hpverif-2.6.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hpverif-2.6.2.dist-info/RECORD
+Filename: hpverif-2.6.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpverif/Theoretical_distance.py

```diff
@@ -1,8 +1,9 @@
 import matplotlib.pyplot as plt
+import numpy as np
 import math
 import ast
 
 class Theoretical_distance:
 
     def __init__ (self):
         pass
@@ -20,29 +21,135 @@
         #Calculem distancia central
         dist, interseccio_paret = self.distancia_propera(point, angle_degrees, lines)
 
         #Camp de visió càmara
         FOV_right, interseccio_paret_right = self.distancia_propera(point, angle_degrees - angle_FOV, lines)
         FOV_left, interseccio_paret_left = self.distancia_propera(point, angle_degrees + angle_FOV, lines)
 
+        angles = array = np.arange(-angle_FOV, angle_FOV, 0.5)
+        scalar_angles = [math.radians(angle) for angle in angles]
+
+        d = []                          #Vector de distancies
+        interseccio_paret_aa = []       #Vector de les interseccions
+        distancia_max = 0               #inicialitzacio pel calcul de la distancia max
+        distancia_min_c = 1500          #inicialitzacio pel calcul de la distancia min
+        cares_columna = 0               #Indica el nombre de cares d'una columna que veu la camara
+        estam_veiem_columna = False     #boolean que indica si en quin moment s'esta observant la columna dintra de la iteracio 
+        index_columna_final = -1        #inicialitzacio per a la distancia de la columna
+        index_columna_inici = -1        #idem
+        index_min_c = 1500
+        hem_estat_columna = False
+
+        for i in range(len(scalar_angles)):
+            distancia, interseccio = self.distancia_propera(point, angle_degrees + angles[i], lines)
+            distancia = distancia*math.cos(scalar_angles[i])
+            #print(i,distancia, angles[i])
+            d.append(distancia)
+            interseccio_paret_aa.append(interseccio)
+            if distancia > distancia_max: #Guardem el valor i index de la distancia maxima i per tant, cantonada
+                index_max = i-1
+                distancia_max = distancia
+
+            if abs(distancia-d[i-1]) > 10: #Si hi ha salts de valors "grans" significa que la camara veu una columna
+                if not estam_veiem_columna: 
+                    print("entrem de la columna",i)
+                    index_columna_inici = i
+                    estam_veiem_columna = True
+                    hem_estat_columna = True
+        
+                else:
+                    print("sortim de la columna",i)
+                    index_columna_final = i-1
+                    estam_veiem_columna = False
+
+            if distancia < distancia_min_c and estam_veiem_columna: #Veiem la cantonada de la columna
+                index_min_c = i
+                distancia_min_c = distancia
+
+        #La columna es recte, per tant si el valor maxim esta al principi o al final, ja sabem que la camara no veu
+        #cap cantonada, en el cas que el maxim no coincideixi amb inici o final, sabem que hi haura una cantonada
+        #si hi ha cantonada sabem que la camara veu dues cares de la columna
+        if hem_estat_columna:
+            if abs(distancia_min_c-d[index_columna_inici]) < 0.01 or abs(distancia_min_c-d[index_columna_final]) < 0.01:
+                cares_columna = 1
+            else:
+                cares_columna = 2
+
+        plt.plot(angles,d)
+        plt.xlabel("Degrees")
+        plt.ylabel("Distancia")  
+
+        #print(distancia_max,angles_distancia_max, index_max)
+
+        
+        #La paret es recte, per tant si el valor maxim esta al principi o al final, ja sabem que no topem cap cantonada
+        #En el cas que el maxim no coincideixi amb inici o final, sabem que hi haura una cantonada
+
+        if(abs(distancia_max-d[0]) < 0.01 or abs(distancia_max-d[len(scalar_angles)-1]) < 0.01):
+            veiem_cantonada = False
+        else:
+            veiem_cantonada = True
+
+        #--------------------< CALCUL DE LES DISTANCIES FINALS >--------------------
+
+        print("cares columna", cares_columna)
+
+        if cares_columna == 0:
+            if not veiem_cantonada: 
+                print("Veiem una paret")
+
+                #Distancia mitja de la paret
+                dist = sum(d) / len(d)
+
+            else:
+                print("Veiem cantonada (dues parets)")
+                mean_1_np = np.mean(d[:index_max-1],dtype=np.float64)
+                mean_2_np = np.mean(d[index_max:],dtype=np.float64)
+
+                #Distacia mitja de les dues parets
+                dist = [mean_1_np, mean_2_np]
+
+        elif cares_columna == 1:
+
+            mean_columna = np.mean(d[index_columna_inici:index_columna_final-1],dtype=np.float64)
+            mean_paret_1 = np.mean(d[:index_columna_inici-1],dtype=np.float64)
+            mean_paret_2 = np.mean(d[index_columna_final+1:],dtype=np.float64)
+
+            #Distancia mitja de la de la columna i la dels dos trossos de paret
+            dist = [mean_columna, mean_paret_1, mean_paret_2]
+
+        elif cares_columna == 2:
+            print("Veiem columna amb dues cares")
+
+            mean_columna_a = np.mean(d[index_columna_inici:index_min_c-1],dtype=np.float64)
+            mean_columna_b = np.mean(d[index_min_c:index_columna_final-1],dtype=np.float64)
+            mean_paret_1 = np.mean(d[:index_columna_inici],dtype=np.float64)
+            mean_paret_2 = np.mean(d[index_columna_final+1:],dtype=np.float64)
+
+            #Distancia mitja de les dues cares (a i b) de la columna i la dels dos trossos de paret
+            dist = [mean_columna_a,mean_columna_b, mean_paret_1, mean_paret_2]
+
+
+
 
         #--------------------< REPRESENTACIÓ >--------------------
         if(show):
             #Creem mapa
             fig, ax = plt.subplots()
             # Setejem la nostra posició
             ax.scatter(point[0],point[1], label=f'Camera location: {(point[0], point[1])}' + ' cm.', color='blue', marker='o', s=30)
             # Graficar mapa
             for i in range(len(lines)):
                 x1, y1 = lines[i][0][0], lines[i][0][1]
                 x2, y2 = lines[i][1][0], lines[i][1][1]
                 ax.plot([x1, x2], [y1, y2], 'k-')
 
             #Mostrem distancia  
-            ax.plot([point[0],interseccio_paret[0]], [point[1],interseccio_paret[1]], 'g-', label=f'Central distance: {round(dist, 3)}' + ' cm.')
+            #ax.plot([point[0],interseccio_paret[0]], [point[1],interseccio_paret[1]], 'g-', label=f'Central distance: {round(dist, 3)}' + ' cm.')
+            ax.scatter(point[0],point[1], label=f'Distance to object: {round(dist[0])}' + ' cm.', color='green', marker='o', s=30)
 
             #Mostrem rang de visió de la càmara
             ax.plot([point[0],interseccio_paret_right[0]], [point[1],interseccio_paret_right[1]], 'r-', label=f'Field of view.')
             ax.plot([point[0],interseccio_paret_left[0]], [point[1],interseccio_paret_left[1]], 'r-')
 
             ax.legend(loc='upper left')
 
@@ -50,15 +157,15 @@
             ax.set_aspect('equal')
 
             plt.title('Distance between HP SitePrint and the objective')
             plt.xlabel('X Axis (cm)')
             plt.ylabel('Y Axis (cm)')
 
             #Establim valor de la distància teòrica
-            plt.text(interseccio_paret[0], interseccio_paret[1], f"{round(dist, 3)}" + " cm", ha='right', va='bottom')
+            #plt.text(interseccio_paret[0], interseccio_paret[1], f"{round(dist, 3)}" + " cm", ha='right', va='bottom')
             plt.text(point[0], point[1], f"{(point[0], point[1])}" + " cm  ", ha='right', va='bottom')
 
 
             plt.show()
 
         return dist
```

## Comparing `hpverif-2.6.2.dist-info/RECORD` & `hpverif-2.6.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 hpverif/Calibraton.py,sha256=3_apH-bhEFaYuS4uhOipNU8I4CG_9ubnpSvyJvvmeXA,3046
 hpverif/Driver.py,sha256=Ra-CMqpmRVMUhNoB5H3lYtz7_u5kHI8_umIvbVjOrco,449
 hpverif/FrameCapture.py,sha256=TH7-3ZDrAwIEckOjmM6oeYtGcD0cfx_4GgG78qHeWhk,3961
 hpverif/FrameCapturePLY.py,sha256=PK6Ki_7RZrIizsvZXJL4ixMeVrMG6ESU7vKrMOafbKA,2576
 hpverif/PointCloud.py,sha256=TreRhzS2rbdM2SovJZz-gXDRSpSfxRdqrqNp7fRb04Y,3967
 hpverif/Segmentation.py,sha256=eZFBV1NC5ALDI9fvfiyeRcSWdmDvcBM2KhMIJpXF9Ow,5584
 hpverif/ShowFiles.py,sha256=vofjelAT-1kIfQC6KB6B_Vu-NljtjvZeV-uidOOOslk,2443
-hpverif/Theoretical_distance.py,sha256=AZMGa1AavpwJ_Ilk20II-2Ac52dEbG33SGbDglhhbHE,4934
+hpverif/Theoretical_distance.py,sha256=3Trsaf8zK-SxfDJYXpV7qUdHWIfDUa72WmesJIugLMc,9966
 hpverif/Verification.py,sha256=H6gtRaBNU239j56JVoWV3GxVjIAO7g3WOqljHnN-Bmk,1876
 hpverif/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hpverif/driver.py,sha256=-Y_3y4xh1Gtygx3AruRyzaBszP15mLxSS0toIuZ_qO8,389
-hpverif-2.6.2.dist-info/METADATA,sha256=xirPyg4SLslSv-iTXyFQXs3Ixbv8HBhj_jkk02C9p1M,321
-hpverif-2.6.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hpverif-2.6.2.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
-hpverif-2.6.2.dist-info/RECORD,,
+hpverif-2.6.3.dist-info/METADATA,sha256=ywzPw_ucV-1P6evwgKec3OnC09Lr85M_K_DjgBSxRPc,321
+hpverif-2.6.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hpverif-2.6.3.dist-info/top_level.txt,sha256=XZSD1QWULYM6ehhNqJ8z6ssxrXEfKSsM1Gk2hv4UMcw,8
+hpverif-2.6.3.dist-info/RECORD,,
```

