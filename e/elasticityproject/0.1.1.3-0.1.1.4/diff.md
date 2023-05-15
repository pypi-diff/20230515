# Comparing `tmp/elasticityproject-0.1.1.3.tar.gz` & `tmp/elasticityproject-0.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticityproject-0.1.1.3.tar", max compression
+gzip compressed data, was "elasticityproject-0.1.1.4.tar", max compression
```

## Comparing `elasticityproject-0.1.1.3.tar` & `elasticityproject-0.1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0    35100 2023-05-13 19:37:36.869380 elasticityproject-0.1.1.3/LICENSE
--rw-r--r--   0        0        0      793 2023-05-13 19:37:37.816241 elasticityproject-0.1.1.3/README.md
--rw-r--r--   0        0        0      637 2023-05-13 21:01:28.766573 elasticityproject-0.1.1.3/pyproject.toml
--rw-r--r--   0        0        0      119 2023-05-13 19:37:42.637839 elasticityproject-0.1.1.3/src/elasticityproject/__init__.py
--rw-r--r--   0        0        0    21274 2023-05-13 19:57:02.043623 elasticityproject-0.1.1.3/src/elasticityproject/elasticityproject.py
--rw-r--r--   0        0        0     2891 2023-05-13 19:57:56.680020 elasticityproject-0.1.1.3/src/elasticityproject/plots3d.py
--rw-r--r--   0        0        0     1637 2023-05-13 21:01:33.478831 elasticityproject-0.1.1.3/setup.py
--rw-r--r--   0        0        0     1437 2023-05-13 21:01:33.479140 elasticityproject-0.1.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0    35100 2023-05-15 20:34:20.067297 elasticityproject-0.1.1.4/LICENSE
+-rw-r--r--   0        0        0      793 2023-05-15 20:34:20.074443 elasticityproject-0.1.1.4/README.md
+-rw-r--r--   0        0        0      637 2023-05-15 20:40:14.465538 elasticityproject-0.1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-15 20:34:20.190837 elasticityproject-0.1.1.4/src/elasticityproject/__init__.py
+-rw-r--r--   0        0        0    17539 2023-05-15 20:34:20.204254 elasticityproject-0.1.1.4/src/elasticityproject/elasticityproject.py
+-rw-r--r--   0        0        0     2891 2023-05-15 20:34:20.214104 elasticityproject-0.1.1.4/src/elasticityproject/plots3d.py
+-rw-r--r--   0        0        0     1637 2023-05-15 20:41:17.802822 elasticityproject-0.1.1.4/setup.py
+-rw-r--r--   0        0        0     1437 2023-05-15 20:41:17.803193 elasticityproject-0.1.1.4/PKG-INFO
```

### Comparing `elasticityproject-0.1.1.3/LICENSE` & `elasticityproject-0.1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticityproject-0.1.1.3/README.md` & `elasticityproject-0.1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `elasticityproject-0.1.1.3/pyproject.toml` & `elasticityproject-0.1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elasticityproject"
-version = "0.1.1.3"
+version = "0.1.1.4"
 description = "A collection of classes and routines to help the treatment and presentation of single and polycrystal elastic properties"
 authors = ["EELElasticityGroup"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `elasticityproject-0.1.1.3/src/elasticityproject/elasticityproject.py` & `elasticityproject-0.1.1.4/src/elasticityproject/elasticityproject.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,21 +15,18 @@
             independent elastic constants, the quantity of constants depends on the crystal class, as indicated between parenthesis above, GPa is the refered unit
 
         Returns
         ----------
         C: array
             (6x6) numpy array, stiffness matrix based on the given constants and material crystal class
         S: array
-            (6x6) numpy array | compliance matrix based on the given constants and material crystal class
-        St:
-            (3x3x3x3) numpy array | compliance tensor based on the given constants and material crystal class
+            (6x6) numpy array, compliance matrix based on the given constants and material crystal class
+        St: array
+            (3x3x3x3) numpy array, compliance tensor based on the given constants and material crystal class
 
