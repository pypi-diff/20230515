# Comparing `tmp/QuantumIntelligence-0.0.7.tar.gz` & `tmp/QuantumIntelligence-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumIntelligence-0.0.7.tar", last modified: Fri May  5 09:43:58 2023, max compression
+gzip compressed data, was "QuantumIntelligence-0.0.8.tar", last modified: Mon May 15 01:27:36 2023, max compression
```

## Comparing `QuantumIntelligence-0.0.7.tar` & `QuantumIntelligence-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.126597 QuantumIntelligence-0.0.7/
--rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1763 2023-05-05 09:43:58.125792 QuantumIntelligence-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 09:43:58.126597 QuantumIntelligence-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     8844 2023-05-05 09:42:18.000000 QuantumIntelligence-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.102859 QuantumIntelligence-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.107309 QuantumIntelligence-0.0.7/src/QuantumIntelligence/
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.117930 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/
--rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/__init__.py
--rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
--rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
--rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.121977 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/
--rw-rw-rw-   0        0        0    48914 2023-05-04 19:29:25.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Circuit.py
--rw-rw-rw-   0        0        0     9960 2023-04-28 05:24:32.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Gate.py
--rw-rw-rw-   0        0        0    18277 2023-05-04 19:49:53.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Simulator.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.125208 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/
--rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/MPSclass.py
--rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TEBD.py
--rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TNclass.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:43:58.112203 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/
--rw-rw-rw-   0        0        0     1763 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 09:43:58.000000 QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/
+-rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     8844 2023-05-15 01:27:15.000000 QuantumIntelligence-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.173317 QuantumIntelligence-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.180697 QuantumIntelligence-0.0.8/src/QuantumIntelligence/
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.231709 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/
+-rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/__init__.py
+-rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
+-rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
+-rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.253903 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/
+-rw-rw-rw-   0        0        0    49591 2023-05-15 01:21:09.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Circuit.py
+-rw-rw-rw-   0        0        0     9960 2023-04-28 05:24:32.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Gate.py
+-rw-rw-rw-   0        0        0    18277 2023-05-04 19:49:53.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Simulator.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.259991 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/
+-rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/MPSclass.py
+-rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TEBD.py
+-rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TNclass.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.203683 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/top_level.txt
```

### Comparing `QuantumIntelligence-0.0.7/LICENSE` & `QuantumIntelligence-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/PKG-INFO` & `QuantumIntelligence-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.7
+Version: 0.0.8
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.7/README.md` & `QuantumIntelligence-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/setup.py` & `QuantumIntelligence-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="QuantumIntelligence",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.7",  # Required
+    version="0.0.8",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Developing quantum intelligence.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Circuit.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import stim
 import copy
 import pyzx as zx
 from QuantumIntelligence.QuantumSimulator import Gate
 from QuantumIntelligence.BasicFunSZZ import tensor_trick as tt
 from cirq.contrib.qasm_import import circuit_from_qasm
 from cirq.circuits.qasm_output import QasmUGate
-
+from qiskit.quantum_info import Operator
 
 
 # [1, 0] is |0>, [0, 1] is |1>
 # do not use fake functions, it will be removed soon
 # please apply gate on position as list(range(?)) as much as possible, this will make it faster
 # please control gate on position as list(range(?, n_qubit)) as much as possible, this will make it faster
 
