# Comparing `tmp/cipher_parse-0.5.0a2.tar.gz` & `tmp/cipher_parse-0.5.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_parse-0.5.0a2.tar", max compression
+gzip compressed data, was "cipher_parse-0.5.0a3.tar", max compression
```

## Comparing `cipher_parse-0.5.0a2.tar` & `cipher_parse-0.5.0a3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/LICENSE
--rw-r--r--   0        0        0      807 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/README.md
--rw-r--r--   0        0        0      280 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/__init__.py
--rw-r--r--   0        0        0       24 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/_version.py
--rw-r--r--   0        0        0    27477 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/cipher_input.py
--rw-r--r--   0        0        0    30837 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/cipher_output.py
--rw-r--r--   0        0        0      384 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/derived_outputs.py
--rw-r--r--   0        0        0    11603 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/discrete_voronoi.py
--rw-r--r--   0        0        0      603 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/errors.py
--rw-r--r--   0        0        0        0 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/example_data/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 11:54:16.232420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/__init__.py
--rw-r--r--   0        0        0   807612 2023-03-03 11:54:16.236420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-03-03 11:54:16.236420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
--rw-r--r--   0        0        0     2154 2023-03-03 11:54:16.236420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0        0 2023-03-03 11:54:16.236420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/__init__.py
--rw-r--r--   0        0        0 10104120 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
--rw-r--r--   0        0        0     2160 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0    41707 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/geometry.py
--rw-r--r--   0        0        0     5726 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/interface.py
--rw-r--r--   0        0        0     9770 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/material.py
--rw-r--r--   0        0        0     7286 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/quats.py
--rw-r--r--   0        0        0    16893 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/utilities.py
--rw-r--r--   0        0        0    11629 2023-03-03 11:54:16.264420 cipher_parse-0.5.0a2/cipher_parse/voxel_map.py
--rw-r--r--   0        0        0     1533 2023-03-03 11:54:16.268420 cipher_parse-0.5.0a2/pyproject.toml
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 cipher_parse-0.5.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/LICENSE
+-rw-r--r--   0        0        0      807 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/README.md
+-rw-r--r--   0        0        0      280 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/_version.py
+-rw-r--r--   0        0        0    28011 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/cipher_input.py
+-rw-r--r--   0        0        0    35818 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/cipher_output.py
+-rw-r--r--   0        0        0      384 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/derived_outputs.py
+-rw-r--r--   0        0        0    11603 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/discrete_voronoi.py
+-rw-r--r--   0        0        0      603 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/errors.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/example_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/__init__.py
+-rw-r--r--   0        0        0   807612 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2154 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0        0 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/__init__.py
+-rw-r--r--   0        0        0 10104120 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2160 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0    47897 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/geometry.py
+-rw-r--r--   0        0        0     5726 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/interface.py
+-rw-r--r--   0        0        0     9770 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/material.py
+-rw-r--r--   0        0        0     7286 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/quats.py
+-rw-r--r--   0        0        0    20946 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/utilities.py
+-rw-r--r--   0        0        0    12404 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/voxel_map.py
+-rw-r--r--   0        0        0     1612 2023-05-15 13:00:57.343619 cipher_parse-0.5.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 cipher_parse-0.5.0a3/PKG-INFO
```

### Comparing `cipher_parse-0.5.0a2/LICENSE` & `cipher_parse-0.5.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/README.md` & `cipher_parse-0.5.0a3/README.md`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/cipher_input.py` & `cipher_parse-0.5.0a3/cipher_parse/cipher_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -554,127 +554,134 @@
             yaml.dump(cipher_input_data, fp)
 
         return path
 
     def bin_interfaces_by_misorientation_angle(
         self,
         base_interface_name,
-        energy_range,
-        mobility_range,
         theta_max,
+        energy_range=None,
+        mobility_range=None,
         n=4,
         B=5,
         bin_width=5,
         degrees=True,
     ):
-        base_defn, phase_pairs = self.geometry.remove_interface(base_interface_name)
+        if energy_range is None and mobility_range is None:
+            raise ValueError(
+                "Specify at least one of `energy_range` and `mobility_range`."
+            )
+
         if self.geometry.misorientation_matrix is None:
             misori_matrix = self.geometry.get_misorientation_matrix()
         else:
             misori_matrix = self.geometry.misorientation_matrix
 
-        print(f"{bin_width=}")
-
         min_mis, max_mis = np.min(misori_matrix), np.max(misori_matrix)
         min_range = np.floor(min_mis / bin_width) * bin_width
         max_range = np.ceil(max_mis / bin_width) * bin_width + bin_width
         misori_bins = np.linspace(
             min_range,
             max_range,
             num=int((max_range - min_range) / bin_width),
             endpoint=False,
         )
         bin_idx = np.digitize(
             misori_matrix,
             misori_bins,
             right=False,
         )
-        num_bins = misori_bins.size
-        energy_bins = np.linspace(*energy_range, num=num_bins)
-        mobility_bins = np.linspace(*mobility_range, num=num_bins)
-
         theta = (misori_bins + (bin_width / 2))[:-1]
-        print(f"{misori_bins=}")
-        print(f"{theta=}")
 
-        energy = (
-            read_shockley(
-                theta=theta,
-                E_max=(energy_range[1] - energy_range[0]),
-                theta_max=theta_max,
-                degrees=degrees,
+        if not isinstance(base_interface_name, list):
+            base_interface_name = [base_interface_name]
+
+        if energy_range is not None:
+            energy = (
+                read_shockley(
+                    theta=theta,
+                    E_max=(energy_range[1] - energy_range[0]),
+                    theta_max=theta_max,
+                    degrees=degrees,
+                )
+                + energy_range[0]
             )
-            + energy_range[0]
-        )
-        mobility = (
-            grain_boundary_mobility(
-                theta=theta,
-                M_max=(mobility_range[1] - mobility_range[0]),
-                theta_max=theta_max,
-                degrees=degrees,
-                n=n,
-                B=B,
+        if mobility_range is not None:
+            mobility = (
+                grain_boundary_mobility(
+                    theta=theta,
+                    M_max=(mobility_range[1] - mobility_range[0]),
+                    theta_max=theta_max,
+                    degrees=degrees,
+                    n=n,
+                    B=B,
+                )
+                + mobility_range[0]
             )
-            + mobility_range[0]
-        )
 
-        phase_pairs_bin_idx = bin_idx[phase_pairs[0], phase_pairs[1]]
+        for int_name in base_interface_name:
 
-        max_phase_pairs_fmt_len = 10
+            base_defn, phase_pairs = self.geometry.remove_interface(int_name)
 
-        num_existing_int_defns = len(self.geometry.interfaces)
-        print("Preparing new interface defintions...")
-        new_int_idx = 0
-        for bin_idx_i, bin_i in enumerate(misori_bins, start=1):
-
-            phase_pairs_bin_i_idx = np.where(phase_pairs_bin_idx == bin_idx_i)[0]
-            if not phase_pairs_bin_i_idx.size:
-                continue
-
-            else:
-                phase_pairs_bin_i = phase_pairs[:, phase_pairs_bin_i_idx].T
-                phase_pairs_bin_i_fmt = ",".join(
-                    f"{i[0]}-{i[1]}" for i in phase_pairs_bin_i
-                )
-                if len(phase_pairs_bin_i_fmt) > max_phase_pairs_fmt_len:
-                    phase_pairs_bin_i_fmt = (
-                        phase_pairs_bin_i_fmt[: max_phase_pairs_fmt_len - 3] + "..."
-                    )
+            phase_pairs_bin_idx = bin_idx[phase_pairs[0], phase_pairs[1]]
 
-                props = copy.deepcopy(base_defn.properties)
+            max_phase_pairs_fmt_len = 10
 
-                new_e0 = energy[bin_idx_i - 1].item()
-                set_by_path(root=props, path=("energy", "e0"), value=new_e0)
+            num_existing_int_defns = len(self.geometry.interfaces)
+            print("Preparing new interface defintions...")
+            new_int_idx = 0
+            for bin_idx_i, bin_i in enumerate(misori_bins, start=1):
 
-                new_m0 = mobility[bin_idx_i - 1].item()
-                set_by_path(root=props, path=("mobility", "m0"), value=new_m0)
+                phase_pairs_bin_i_idx = np.where(phase_pairs_bin_idx == bin_idx_i)[0]
+                if not phase_pairs_bin_i_idx.size:
+                    continue
 
-                print(
-                    f"  Adding {phase_pairs_bin_i_idx.size!r} phase pair(s) "
-                    f"({phase_pairs_bin_i_fmt}) to bin {bin_idx_i} with mid value: "
-                    f"{theta[bin_idx_i - 1]!r}."
-                )
+                else:
+                    phase_pairs_bin_i = phase_pairs[:, phase_pairs_bin_i_idx].T
+                    phase_pairs_bin_i_fmt = ",".join(
+                        f"{i[0]}-{i[1]}" for i in phase_pairs_bin_i
+                    )
+                    if len(phase_pairs_bin_i_fmt) > max_phase_pairs_fmt_len:
+                        phase_pairs_bin_i_fmt = (
+                            phase_pairs_bin_i_fmt[: max_phase_pairs_fmt_len - 3] + "..."
+                        )
+
+                    props = copy.deepcopy(base_defn.properties)
+
+                    if energy_range is not None:
+                        new_e0 = energy[bin_idx_i - 1].item()
+                        set_by_path(root=props, path=("energy", "e0"), value=new_e0)
+
+                    if mobility_range is not None:
+                        new_m0 = mobility[bin_idx_i - 1].item()
+                        set_by_path(root=props, path=("mobility", "m0"), value=new_m0)
+
+                    print(
+                        f"  Adding {phase_pairs_bin_i_idx.size!r} phase pair(s) "
+                        f"({phase_pairs_bin_i_fmt}) to bin {bin_idx_i} with mid value: "
+                        f"{theta[bin_idx_i - 1]!r}."
+                    )
 
-                new_type_lab = str(new_int_idx)
-                if base_defn.type_label:
-                    new_type_lab = f"{base_defn.type_label}-{new_type_lab}"
-
-                new_int = InterfaceDefinition(
-                    phase_types=base_defn.phase_types,
-                    type_label=new_type_lab,
-                    properties=props,
-                    phase_pairs=phase_pairs_bin_i.tolist(),
-                )
-                self.geometry.interfaces.append(new_int)
-                self.geometry._modify_interface_map(
-                    phase_A=phase_pairs_bin_i[:, 0],
-                    phase_B=phase_pairs_bin_i[:, 1],
-                    interface_idx=(num_existing_int_defns + new_int_idx),
-                )
-                new_int_idx += 1
+                    new_type_lab = str(new_int_idx)
+                    if base_defn.type_label:
+                        new_type_lab = f"{base_defn.type_label}-{new_type_lab}"
+
+                    new_int = InterfaceDefinition(
+                        phase_types=base_defn.phase_types,
+                        type_label=new_type_lab,
+                        properties=props,
+                        phase_pairs=phase_pairs_bin_i.tolist(),
+                    )
+                    self.geometry.interfaces.append(new_int)
+                    self.geometry._modify_interface_map(
+                        phase_A=phase_pairs_bin_i[:, 0],
+                        phase_B=phase_pairs_bin_i[:, 1],
+                        interface_idx=(num_existing_int_defns + new_int_idx),
+                    )
+                    new_int_idx += 1
 
         print("done!")
         self.geometry._check_interface_phase_pairs()
         self.geometry._validate_interfaces()
         self.geometry._validate_interface_map()
 
     def apply_interface_property(
```