-        Example:
-        ----------
-        CsNiF3 =  ElasticityTheory('tetragonal_1', 29.10, -13.10, -1.81, 11.00, 213.00, 84.00)
 
 
     '''
 
     def __init__(self, crystal_class, *stiff_consts):
 
         self.crystal_classes = {'isotropic': 2, 'cubic': 3, 'hexagonal': 5,
@@ -48,16 +45,14 @@
         self.S = self.ComplianceMatrix(self.C)
         self.St = self.ComplianceTensor(self.S)
 
     def StiffnessMatrix(self, crystal_class, *stiff_consts):
         '''
         Generates the stiffness matrix based on the given crystal class and independent elastic constants based on voigt notation
 
-        Generates the compliance matrix, compliance tensor and stiffness matrix based on the given inputs. Each crystal class have a specific number of constants to be given
-
         Parameters
         ----------
         crystal_class: str
             one of the following crystal classes: isotropic (2), cubic (3), hexagonal (5), trigonal_1 (6), trigonal_2 (7), tetragonal_1 (6), tetragonal_2 (7), orthorhombic (9), monoclinic_1 (13), monoclinic_2 (13), triclinic (21)
         stiffness constants: int
             independent elastic constants, the quantity of constants depends on the crystal class, as indicated between parenthesis above, GPa is the refered unit
 
@@ -212,15 +207,15 @@
             one of the following crystal classes: isotropic (2), cubic (3), hexagonal (5), trigonal_1 (6), trigonal_2 (7), tetragonal_1 (6), tetragonal_2 (7), orthorhombic (9), monoclinic_1 (13), monoclinic_2 (13), triclinic (21)
         stiffness constants: int
             independent elastic constants, the quantity of constants depends on the crystal class, as indicated between parenthesis above, GPa is the refered unit
 
         Returns
         ----------
         S: array
-            (6x6) numpy array | compliance matrix based on the given constants and material crystal class
+            (6x6) numpy array, compliance matrix based on the given constants and material crystal class
         '''
 
         return la.inv(C)
 
     def ComplianceTensor(self, S):
         '''
         Generates the compliance tensor based on the given crystal class and independent elastic constants based on voigt notation
@@ -232,15 +227,15 @@
         stiffness constants: int
             independent elastic constants, the quantity of constants depends on the crystal class, as indicated between parenthesis above, GPa is the refered unit
 
 
         Returns
         ----------
         St: array
-            (3x3x3x3) numpy array | compliance tensor based on the given constants and material crystal class
+            (3x3x3x3) numpy array, compliance tensor based on the given constants and material crystal class
         '''
 
 
         St = np.zeros((3, 3, 3, 3), dtype=float)
 
         rel = {'00': 0, '11': 1, '22': 2,
                '12': 3, '21': 3, '02': 4, '20': 4,
@@ -263,176 +258,124 @@
 
         return St
 
 
 class DirectionalProperties(ElasticityTheory):
 
     '''
-    Generates the object that calculate directional properties based on the given input properties
+        Generates the object that calculate directional properties based on the given input properties
+
         Parameters
         ----------
         crystal_class: str
             one of the following crystal classes: isotropic (2), cubic (3), hexagonal (5), trigonal_1 (6), trigonal_2 (7), tetragonal_1 (6), tetragonal_2 (7), orthorhombic (9), monoclinic_1 (13), monoclinic_2 (13), triclinic (21)
         stiffness constants: int
             independent elastic constants, the quantity of constants depends on the crystal class, as indicated between parenthesis above, GPa is the refered unit
 
 
         Returns
         ----------
-        B | (NxN) np array | Linear compressibility for each direction l
-        E | (NxN) np array | Young Modulus for each direction l
-        G | (NxNxN) np array | Shear Modulus for l and n directions
-        p | (NxNxN) np array | Poisson's Ration for l and n directions
+        B:  array
+            (NxN) np array, Linear compressibility for each direction l
+        E: array
+            (NxN) np array, Young Modulus for each direction l
+        G: array
+            (NxNxN) np array | Shear Modulus for l and n directions
+        p: array
+            (NxNxN) np array | Poisson's Ration for l and n directions
         *N is the number of points specified in the l direction
 