@@ -48,15 +48,14 @@
         if qubit_position is None:
             self.qubit_position = list()
             for ii in range(self.n_qubit):
                 self.qubit_position.append((ii // self.size[1], ii % self.size[1]))
         else:
             self.qubit_position = qubit_position
 
-
     @property
     def requires_grad(self):
         flag = list()
         for gg in self.gate_list:
             flag.append(gg.requires_grad)
         return flag
 
@@ -107,15 +106,15 @@
                     new_c.append(position[oo])
                 for oo in control:
                     new_c.append(oo)
                 self.append(gate=cc[0], position=new_p.copy(), control=new_c.copy())
         else:
             raise ValueError('error in extend, check position')
 
-    def add_single_gate(self, gate:Gate, position, control=None, inverse=False):
+    def add_single_gate(self, gate: Gate, position, control=None, inverse=False):
         # gate can be sparse, but there seems to be no speedup
         # one should be careful when add inverse gates
         # the gate will be cloned and detached by default
 
         # do not change the following code, or some bugs would occur in circuit.ch
         gate = Gate.Gate(gate, independent=True)
         # gate = Gate.Gate(gate, independent=True).to(self.device).to(self.dtype)
@@ -179,15 +178,15 @@
         return len(self.gate_list)
 
     def __add__(self, circuit):
 
         if circuit.n_qubit != self.n_qubit:
             raise ValueError('error in +, n_qubit not equal')
 
-        tmp_circuit = Circuit(self.n_qubit, device=self.device, dtype=self.dtype)
+        tmp_circuit = Circuit(self.n_qubit, device=self.device, dtype=self.dtype, qubit_position=self.qubit_position)
         tmp_circuit.gate_list = self.gate_list + circuit.gate_list
         tmp_circuit.position_list = self.position_list + circuit.position_list
         tmp_circuit.control_list = self.control_list + circuit.control_list
         return tmp_circuit
 
     def __copy__(self):
         raise NameError('I do not permit copy for now. Please use deepcopy().')
@@ -197,15 +196,14 @@
         self.position_list.pop(index)
         self.control_list.pop(index)
 
     def clear(self):
         while len(self) > 0:
             self.pop(0)
 
-
     def add_noise_gate(self, strength=0.01):
         for ii in range(len(self)):
             if self.control_list[ii] is not None:
                 tmp_noise = Gate.noise_gate_single_gaussian(strength=strength, device=self.device, dtype=self.dtype)
                 self.gate_list[ii].tensor = self.gate_list[ii].tensor.mm(tmp_noise.tensor)
 
     def cal_barrier(self):
@@ -272,15 +270,15 @@
                         if nn in index_list_strict:
                             index_list_strict.remove(nn)
                     ii = ii + 1
         self.gate_list = new_gate_list
         self.position_list = new_position_list
         self.control_list = new_control_list
 
-    def map_qubits(self, qubit_map:dict):
+    def map_qubits(self, qubit_map: dict):
         for ii in range(len(self)):
             self.position_list[ii] = [qubit_map[pp] for pp in self.position_list[ii]]
             self.control_list[ii] = [qubit_map[pp] for pp in self.control_list[ii]]
         self.qubit_position = [self.qubit_position[ii] for ii in qubit_map.keys()]
 
     def using_qubits(self):
         using_qubits = list()
@@ -353,172 +351,171 @@
                 elif len(tmp_control) == 1:
                     raise ValueError('Waiting to support controlled ', tmp_label)
             elif tmp_label in supported_label:
                 if tmp_label == 'Z':
                     if len(tmp_control) == 0:
                         self.rz_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
-                        self.cz_gate(position=[tmp_position+tmp_control])
+                        self.cz_gate(position=[tmp_position + tmp_control])
                 elif tmp_label == 'X':
                     if len(tmp_control) == 0:
                         self.rx_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
                         self.rz_gate(position=tmp_position, theta=np.pi)
-                        self.ry_gate(position=tmp_position, theta=np.pi/2)
-                        self.cz_gate(position=[tmp_position+tmp_control])
+                        self.ry_gate(position=tmp_position, theta=np.pi / 2)
+                        self.cz_gate(position=[tmp_position + tmp_control])
                         self.ry_gate(position=tmp_position, theta=-np.pi / 2)
                         self.rz_gate(position=tmp_position, theta=-np.pi)
                 elif tmp_label == 'Y':
                     if len(tmp_control) == 0:
                         self.ry_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
-                        self.rz_gate(position=tmp_position, theta=-np.pi/2)
-                        self.ry_gate(position=tmp_position, theta=-np.pi/2)
-                        self.cz_gate(position=[tmp_position+tmp_control])
-                        self.ry_gate(position=tmp_position, theta=np.pi/2)
-                        self.rz_gate(position=tmp_position, theta=np.pi/2)
+                        self.rz_gate(position=tmp_position, theta=-np.pi / 2)
+                        self.ry_gate(position=tmp_position, theta=-np.pi / 2)
+                        self.cz_gate(position=[tmp_position + tmp_control])
+                        self.ry_gate(position=tmp_position, theta=np.pi / 2)
+                        self.rz_gate(position=tmp_position, theta=np.pi / 2)
                 elif tmp_label == 'H':
                     if len(tmp_control) > 1:
                         raise ValueError('Do not support controlled ', tmp_label)
                     self.rz_gate(position=tmp_position, theta=np.pi)
-                    self.ry_gate(position=tmp_position, theta=np.pi/2)
+                    self.ry_gate(position=tmp_position, theta=np.pi / 2)
                 else:
                     raise ValueError('tired')
             else:
                 raise ValueError('The unsupported label is', tmp_label)
 
     def cancel_rz_clifford_exp(self):
         rz_index = len(self) - 1
-        while rz_index >=0:
+        while rz_index >= 0:
             if self.gate_list[rz_index].label[0] == 'RZ':
                 walk_index = rz_index
                 walk_label = self.gate_list[walk_index].label
                 walk_position = self.position_list[walk_index][0]
                 self.pop(walk_index)
                 while walk_index > 0:
                     check_index = walk_index - 1
-                    if  walk_position in self.position_list[check_index]:
+                    if walk_position in self.position_list[check_index]:
                         check_label = self.gate_list[check_index].label
                         if check_label == 'CZ':
                             pass
                         elif check_label[0] == 'RZ':
                             new_theta = walk_label[1] + check_label[1]
-                            new_theta = ((new_theta/np.pi) % 2) * np.pi
+                            new_theta = ((new_theta / np.pi) % 2) * np.pi
                             walk_label = ('RZ', new_theta)
                             self.pop(check_index)
                             walk_index = walk_index - 1
                             rz_index = rz_index - 1
-                            if ((new_theta/np.pi) % 2) == 0:
+                            if ((new_theta / np.pi) % 2) == 0:
                                 walk_index = -1
-                        elif check_label[0] =='RX':
-                            if np.isclose((walk_label[1]/np.pi) % 2, 0.5):
+                        elif check_label[0] == 'RX':
+                            if np.isclose((walk_label[1] / np.pi) % 2, 0.5):
                                 self.gate_list[check_index] = Gate.ry_gate(theta=check_label[1])
-                            elif np.isclose((walk_label[1]/np.pi) % 2, 1):
+                            elif np.isclose((walk_label[1] / np.pi) % 2, 1):
                                 self.gate_list[check_index] = Gate.rx_gate(theta=-check_label[1])
-                            elif np.isclose((walk_label[1]/np.pi) % 2, 1.5):
+                            elif np.isclose((walk_label[1] / np.pi) % 2, 1.5):
                                 self.gate_list[check_index] = Gate.ry_gate(theta=-check_label[1])
                             else:
-                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1]/np.pi)
-                        elif check_label[0] =='RY':
-                            if (walk_label[1]/np.pi) % 2 == 0.5:
+                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1] / np.pi)
+                        elif check_label[0] == 'RY':
+                            if (walk_label[1] / np.pi) % 2 == 0.5:
                                 self.gate_list[check_index] = Gate.rx_gate(theta=-check_label[1])