### Comparing `cipher_parse-0.5.0a2/cipher_parse/cipher_output.py` & `cipher_parse-0.5.0a3/cipher_parse/cipher_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 import numpy as np
 import pyvista as pv
 import pandas as pd
 import plotly.express as px
 
 from cipher_parse.cipher_input import CIPHERInput
 from cipher_parse.geometry import CIPHERGeometry
-from cipher_parse.utilities import get_subset_indices, get_time_linear_subset_indices
+from cipher_parse.utilities import (
+    get_subset_indices,
+    get_time_linear_subset_indices,
+    update_plotly_figure_animation_slider_to_times,
+)
 from cipher_parse.derived_outputs import num_voxels_per_phase
 
 DEFAULT_PARAVIEW_EXE = "pvbatch"
 INC_DATA_NON_ARRAYS = (
     "increment",
     "time",
     "dimensions",
@@ -159,14 +163,15 @@
         options,
         input_YAML_file_name,
         stdout_file_name,
         input_YAML_file_str,
         stdout_file_str,
         incremental_data,
         quiet=False,
+        cipher_input=None,
     ):
 
         default_options = {
             "paraview_exe": DEFAULT_PARAVIEW_EXE,
             "delete_VTIs": True,
             "delete_VTUs": False,
             "use_existing_VTIs": False,
@@ -181,15 +186,15 @@
         self.input_YAML_file_name = input_YAML_file_name
         self.input_YAML_file_str = input_YAML_file_str
         self.stdout_file_name = stdout_file_name
         self.stdout_file_str = stdout_file_str
         self.incremental_data = incremental_data
         self.quiet = quiet
 
-        self._cipher_input = None
+        self._cipher_input = cipher_input or None
         self._cipher_stdout = None
         self._geometries = None  # assigned by set_geometries
 
         if (
             options.get("VTU_files_time_interval") is not None
             and options.get("num_VTU_files") is not None
         ):
@@ -415,15 +420,15 @@
                     if key not in INC_DATA_NON_ARRAYS:
                         as_list_val = data["incremental_data"][inc_idx][key].tolist()
                         data["incremental_data"][inc_idx][key] = as_list_val
 
         return data
 
     @classmethod
-    def from_JSON(cls, data, quiet=True):
+    def from_JSON(cls, data, cipher_input=None, quiet=True):
 
         attrs = {
             "directory": data["directory"],
             "options": data["options"],
             "input_YAML_file_name": data["input_YAML_file_name"],
             "input_YAML_file_str": data["input_YAML_file_str"],
             "stdout_file_name": data["stdout_file_name"],
@@ -433,15 +438,15 @@
 
         for inc_idx, inc_i in enumerate(attrs["incremental_data"] or []):
             for key, val in inc_i.items():
                 if key not in INC_DATA_NON_ARRAYS and not isinstance(val, np.ndarray):
                     as_arr_val = np.array(attrs["incremental_data"][inc_idx][key])
                     attrs["incremental_data"][inc_idx][key] = as_arr_val
 
-        obj = cls(**attrs, quiet=quiet)
+        obj = cls(**attrs, cipher_input=cipher_input, quiet=quiet)
         geoms = [
             CIPHERGeometry.from_JSON(i, quiet=quiet) for i in data.get("geometries", [])
         ]
         obj._geometries = geoms or None
 
         return obj
 
@@ -512,14 +517,15 @@
         for idx, out_i in enumerate(cipher_outputs):
             (
                 df_hist_i,
                 max_counts_i,
                 max_prob_i,
                 _,
                 max_phase_size_i,
+                available_inc_idx,
             ) = cls._prepare_phase_size_dist_evolution_dataframe(
                 out_i,
                 use_phaseid=use_phaseid,
                 as_probability=as_probability,
                 bin_size=bin_size,
                 max_increments=max_increments,
             )
@@ -722,15 +728,15 @@
                     }
                 )
 
             df_hist_i["evo_idx"] = evo_idx
 
             df_hist = df_hist.append(df_hist_i)
 