-        Example:
-        ----------
-        #For l dependant functions
-        DirProp = DirectionalProperties('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
-        theta, phi = np.mgrid[0:np.pi:100, 0:2*np.pi:100]
-        ldir = np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
-        DirProp.LinearCompressibility(ldir)
-        #For l,n dependant functions
-        n_dir_theta, n_dir_phi, n_dir_psi = np.mgrid[0:np.pi:int(100) * 1j, 0:2*np.pi:int(100) * 1j, 0:2*np.pi:int(100) * 1j]
-        ndir  = np.array([
-                    np.sin(n_dir_phi) * np.sin(0)- np.cos(n_dir_theta)*np.cos(n_dir_phi)*np.cos(0),
-                    -np.cos(n_dir_phi)*np.sin(0) - np.cos(n_dir_phi)*np.sin(n_dir_phi)*np.cos(0),
-                    np.sin(n_dir_phi)*np.cos(0)
-                ])
-        DirProp.ShearModulus(ldir,ndir)
     '''
 
     def LinearCompressibility(self, l):
         '''
             Generates the material linear compressibility matrix based on the l direction input
+
             Parameters
             ----------
             l: array
                 Stress direction (NxN) array
 
             Returns
             ----------
             B: array
-                (NxN) np array | Linear compressibility for each direction l
-
-            Example:
-            ----------
-            DirProp = DirectionalProperties('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
-            #N=100
-            theta, phi = np.mgrid[0:np.pi:100, 0:2*np.pi:100]
-            ldir = np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
-            DirProp.LinearCompressibility(ldir)
+                (NxN) np array, Linear compressibility for each direction l
         '''
 
         B = 0.
         for i in range(3):
             for j in range(3):
                 for k in range(3):
                     B += self.St[i, j, k, k] * l[i] * l[j]
         return 1.0 / B
 
     def YoungModulus(self, l):
         '''
             Generates the material young modulus matrix based on the l direction input
+
             Parameters
             ----------
             l: array
                 Stress direction (NxN) array
 
             Returns
             ----------
             E: array
-                (NxN) np array | Linear compressibility for each direction l
-
-            Example:
-            ----------
-            DirProp = DirectionalProperties('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
-            #N=100
-            theta, phi = np.mgrid[0:np.pi:100, 0:2*np.pi:100]
-            ldir = np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
-            DirProp.LinearCompressibility(ldir)
+                (NxN) np array, Linear compressibility for each direction l
         '''
         E = 0.
         for i in range(3):
             for j in range(3):
                 for k in range(3):
                     for m in range(3):
                         E += self.St[i, j, k, m] * l[i] * l[j] * l[k] * l[m]
         return 1.0 / E
 
     def ShearModulus(self, l, n):
         '''
             Generates the material shear modulus matrix based on the l direction input
+
             Parameters
             ----------
             l: array
                 Stress direction (NxN) array
             n: array
                 Normal direction (NxNxN) array
 
             Returns
             ----------
             G: array
-                (NxNxN) np array | Linear compressibility for each direction l and normal direction n
+                (NxNxN) np array, Linear compressibility for each direction l and normal direction n
 
-
-            Example:
-            ----------
-            DirProp = DirectionalProperties('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
-            theta, phi = np.mgrid[0:np.pi:int(100)*1j, 0:2*np.pi:int(100)*1j]
-            ldir = np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
-            n_dir_theta, n_dir_phi, n_dir_psi = np.mgrid[0:np.pi:int(100) * 1j, 0:2*np.pi:int(100) * 1j, 0:2*np.pi:int(100)* 1j]
-            *N is the number of points specified in the l direction
-            *The psi angle in ndir must be fixated to generate a plottable image
-            ndir  = np.array([
-                    np.sin(n_dir_phi) * np.sin(0)- np.cos(n_dir_theta)*np.cos(n_dir_phi)*np.cos(0),
-                    -np.cos(n_dir_phi)*np.sin(0) - np.cos(n_dir_phi)*np.sin(n_dir_phi)*np.cos(0),
-                    np.sin(n_dir_phi)*np.cos(0)
-                ])
-            DirProp.ShearModulus(ldir,ndir)
         '''
 
         G = 0.
         for i in range(3):
             for j in range(3):
                 for k in range(3):
                     for m in range(3):
                         G += self.St[i, j, k, m] * l[i] * n[j] * l[k] * n[m]
         return .25 / G
 
     def PoissonRatio(self, l, n):
         '''
             Generates the material Poisson Ratio matrix based on the l direction input
+
             Parameters
             ----------
             l: array
                 Stress direction (NxN) array
             n: array
                 Normal direction (NxNxN) array
 
             Returns
             ----------
             PoissonRatio: array
-                (NxNxN) np array | Linear compressibility for each direction l and normal direction n
+                (NxNxN) np array, Linear compressibility for each direction l and normal direction n
 
-
-            Example:
-            ----------
-            DirProp = DirectionalProperties('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
-            theta, phi = np.mgrid[0:np.pi:int(100)*1j, 0:2*np.pi:int(100)*1j]
-            ldir = np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
-            n_dir_theta, n_dir_phi, n_dir_psi = np.mgrid[0:np.pi:int(100) * 1j, 0:2*np.pi:int(100) * 1j, 0:2*np.pi:int(100)* 1j]
-            *N is the number of points specified in the l direction
-            *The psi angle in ndir must be fixated to generate a plottable image
-            ndir  = np.array([
-                    np.sin(n_dir_phi) * np.sin(0)- np.cos(n_dir_theta)*np.cos(n_dir_phi)*np.cos(0),
-                    -np.cos(n_dir_phi)*np.sin(0) - np.cos(n_dir_phi)*np.sin(n_dir_phi)*np.cos(0),
-                    np.sin(n_dir_phi)*np.cos(0)
-                ])
-            DirProp.PoissonRatio(ldir,ndir)
         '''
 
         p = 0.
         for i in range(3):
             for j in range(3):
                 for k in range(3):
                     for m in range(3):
@@ -470,17 +413,14 @@
         BulkModulus: int
             VRH approximation of Bulk Modulus using data from the three approximations
         YoungModulus: int
             VRH approximation of Young Modulus using data from the three approximations
         PoissonRatio: int
             VRH approximation of Poisson Ratio using data from the three approximations
 
-        Example:
-        ----------
-        VRHProp = VRH('hexagonal', 246.73, 126.66, 104.6,241.26, 58.48 )
     '''
 
     def Reuss(self):
 
         sii = self.S[0, 0] + self.S[1, 1] + self.S[2, 2]
         sij = self.S[0, 1] + self.S[0, 2] + self.S[1, 2]
         skl = self.S[3, 3] + self.S[4, 4] + self.S[5, 5]
@@ -510,14 +450,18 @@
         B, G = self.BH, self.GH
         self.BulkModulus, self.ShearModulus = B, G
         self.YoungModulus = 9. * B * G / (3. * B + G)
         self.PoissonRatio = (3. * B - 2. * G) / 2. / (3. * B + G)
 
 
 class DebyeGruneisen(VRH):
-
+    '''
+    Class under development
+    '''
     pass
 
 
 class Elasticity(DirectionalProperties, VRH):
-
+    '''
+    Class under development
+    '''
     pass
```

### Comparing `elasticityproject-0.1.1.3/src/elasticityproject/plots3d.py` & `elasticityproject-0.1.1.4/src/elasticityproject/plots3d.py`

 * *Files identical despite different names*

### Comparing `elasticityproject-0.1.1.3/setup.py` & `elasticityproject-0.1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mayavi>=4.8.1,<5.0.0', 'numpy>=1.24.3,<2.0.0', 'vtk>=9.2.6,<10.0.0']
 
 setup_kwargs = {
     'name': 'elasticityproject',
-    'version': '0.1.1.3',
+    'version': '0.1.1.4',
     'description': 'A collection of classes and routines to help the treatment and presentation of single and polycrystal elastic properties',
     'long_description': '# elasticityproject\n\nA collection of classes and routines to help the treatment and presentation of single and polycrystal elastic properties\n\n## Installation\n\n```bash\n$ pip install elasticityproject\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`elasticityproject` was created by EELElasticityGroup. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`elasticityproject` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'EELElasticityGroup',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `elasticityproject-0.1.1.3/PKG-INFO` & `elasticityproject-0.1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticityproject
-Version: 0.1.1.3
+Version: 0.1.1.4
 Summary: A collection of classes and routines to help the treatment and presentation of single and polycrystal elastic properties
 License: GNU General Public License v3.0
 Author: EELElasticityGroup
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