-                            elif (walk_label[1]/np.pi) % 2 == 1:
+                            elif (walk_label[1] / np.pi) % 2 == 1:
                                 self.gate_list[check_index] = Gate.ry_gate(theta=-check_label[1])
-                            elif (walk_label[1]/np.pi) % 2 == 1.5:
+                            elif (walk_label[1] / np.pi) % 2 == 1.5:
                                 self.gate_list[check_index] = Gate.rx_gate(theta=check_label[1])
                             else:
-                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1]/np.pi)
+                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1] / np.pi)
                         else:
                             raise ValueError('tired')
                     walk_index = walk_index - 1
             rz_index = rz_index - 1
         self.to(self.device).to(self.dtype)
 
     def cancel_rxy_clifford_exp(self):
         rxy_index = len(self) - 1
-        while rxy_index >0:
+        while rxy_index > 0:
             if self.gate_list[rxy_index].label[0] in ('RX', 'RY'):
                 walk_index = rxy_index
                 walk_label = self.gate_list[walk_index].label
                 walk_position = self.position_list[walk_index][0]
-                if (walk_label[1]/np.pi) % 2 ==0:
+                if (walk_label[1] / np.pi) % 2 == 0:
                     walk_index = -1
                 while walk_index > 0:
                     check_index = walk_index - 1
-                    if  walk_position in self.position_list[check_index]:
+                    if walk_position in self.position_list[check_index]:
                         check_label = self.gate_list[check_index].label
                         if check_label == 'CZ':
                             walk_index = 1
                         elif check_label[0] == 'RZ':
                             raise ValueError('cancel rz first')
                         elif check_label[0] == walk_label[0]:
                             new_theta = walk_label[1] + check_label[1]