-        return df_hist, max_counts, max_prob, bin_size, max_phase_size
+        return df_hist, max_counts, max_prob, bin_size, max_phase_size, avail_inc_idx
 
     def show_phase_size_dist_evolution(
         self,
         use_phaseid=False,
         as_probability=False,
         num_bins=None,
         bin_size=None,
@@ -753,14 +759,15 @@
 
         (
             df_hist,
             max_counts,
             max_prob,
             bin_size,
             max_phase_size,
+            available_inc_idx,
         ) = self._prepare_phase_size_dist_evolution_dataframe(
             self,
             use_phaseid=use_phaseid,
             as_probability=as_probability,
             num_bins=num_bins,
             bin_size=bin_size,
             max_increments=max_increments,
@@ -805,14 +812,101 @@
                 },
                 **(layout_args or {}),
             }
         )
         fig.update_traces(width=bin_size)
         fig.update_traces(marker_line={"width": 0})  # remove gap between stacked bars
 
+        times = [
+            i["time"]
+            for idx, i in enumerate(self.incremental_data)
+            if idx in available_inc_idx
+        ]
+        update_plotly_figure_animation_slider_to_times(fig, times)
+
+        return fig
+
+    def show_misorientation_dist_evolution(
+        self,
+        num_bins=None,
+        bin_size=None,
+        layout_args=None,
+    ):
+
+        all_misori_vox = []
+        inc_dat_indices = []
+        incs = []
+        times = []
+        max_misori = 0
+        for geom in self.geometries:
+            misori_voxels = geom.voxel_map.get_interface_idx(
+                self.cipher_input.geometry.misorientation_matrix
+            ).flatten()
+            misori_voxels = misori_voxels[misori_voxels != -1]
+            all_misori_vox.append(misori_voxels)
+            inc_dat_indices.append(geom.incremental_data_idx)
+            incs.append(geom.increment)
+            times.append(geom.time)
+            max_misori_i = misori_voxels.max()
+            if max_misori_i > max_misori:
+                max_misori = max_misori_i
+
+        if num_bins is not None and bin_size is not None:
+            raise TypeError(f"Specify exactly one of `num_bins` and `bin_size`.")
+        elif num_bins is None and bin_size is None:
+            num_bins = 50
+
+        if bin_size is None:
+            bin_size = max_misori / num_bins
+        else:
+            num_bins = int(max_misori / bin_size)
+
+        bin_edges = np.linspace(0, max_misori + (bin_size / 2), num=num_bins + 1)
+        bin_edges -= bin_size / 2  # so we have a bin centred on zero.
+
+        df_hist = pd.DataFrame()
+        max_counts = 0
+        for idx, voxels in enumerate(all_misori_vox):
+            counts, bins = np.histogram(voxels, bins=bin_edges)
+            max_counts_i = np.max(counts)
+            if max_counts_i > max_counts:
+                max_counts = max_counts_i
+            bin_centres = (np.array(bins) + (bin_size / 2))[:-1]
+            df_hist_i = pd.DataFrame(
+                {
+                    "incremental_data_idx": np.repeat(inc_dat_indices[idx], counts.size),
+                    "increment": np.repeat(incs[idx], counts.size),
+                    "time": np.repeat(times[idx], counts.size),
+                    "misorientation": bin_centres,
+                    "count": counts,
+                }
+            )
+            df_hist = df_hist.append(df_hist_i)
+
+        fig = px.bar(df_hist, x="misorientation", y="count", animation_frame="time")
+
+        # turn off frame transitions:
+        fig.layout.updatemenus[0].buttons[0].args[1]["transition"]["duration"] = 0
+
+        fig.layout.update(
+            {
+                "xaxis": {
+                    "range": [
+                        -bin_size / 2,
+                        np.round(max_misori * 1.1, decimals=6),
+                    ],
+                    "title": "Misorientation /degrees",
+                },
+                "yaxis": {"range": [0, max_counts], "title": "Num. voxels"},
+                **(layout_args or {}),
+            }
+        )
+        fig.update_traces(width=bin_size)
+        fig.update_traces(marker_line={"width": 0})  # remove gap between stacked bars
+
         return fig
 
     def get_geometry(self, inc_data_index):
         start_geom = self.cipher_input.geometry
         inc_dat = self.incremental_data[inc_data_index]
         voxel_phase = inc_dat["phaseid"]
         if start_geom.dimension == 2:
@@ -822,24 +916,27 @@
             materials=start_geom.materials,
             interfaces=start_geom.interfaces,
             size=start_geom.size,
             voxel_phase=voxel_phase,
             allow_missing_phases=True,
             quiet=True,
             time=inc_dat["time"],
+            increment=inc_dat["increment"],
+            incremental_data_idx=inc_data_index,
         )
         return geom
 
     def get_all_geometries(self, include_initial=True):
         """A generator function to provide all available `CIPHERGeometry` objects."""
 
         if include_initial:
             geom_0 = self.cipher_input.geometry
             if geom_0.time is None:
                 geom_0.time = 0
+                geom_0.increment = 0
             yield geom_0
 
         if self._geometries is not None:
             for i in self._geometries:
                 yield i
         else:
             for idx, inc_dat in enumerate(self.incremental_data):
@@ -861,47 +958,78 @@
     def show_slice_evolution(
         self,
         slice_index=0,
         normal_dir="z",
         data_label="phase",
         include=None,
         misorientation_matrix=None,
+        layout_args=None,
+        discrete_colours=None,
+        step_size=None,
         **kwargs,
     ):
+        """
+        Parameters
+        ----------
+        discrete_colours : dict, optional
+            If specified, a dict that maps slice data values to RGB three-tuples.
+        """
         slices = []
         times = []
-        for geom in self.geometries:
+        step_size = step_size or 1
+        for geom in self.geometries[::step_size]:
             slices.append(
                 geom.get_slice(
                     slice_index, normal_dir, data_label, include, misorientation_matrix
                 )[None]
             )
             times.append(geom.time)
 
         slices = np.concatenate(slices)
-        min_val = np.min(slices)
-        max_val = np.max(slices)
-        fig = px.imshow(
-            img=slices,
-            animation_frame=0,
-            color_continuous_scale="viridis",
-            zmin=min_val,
-            zmax=max_val,
-            **kwargs,
-        )
-
-        ani_steps = list(fig.layout.sliders[0]["steps"])
-        ani_steps_new = []
-        for idx, i in enumerate(ani_steps):
-            i["label"] = f"{round(times[idx]):_}"
-            ani_steps_new.append(i)
+        if discrete_colours:
+            slice_RGB = np.tile(slices[..., None], (1, 1, 1, 3)).astype(float)
+            for k, v in discrete_colours.items():
+                slice_RGB[np.where(np.all(slice_RGB == k, axis=3))] = v
+            slices = slice_RGB
+            fig = px.imshow(
+                img=slices,
+                animation_frame=0,
+                **kwargs,
+            )
+        else:
+            min_val = np.min(slices)
+            max_val = np.max(slices)
+            fig = px.imshow(
+                img=slices,
+                animation_frame=0,
+                color_continuous_scale="viridis",
+                zmin=min_val,
+                zmax=max_val,
+                labels={"color": data_label},
+                **kwargs,
+            )
 
-        fig.update_layout(
-            sliders=[
-                {
-                    "currentvalue": {"prefix": "Time = ", "suffix": " s"},
-                    "steps": ani_steps_new,
-                }
-            ]
+        fig.update_layout(layout_args or {})
+        update_plotly_figure_animation_slider_to_times(fig, times)
+        return fig
+
+    def get_average_radius_evolution(self, exclude=None):
+        """Get an evolution proportional to the average radius across all phases."""
+        exclude = exclude or []
+        all_phases_num_voxels = [[] for _ in range(self.geometries[0].num_phases)]
+        times = []
+        for dat_i in self.incremental_data:
+            if "num_voxels_per_phase" in dat_i:
+                for idx, i in enumerate(dat_i["num_voxels_per_phase"]):
+                    if idx in exclude:
+                        i = 0
+                    all_phases_num_voxels[idx].append(i)
+                times.append(dat_i["time"])
+
+        power = 1 / self.geometries[0].dimension
+        all_phases_prop_radius = np.array(
+            [np.power(i, power) for i in all_phases_num_voxels]
         )
+        all_phases_prop_radius[np.isclose(all_phases_prop_radius, 0)] = np.nan
+        prop_avg_radius = np.nanmean(all_phases_prop_radius, axis=0)
 
-        return fig
+        return prop_avg_radius, np.array(times)
```

### Comparing `cipher_parse-0.5.0a2/cipher_parse/discrete_voronoi.py` & `cipher_parse-0.5.0a3/cipher_parse/discrete_voronoi.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/errors.py` & `cipher_parse-0.5.0a3/cipher_parse/errors.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf` & `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/geometry.py` & `cipher_parse-0.5.0a3/cipher_parse/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,34 @@
     GeometryDuplicateMaterialNameError,
     GeometryExcessTargetVolumeFractionError,
     GeometryMissingPhaseAssignmentError,
     GeometryNonUnitTargetVolumeFractionError,
     GeometryUnassignedPhasePairInterfaceError,
     GeometryVoxelPhaseError,
 )