-                            new_theta = ((new_theta/np.pi) % 2) * np.pi
+                            new_theta = ((new_theta / np.pi) % 2) * np.pi
                             walk_label = (walk_label[0], new_theta)
                             self.pop(check_index)
                             rxy_index = rxy_index - 1
-                            if ((new_theta/np.pi) % 2) == 0:
+                            if ((new_theta / np.pi) % 2) == 0:
                                 walk_index = -1
                         elif check_label[0] in ('RX', 'RY'):
-                            if (check_label[1]/np.pi) % 2 == 0:
+                            if (check_label[1] / np.pi) % 2 == 0:
                                 self.pop(check_index)
                                 walk_index = walk_index - 1
                                 rxy_index = rxy_index - 1
-                            elif (check_label[1]/np.pi) % 2 == 1:
+                            elif (check_label[1] / np.pi) % 2 == 1:
                                 walk_label = (walk_label[0], -walk_label[1])
                             else:
-                                if (walk_label[1]/np.pi) % 2 == 1:
-                                    self.gate_list[check_index] = Gate.r_gate(theta=-check_label[1], label=check_label[0])
+                                if (walk_label[1] / np.pi) % 2 == 1:
+                                    self.gate_list[check_index] = Gate.r_gate(theta=-check_label[1],
+                                                                              label=check_label[0])
                                 else:
                                     walk_index = 1
                         else:
                             raise ValueError('tired')
                     walk_index = walk_index - 1
                 if walk_index <= 0:
                     self.pop(rxy_index)
-                if walk_index  == 0:
+                if walk_index == 0:
                     self.gate_list.insert(check_index + 1, Gate.r_gate(theta=walk_label[1], label=walk_label[0]))
                     self.position_list.insert(check_index + 1, [walk_position])
                     self.control_list.insert(check_index + 1, [])
             rxy_index = rxy_index - 1
         self.to(self.device).to(self.dtype)
-            
+
     def cancel_xyz_surface_code_abandoned(self):
         walk_index = 0
         xyz_list = ['X', 'Y', 'Z']
         rxyz_list = ['RX', 'RY', 'RZ']
         while walk_index < len(self):
             pop_flag = False
             tmp_label = self.gate_list[walk_index].label
             tmp_control = self.control_list[walk_index]
             if tmp_label in xyz_list:
                 if len(tmp_control) == 0:
                     pop_flag = True
             elif tmp_label[0] in rxyz_list:
                 if len(tmp_control) == 0:
-                    if (tmp_label[1]/np.pi) % 1 == 0:
+                    if (tmp_label[1] / np.pi) % 1 == 0:
                         pop_flag = True
 
             if pop_flag:
                 self.pop(walk_index)
             else:
                 walk_index = walk_index + 1
         self.to(self.device).to(self.dtype)
 
-
     # useful gates and circuits
 
     def labelled_gate(self, name, position, control=None, params=None):
         tmp_gate = Gate.labelled_simple_gate(name=name, params=params)
         for pp in position:
             if not isinstance(pp, list):
                 pp = [pp]
             self.add_single_gate(tmp_gate, position=pp, control=control)
 
-
     def x_gate(self, position, control=None):
         tmp_gate = Gate.x_gate()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def y_gate(self, position, control=None):
         tmp_gate = Gate.y_gate()
@@ -563,23 +560,26 @@
     def time_evolution(self, hamiltonian, time, position, control=None):
         tmp_gate = Gate.time_evolution(hamiltonian, time, device=self.device, dtype=self.dtype)
         self.add_single_gate(tmp_gate, position=position, control=control)
 
     def qft(self, position, control=None, inverse=False):
         if control is None:
             control = []