+from cipher_parse.utilities import generate_interface_energies_plot
+from cipher_parse.quats import quat_angle_between
 
 
 class CIPHERGeometry:
     def __init__(
         self,
         materials,
         interfaces,
         size,
         seeds=None,
         voxel_phase=None,
         voxel_map=None,
+        is_periodic=False,
         random_seed=None,
         allow_missing_phases=False,
         quiet=False,
         time=None,
+        increment=None,
+        incremental_data_idx=None,
     ):
         """
         Parameters
         ----------
 
         allow_missing_phases : bool, optional
             If True, allow references to phases that do not appear in the voxel map.
@@ -42,31 +47,35 @@
 
         if sum(i is not None for i in (voxel_phase, voxel_map)) != 1:
             raise ValueError(f"Specify exactly one of `voxel_phase` and `voxel_map`")
         if voxel_map is None:
             voxel_map = VoxelMap(
                 region_ID=voxel_phase,
                 size=size,
-                is_periodic=True,
+                is_periodic=is_periodic,
                 quiet=quiet,
             )
         else:
             voxel_phase = voxel_map.region_ID
+            is_periodic = voxel_map.is_periodic
 
         self._interfaces = None
+        self._is_periodic = is_periodic
 
         self.voxel_map = voxel_map
         self.voxel_phase = voxel_phase
         self.seeds = np.asarray(seeds)
         self.materials = materials
         self.interfaces = interfaces
         self.random_seed = random_seed
         self.size = np.asarray(size)
         self.allow_missing_phases = allow_missing_phases
         self.time = time
+        self.increment = increment
+        self.incremental_data_idx = incremental_data_idx
 
         for i in self.materials:
             i._geometry = self
 
         for idx, i in enumerate(self.interfaces):
             i.index = idx
 
@@ -143,20 +152,23 @@
     def to_JSON(self, keep_arrays=False):
         data = {
             "materials": [i.to_JSON(keep_arrays) for i in self.materials],
             "interfaces": [i.to_JSON(keep_arrays) for i in self.interfaces],
             "size": self.size,
             "seeds": self.seeds,
             "voxel_phase": self.voxel_phase,
+            "is_periodic": self.is_periodic,
             "random_seed": self.random_seed,
             "misorientation_matrix": self.misorientation_matrix,
             "misorientation_matrix_is_degrees": self.misorientation_matrix_is_degrees,
             "allow_missing_phases": self.allow_missing_phases,
             "grain_boundaries": self._grain_boundaries,
             "time": self.time,
+            "increment": self.increment,
+            "incremental_data_idx": self.incremental_data_idx,
         }
         if not keep_arrays:
             data["size"] = data["size"].tolist()
             data["seeds"] = data["seeds"].tolist()
             data["voxel_phase"] = data["voxel_phase"].tolist()
             if data["misorientation_matrix"] is not None:
                 data["misorientation_matrix"] = data["misorientation_matrix"].tolist()
@@ -175,32 +187,33 @@
     def from_JSON(cls, data, quiet=True):
         data_init = {
             "materials": [MaterialDefinition.from_JSON(i) for i in data["materials"]],
             "interfaces": [InterfaceDefinition.from_JSON(i) for i in data["interfaces"]],
             "size": np.array(data["size"]),
             "seeds": np.array(data["seeds"]),
             "voxel_phase": np.array(data["voxel_phase"]),
+            "is_periodic": data.get("is_periodic", False),
             "random_seed": data["random_seed"],
             "allow_missing_phases": data.get("allow_missing_phases", False),
             "time": data.get("time"),
+            "increment": data.get("increment"),
+            "incremental_data_idx": data.get("incremental_data_idx"),
         }
         GBs = {}
         for phase_pair in data.get("grain_boundaries") or []:
             GB = data["grain_boundaries"][phase_pair]
             GBs[phase_pair] = {
                 "interface_idx": GB["interface_idx"],
                 "voxel_indices": tuple(np.array(i) for i in GB["voxel_indices"]),
                 "voxel_coordinates": np.array(GB["voxel_coordinates"]),
                 "centroid": np.array(GB["centroid"]),
             }
         obj = cls(**data_init, quiet=quiet)
-        obj._misorientation_matrix = np.array(data["misorientation_matrix"])
-        obj._misorientation_matrix_is_degrees = np.array(
-            data["misorientation_matrix_is_degrees"]
-        )
+        if data["misorientation_matrix"] is not None:
+            obj._misorientation_matrix = np.array(data["misorientation_matrix"])
         obj._grain_boundaries = GBs or None
         return obj
 
     @property
     def present_phases(self):
         return np.unique(self.voxel_phase)
 
@@ -215,14 +228,18 @@
             phases.append(mat.phases)
         return np.concatenate(phases)
 
     @property
     def interfaces(self):
         return self._interfaces
 
+    @property
+    def is_periodic(self):
+        return self._is_periodic
+
     @interfaces.setter
     def interfaces(self, interfaces):
         self._interfaces = interfaces
         self._validate_interfaces()
 
     @property
     def misorientation_matrix(self):
@@ -608,14 +625,15 @@
     def interface_map_int(self):
         """Get the interface map as an integer matrix, where NaNs are replaced by -2."""
         int_map = np.copy(self.interface_map)
         int_map[np.isnan(int_map)] = -2
         return int_map.astype(int)
 
     def get_interface_idx(self):
+        """Get the interface index associated with each voxel."""
         return self.voxel_map.get_interface_idx(self.interface_map_int)
 
     def get_interface_misorientation(self):
         return self.voxel_map.get_interface_idx(self.misorientation_matrix)
 
     def _modify_interface_map(self, phase_A, phase_B, interface_idx):
         """
@@ -832,14 +850,26 @@
         int_idx = self.voxel_interface_idx
         if self.dimension == 3:
             return int_idx
         else:
             return int_idx.T[:, :, None]
 
     @property
+    def voxel_interface(self):
+        return self.voxel_map.get_interface_voxels()
+
+    @property
+    def voxel_interface_3D(self):
+        int_vox = self.voxel_interface
+        if self.dimension == 3:
+            return int_vox
+        else:
+            return int_vox.T[:, :, None]
+
+    @property
     def voxel_phase_neighbours_3D(self):
         if self.dimension == 3:
             return self.voxel_phase_neighbours
         else:
             return self.voxel_phase_neighbours.T[:, :, None]
 
     def get_slice(
@@ -850,34 +880,40 @@
         include=None,
         misorientation_matrix=None,
     ):
 
         allowed_data = [
             "phase",
             "material",
+            "interface",
             "interface_idx",
             "phase_neighbours",
             "grain_boundaries",
             "GB_misorientation",
+            "IPF_z",
         ]
         if data_label not in allowed_data:
             raise ValueError(f"`data_label` must be one of: {allowed_data}.")
 
         if data_label == "phase":
             data = self.voxel_phase_3D
         elif data_label == "material":
             data = self.voxel_material_3D
+        elif data_label == "interface":
+            data = self.voxel_interface_3D
         elif data_label == "interface_idx":
             data = self.voxel_interface_idx_3D
         elif data_label == "phase_neighbours":
             data = self.voxel_phase_neighbours_3D
         elif data_label == "grain_boundaries":
             data = self.get_grain_boundary_map(as_3D=True)
         elif data_label == "GB_misorientation":
             data = self.voxel_map.get_interface_idx(misorientation_matrix, as_3D=True)
+        elif data_label == "IPF_z":
+            data = self.get_voxel_IPF(IPF_dir=None, as_3D=True)
 
         data = np.copy(data)
         if normal_dir == "x":
             data = data[slice_index, :, :]
         elif normal_dir == "y":
             data = data[:, slice_index, :]
         elif normal_dir == "z":