-        tmp_circuit = qft(self.n_qubit, position=position, control=control, inverse=inverse, device=self.device, dtype=self.dtype)
+        tmp_circuit = qft(self.n_qubit, position=position, control=control, inverse=inverse, device=self.device,
+                          dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def ch(self, unitary, position_phi, position_c, control=None, inverse=False):
-        tmp_circuit = ch(self.n_qubit, unitary, position_phi, position_c, control, inverse, device=self.device, dtype=self.dtype)
+        tmp_circuit = ch(self.n_qubit, unitary, position_phi, position_c, control, inverse, device=self.device,
+                         dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def qpe(self, unitary, position_phi, position_qpe, control=None, inverse=False):
-        tmp_circuit = qpe(self.n_qubit, unitary, position_phi, position_qpe, control, inverse, device=self.device, dtype=self.dtype)
+        tmp_circuit = qpe(self.n_qubit, unitary, position_phi, position_qpe, control, inverse, device=self.device,
+                          dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def add_one(self, position=None, control=None, inverse=False):
         tmp_circuit = add_one(self.n_qubit, position, control, inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def qhc(self, unitary, position_phi, position_qpe, position_f, n_f=None,
@@ -682,15 +682,15 @@
                     else:
                         raise ValueError('Please report this bug to deveploper. Error occurs in supported_label_r.')
             elif old_label[0] in supported_label_u:
                 theta = (old_label[1][0], old_label[1][1], old_label[1][2])
                 if self.gate_list[ii].inverse:
                     theta = (-theta[0], - theta[2], - theta[1])
                 if len(c_position) > 1:
-                    raise ValueError('Do not support control.', supported_label_u)
+                    raise ValueError('Do not support multi control.', supported_label_u)
                 if len(c_position) == 0:
                     if old_label[0] in ('U3', 'U4'):
                         qiskit_circuit.u(theta[0], theta[1], theta[2], qubit=q_position)
                 elif len(c_position) == 1:
                     if old_label[0] in ('U3', 'U4'):
                         if old_label[0] == 'U4':
                             theta3 = old_label[1][3]
@@ -701,23 +701,31 @@
                         qiskit_circuit.cu(*theta, gamma=theta3, control_qubit=c_position, target_qubit=q_position)
                     else:
                         raise ValueError('tired')
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
         return qiskit_circuit
 
-
     def to_qasm(self):
         # this is achieved by qiskit
         qiskit_circuit = self.to_qiskit()
         qasm_circuit = qiskit_circuit.qasm()
         return qasm_circuit
 
-    def from_qasm(self, qasm_circuit, replace=False):
-        qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(qasm_circuit)
+    def to_tensor(self):
+        qiskit_circuit = self.to_qiskit()
+        out_tensor = Operator(qiskit_circuit.reverse_bits()).data
+        out_tensor = tc.from_numpy(out_tensor).to(self.device).to(self.dtype)
+        return out_tensor
+
+    def from_qasm(self, qasm_circuit, replace=False, from_file=False):
+        if from_file:
+            qiskit_circuit = qiskit.QuantumCircuit.from_qasm_file(qasm_circuit)
+        else:
+            qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(qasm_circuit)
         circuit = self.from_qiskit(qiskit_circuit=qiskit_circuit, replace=replace)
         if not replace:
             return circuit
 
     def from_qiskit(self, qiskit_circuit, replace=False):
         if replace:
             circuit = self
@@ -772,34 +780,33 @@
             return circuit
 
     def positive_theta(self):
         for ii in range(len(self)):
             old_label = self.gate_list[ii].label
             if old_label[0] in ('RX', 'RY', 'RZ'):
                 while self.gate_list[ii].label[1] <= 0:
-                    self.gate_list[ii].label = (old_label[0], self.gate_list[ii].label[1] + 4*np.pi)
-
+                    self.gate_list[ii].label = (old_label[0], self.gate_list[ii].label[1] + 4 * np.pi)
 
     def zx_optimize(self, replace=False):
         self.positive_theta()
         qiskit_circuit = self.to_qiskit()
         zx_circuit = zx.Circuit.from_qasm(self.to_qasm())
         # print(zx_circuit)
         new_zx_circuit = zx.optimize.basic_optimization(zx_circuit.split_phase_gates(), do_swaps=False)
         # new_zx_circuit = zx_circuit
         new_qasm_circuit = new_zx_circuit.to_qasm()
         new_qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(new_qasm_circuit)
-        new_qiskit_circuit = qiskit.transpile(new_qiskit_circuit,basis_gates=['cz', 'rx', 'rz'],optimization_level=3)
+        new_qiskit_circuit = qiskit.transpile(new_qiskit_circuit, basis_gates=['cz', 'rx', 'rz'], optimization_level=3)
         circuit = self.from_qiskit(new_qiskit_circuit, replace=True)
         # circuit = self.from_qasm(new_qasm_circuit, replace=replace)
         if not replace:
             return circuit
 
     def qiskit_transpile(self, replace=True, **kwargs):
-        qiskit_circuit = qiskit.transpile(self.to_qiskit(),**kwargs)
+        qiskit_circuit = qiskit.transpile(self.to_qiskit(), **kwargs)
         circuit = self.from_qiskit(qiskit_circuit=qiskit_circuit, replace=replace)
         if not replace:
             return circuit
 
     def to_stim(self):
         stim_circuit = stim.Circuit()
         same_label_control0_list = ['CX', 'CY', 'CZ', 'H']
@@ -836,38 +843,37 @@
                     raise ValueError('Do not support multi control.')
             elif old_label[0] in tuple_RD_list:
                 if len(self.control_list[ii]) > 0:
                     raise ValueError('Do not support control for RD gate.')
                 new_label = old_label[0][1]
                 if self.gate_list[ii].inverse:
                     old_label = (old_label[0], -old_label[1])
-                while old_label[1]/np.pi > 1:
-                    old_label = (old_label[0], old_label[1] - 2*np.pi)
+                while old_label[1] / np.pi > 1:
+                    old_label = (old_label[0], old_label[1] - 2 * np.pi)
                 while old_label[1] / np.pi < -1:
                     old_label = (old_label[0], old_label[1] + 2 * np.pi)
-                if np.abs(old_label[1]/np.pi) == 1:
+                if np.abs(old_label[1] / np.pi) == 1:
                     new_label = new_label
                 elif old_label[1] / np.pi == 0.5:
                     new_label = 'SQRT_' + new_label
                 elif old_label[1] / np.pi == -0.5:
                     new_label = 'SQRT_' + new_label + '_DAG'
                 else:
-                    raise ValueError('Do not support theta/np.pi = ', str(old_label[1]/np.pi))
+                    raise ValueError('Do not support theta/np.pi = ', str(old_label[1] / np.pi))
                 new_position = self.position_list[ii]
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
             stim_circuit.append(new_label, new_position)
         return stim_circuit
 
-
     def to_cirq(self):
-        supported_gates_C = {'CZ':cirq.CZ, 'CX':cirq.CX}
-        supported_gates_R = {'RX':cirq.rx, 'RY':cirq.ry, 'RZ':cirq.rz}
-        supported_gates_CC = {'CCX':cirq.CCX, }
-        supported_gates_U = {'U3':QasmUGate}
+        supported_gates_C = {'CZ': cirq.CZ, 'CX': cirq.CX}
+        supported_gates_R = {'RX': cirq.rx, 'RY': cirq.ry, 'RZ': cirq.rz}
+        supported_gates_CC = {'CCX': cirq.CCX, }
+        supported_gates_U = {'U3': QasmUGate}
         cirq_citcuit = cirq.Circuit()
         for ii in range(len(self)):
             if len(self.control_list[ii]) > 0:
                 raise ValueError('does not support controlled gates')
             tmp_label = self.gate_list[ii].label
             if tmp_label in supported_gates_C.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
@@ -887,15 +893,15 @@
                 position0 = self.qubit_position[self.position_list[ii][0]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
                 cirq_citcuit.append(supported_gates_R[tmp_label[0]](tmp_label[1])(qubit0))
             elif tmp_label[0] in supported_gates_U.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
                 theta, phi, lmda = tmp_label[1]
-                cirq_citcuit.append(supported_gates_U[tmp_label[0]](theta/np.pi, phi/np.pi, lmda/np.pi)(qubit0))
+                cirq_citcuit.append(supported_gates_U[tmp_label[0]](theta / np.pi, phi / np.pi, lmda / np.pi)(qubit0))
             else:
                 raise ValueError(tmp_label, 'is not supported')
         return cirq_citcuit
 
     def cirq_qubit_order(self):
         cirq_order_list = []
 
@@ -909,16 +915,14 @@
         c3d = cirq_web.Circuit3D(cirq_circuit)
         c3d.generate_html_file(file_name=save_path)
 
     def qiskit_draw(self, **kwargs):
         return self.to_qiskit().draw(**kwargs)
 
 
-
-
 def qft(n_qubit, position, control=None, inverse=False, device='cpu', dtype=tc.complex64):
     if control is None:
         control = []
     tmp_circuit = Circuit(n_qubit, device, dtype)
     m_qft = len(position)
     perm = list(range(m_qft))
     perm.reverse()
```

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Gate.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Gate.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/QuantumSimulator/Simulator.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Simulator.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/MPSclass.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/MPSclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TEBD.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TEBD.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence/TEBD/TNclass.py` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TNclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/PKG-INFO` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.7
+Version: 0.0.8
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.7/src/QuantumIntelligence.egg-info/SOURCES.txt` & `QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