@@ -895,14 +931,16 @@
     def show_slice(
         self,
         slice_index=0,
         normal_dir="z",
         data_label="phase",
         include=None,
         phase_centroids=False,
+        discrete_colours=None,
+        layout_args=None,
         **kwargs,
     ):
 
         if "misorientation_matrix" in kwargs:
             slice_dat = self.get_slice(
                 slice_index,
                 normal_dir,
@@ -914,44 +952,52 @@
             slice_dat = self.get_slice(
                 slice_index,
                 normal_dir,
                 data_label,
                 include,
             )
 
+        if discrete_colours:
+            slice_RGB = np.tile(slice_dat[..., None], (1, 1, 3)).astype(float)
+            for k, v in discrete_colours.items():
+                slice_RGB[np.where(np.all(slice_RGB == k, axis=2))] = v
+            slice_dat = slice_RGB
+
         fig = px.imshow(
             slice_dat,
             color_continuous_scale="viridis",
             **kwargs,
         )
         if phase_centroids:
             # TODO fix for 3D?
             cents = self.get_phase_voxel_centroids()
             fig.add_scatter(
                 x=cents[:, 1],
                 y=cents[:, 0],
                 text=np.arange(cents.shape[0]),
                 mode="markers",
             )
+        fig.update_layout(layout_args or {})
         return fig
 
     def show(self):
         """Experimental!"""
 
         print("WARNING: experimental!")
 
         grid = self.get_pyvista_grid()
 
         grid.cell_data["interface_idx"] = self.voxel_interface_idx_3D.flatten(order="F")
         grid.cell_data["material"] = self.voxel_material_3D.flatten(order="F")
         grid.cell_data["phase"] = self.voxel_phase_3D.flatten(order="F")
 
-        pl = pv.PlotterITK()
+        # TODO: fix plotter to show multiple cell data
+        pl = pv.Plotter(notebook=True)
         pl.add_mesh(grid)
-        pl.show(ui_collapsed=False)
+        pl.show()
 
     def write_VTK(self, path):
 
         grid = self.get_pyvista_grid()
 
         grid.cell_data["interface_idx"] = self.voxel_interface_idx_3D.flatten(order="F")
         grid.cell_data["material"] = self.voxel_material_3D.flatten(order="F")
@@ -1066,15 +1112,15 @@
         shape = (self.num_known_phases, 4)
         if oris.shape != shape:
             raise ValueError(f"Phase orientations must have shape {shape!r}")
 
         max_idx = 0
         for phase_type in self.phase_types:
             ori_idx = np.arange(max_idx, max_idx + phase_type.num_phases)
-            max_idx = ori_idx[-1]
+            max_idx = ori_idx[-1] + 1
             phase_type.orientations = oris[ori_idx]
 
         self._phase_orientation = self._get_phase_orientation()
 
     @property
     def voxel_material(self):
         """Get the material index of each voxel."""
@@ -1090,22 +1136,22 @@
         """Get the quaternion of each voxel."""
         return self.phase_orientation[self.voxel_phase]
 
     @property
     def material_num_voxels(self):
         mat_num_vox = []
         for i in self.materials:
-            num_vox_i = sum(self.phase_num_voxels[j] for j in i.phases)
+            num_vox_i = sum(self.get_phase_num_voxels()[j] for j in i.phases)
             mat_num_vox.append(num_vox_i)
         return np.array(mat_num_vox)
 
     @property
     def phase_type_num_voxels(self):
         return np.array(
-            [np.sum(self.phase_num_voxels[i.phases]) for i in self.phase_types]
+            [np.sum(self.get_phase_num_voxels()[i.phases]) for i in self.phase_types]
         )
 
     @property
     def material_volume_fractions(self):
         return np.array([i / self.num_voxels for i in self.material_num_voxels])
 
     @property
@@ -1116,14 +1162,28 @@
     def phase_type_volume_fractions(self):
         return np.array([i / self.num_voxels for i in self.phase_type_num_voxels])
 
     @property
     def seeds_grid(self):
         return np.round(self.grid_size * self.seeds / self.size, decimals=0).astype(int)
 
+    def get_voxel_IPF(self, IPF_dir=None, as_3D=False):
+        if IPF_dir is None:
+            IPF_dir = np.array([0, 0, 1])
+        vox_oris = self.voxel_orientation
+        dms_oris = Orientation(vox_oris.reshape((-1, 4)), family="cubic")
+        IPF = dms_oris.IPF_color(IPF_dir)
+        shape = list(vox_oris.shape[:-1]) + [3]
+        vox_IPF = IPF.reshape(shape)
+
+        if self.dimension == 2 and as_3D:
+            return np.transpose(vox_IPF, axes=(1, 0, 2))[:, :, None, :]
+        else:
+            return vox_IPF
+
     def remove_interface(self, interface_name):
         """Remove an interface from the geometry. This will invalidate the geometry if
         the specified interface is referred by any phase-pairs."""
 
         idx = self.interface_names.index(interface_name)
         interface = self.interfaces.pop(idx)
 
@@ -1148,7 +1208,119 @@
 
         if self.dimension == 3:
             return voxel_GBs
         elif as_3D:
             return voxel_GBs.T[:, :, None]
 
         return voxel_GBs
+
+    def get_interface_energies_by_misorientation(self, misorientation_matrix=None):
+        energies_theta = []
+        if misorientation_matrix is None:
+            misorientation_matrix = self.misorientation_matrix
+        for interface_i in self.interfaces:
+            pp_neighbours = []
+            for pp in interface_i.phase_pairs:
+                pp_is_neighbours = np.any(
+                    np.all(pp[:, None] == self.neighbour_list, axis=0)
+                )
+                if pp_is_neighbours:
+                    pp_neighbours.append(pp)
+            pp_neighbours = np.array(pp_neighbours)
+            if pp_neighbours.size:
+                misoris = misorientation_matrix[pp_neighbours[:, 0], pp_neighbours[:, 1]]
+                energies_theta.append(
+                    {
+                        "energy": interface_i.properties["energy"]["e0"],
+                        "mobility": interface_i.properties["mobility"]["m0"],
+                        "misorientation": misoris,
+                        "phase_pairs": pp_neighbours,
+                    }
+                )
+        return energies_theta
+
+    def show_interface_energies_by_misorientation(
+        self,
+        interface_binning,
+        misorientation_matrix=None,
+        colour_by_bin=False,
+        layout_args=None,
+        show_mobility=True,
+    ):
+        energy_range = interface_binning.get("energy_range")
+        mobility_range = interface_binning.get("mobility_range")
+
+        if mobility_range is None:
+            M_min, M_max = None, None
+        else:
+            M_min, M_max = mobility_range
+
+        if energy_range is None:
+            E_min, E_max = None, None
+        else:
+            E_min, E_max = energy_range
+
+        fig = generate_interface_energies_plot(
+            E_min=E_min,
+            E_max=E_max,
+            M_min=M_min,
+            M_max=M_max,
+            theta_max=interface_binning["theta_max"],
+            n=interface_binning.get("n"),
+            B=interface_binning.get("B"),
+        )
+        e_y = []
+        m_y = []
+        x = []
+        color = []
+        hover = []
+        for bin_idx, bin_i in enumerate(
+            self.get_interface_energies_by_misorientation(misorientation_matrix)
+        ):
+            for m_i_idx, m_i in enumerate(bin_i["misorientation"]):
+                e_y.append(bin_i["energy"])
+                m_y.append(bin_i["mobility"])
+                x.append(m_i)
+                color.append(bin_idx)
+                hover.append(
+                    f"({bin_i['phase_pairs'][m_i_idx, 0], bin_i['phase_pairs'][m_i_idx, 1]})"
+                )
+
+        fig.add_scatter(
+            x=x,
+            y=e_y,
+            secondary_y=False,
+            mode="markers",
+            marker_color=color if colour_by_bin else "blue",
+            marker_size=5,
+            hovertext=hover,
+            name="Model GB energies",
+        )
+        if show_mobility:
+            fig.add_scatter(
+                x=x,
+                y=m_y,
+                secondary_y=True,
+                mode="markers",
+                marker_color=color if colour_by_bin else "red",
+                marker_size=5,
+                hovertext=hover,
+            )
+        fig.layout.title = f"Interface properties at increment {self.increment}"
+        fig.update_layout(layout_args or {})
+        return fig
+
+    def show_relative_misorientation(self, layout_args=None):
+        phase_centroids = self.get_phase_voxel_centroids()
+        idx = np.argmin(phase_centroids[:, 0])
+        fig = px.imshow(
+            np.rad2deg(
+                quat_angle_between(
+                    np.tile(
+                        self.phase_orientation[idx], (self.phase_orientation.shape[0], 1)
+                    ),
+                    self.phase_orientation,
+                )
+            )[self.voxel_phase].T
+        )
+        fig.layout.update(layout_args or {})
+        return fig
```

### Comparing `cipher_parse-0.5.0a2/cipher_parse/interface.py` & `cipher_parse-0.5.0a3/cipher_parse/interface.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/material.py` & `cipher_parse-0.5.0a3/cipher_parse/material.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/quats.py` & `cipher_parse-0.5.0a3/cipher_parse/quats.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a2/cipher_parse/voxel_map.py` & `cipher_parse-0.5.0a3/cipher_parse/voxel_map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pyvista as pv
+from cipher_parse.utilities import get_array_edge_mask
 
 
 class VoxelMap:
     def __init__(self, region_ID, size, is_periodic, region_data=None, quiet=False):
         """
         Parameters
         ---------
@@ -85,15 +86,27 @@
         ----------
         dimension :
             Which dimension to consider (0, 1, or 2 [if 3D])
         direction :
             Which direction to consider (-1, +1)
 
         """
-        return np.roll(self.region_ID, shift=direction, axis=dimension)
+
+        region = np.roll(self.region_ID, shift=direction, axis=dimension)
+
+        if not self.is_periodic:
+            idx = 0 if direction == 1 else -1
+            if dimension == 0:
+                region[idx] = self.region_ID[idx]
+            elif dimension == 1:
+                region[:, idx] = self.region_ID[:, idx]
+            elif dimension == 2:
+                region[:, :, idx] = self.region_ID[:, :, idx]
+
+        return region
 
     @property
     def region_ID_above(self):
         return self.get_neighbour_region(self.dimension - 2, 1)
 
     @property
     def region_ID_below(self):
@@ -202,14 +215,20 @@
             print("Finding neighbouring voxels...", end="")
         interface_voxels = np.copy(self.region_ID)
         interface_voxels[self.region_ID_bulk] = -1
         if not quiet:
             print("done!")
         return interface_voxels
 
+    def get_interface_voxels(self):
+        interface_voxels = np.copy(self.region_ID)
+        interface_voxels[self.region_ID_bulk] = -1
+        interface_voxels[interface_voxels != -1] = 0
+        return interface_voxels
+
     def get_neighbour_list(self, quiet=False):
         """Get the pairs of regions that are neighbours"""
         if not quiet:
             print("Finding neighbour list...", end="")
         region_boundary_above = np.array(
             [self.region_ID_flat, self.region_ID_above.reshape(-1)]
         )
@@ -252,15 +271,14 @@
         neighbours = np.unique(region_boundary_all, axis=1)
         if not quiet:
             print("done!")
 
         return neighbours
 
     def get_interface_idx(self, interface_map, as_3D=False):
-
         interface_idx_above_flat = interface_map[
             self.region_ID_flat, self.region_ID_above.reshape(-1)
         ]
         interface_idx_below_flat = interface_map[
             self.region_ID_flat, self.region_ID_below.reshape(-1)
         ]
         interface_idx_left_flat = interface_map[
@@ -306,20 +324,21 @@
                 axis=0,
             )
 
         # avoid self-phase neighbour idx of -1:
         interface_idx_all = np.sort(interface_idx_all, axis=0)[-1]
         interface_idx_all[self.region_ID_bulk] = -1
 
-        if self.dimension == 3:
-            return interface_idx_all
-        elif as_3D:
-            return interface_idx_all.T[:, :, None]
+        if not self.is_periodic:
+            interface_idx_all[get_array_edge_mask(interface_idx_all)] = -1
 
-        return interface_idx_all
+        if self.dimension == 2 and as_3D:
+            return interface_idx_all.T[:, :, None]
+        else:
+            return interface_idx_all
 
     @property
     def grid_size_3D(self):
         if self.dimension == 2:
             return np.hstack([self.grid_size[::-1], 1])
         else:
             return np.asarray(self.grid_size)
@@ -349,10 +368,11 @@
 
         print("WARNING: experimental!")
 
         grid = self.get_pyvista_grid()
 
         grid.cell_data["data"] = self.region_ID.flatten(order="F")
 
-        pl = pv.PlotterITK()
+        # TODO: fix plotter to show multiple cell data
+        pl = pv.Plotter(notebook=True)
         pl.add_mesh(grid)
-        pl.show(ui_collapsed=False)
+        pl.show()
```

### Comparing `cipher_parse-0.5.0a2/pyproject.toml` & `cipher_parse-0.5.0a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "cipher-parse"
-version = "0.5.0a2"
+version = "0.5.0a3"
 description = "Pre- and post-processing for the phase-field code CIPHER."
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d",
     "cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-numpy = "^1.23.0"
-pyvista = "^0.34.2"
+numpy = "1.21"
 h5py = "2.10.0"
 "ruamel.yaml" = "^0.17.21"
 damask = "^3.0.0-alpha.6"
 plotly = "^5.9.0"
 vecmaths = "^0.1.6"
 nbformat = "^5.4.0"
 itkwidgets = ">=0.25.2"
 hickle = {version = "4.0.4", optional = true}
 matflow = {version = "^0.2.26", optional = true}
 notebook = {version = "^6.5.1", optional = true}
 pandas = "^1.5.1"
 parse = "^1.19.0"
 ipywidgets = "<8.0.0"
+sqlalchemy = {version = "<2.0.0", optional = true}
+pyvista = "^0.39.0"
+trame = "^2.4.2"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.12.2"
 ipykernel = "^6.6.1"
 pytest = "^6.2.5"
 commitizen = "^2.20.3"
 pre-commit = "^2.16.0"
@@ -38,20 +40,20 @@
 pydata-sphinx-theme = "^0.8.0"
 sphinx-jinja = "^2.0.1"
 sphinx-copybutton = "^0.5.0"
 black = "^22.3.0"
 
 [tool.poetry.extras]
 hickle = ["hickle"]
-matflow = ["hickle", "matflow"]
+matflow = ["hickle", "matflow", "sqlalchemy"]
 notebook = ["notebook"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0a2"
+version = "0.5.0a3"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "cipher_parse/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `cipher_parse-0.5.0a2/PKG-INFO` & `cipher_parse-0.5.0a3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher-parse
-Version: 0.5.0a2
+Version: 0.5.0a3
 Summary: Pre- and post-processing for the phase-field code CIPHER.
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,20 +18,22 @@
 Requires-Dist: h5py (==2.10.0)
 Requires-Dist: hickle (==4.0.4) ; extra == "hickle" or extra == "matflow"
 Requires-Dist: ipywidgets (<8.0.0)
 Requires-Dist: itkwidgets (>=0.25.2)
 Requires-Dist: matflow (>=0.2.26,<0.3.0) ; extra == "matflow"
 Requires-Dist: nbformat (>=5.4.0,<6.0.0)
 Requires-Dist: notebook (>=6.5.1,<7.0.0) ; extra == "notebook"
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: numpy (==1.21)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: plotly (>=5.9.0,<6.0.0)
-Requires-Dist: pyvista (>=0.34.2,<0.35.0)
+Requires-Dist: pyvista (>=0.39.0,<0.40.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: sqlalchemy (<2.0.0) ; extra == "matflow"
+Requires-Dist: trame (>=2.4.2,<3.0.0)
 Requires-Dist: vecmaths (>=0.1.6,<0.2.0)
 Description-Content-Type: text/markdown
 
 # cipher-parse
 
 **Pre- and post-processing for the phase-field code [CIPHER](https://github.com/micmog/CIPHER)**
```

