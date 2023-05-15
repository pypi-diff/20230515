# Comparing `tmp/corsika_panama-0.5.2.tar.gz` & `tmp/corsika_panama-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corsika_panama-0.5.2.tar", max compression
+gzip compressed data, was "corsika_panama-0.5.3.tar", max compression
```

## Comparing `corsika_panama-0.5.2.tar` & `corsika_panama-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/LICENSE
--rw-r--r--   0        0        0     5625 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/README.md
--rw-r--r--   0        0        0      364 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/__init__.py
--rw-r--r--   0        0        0       41 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/cli/__init__.py
--rwxr-xr-x   0        0        0      616 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/cli/cli.py
--rw-r--r--   0        0        0     1749 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/cli/corsika_to_hdf5.py
--rw-r--r--   0        0        0     3984 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/cli/run.py
--rw-r--r--   0        0        0      955 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/constants.py
--rw-r--r--   0        0        0      170 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/fluxes/__init__.py
--rw-r--r--   0        0        0     7512 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/fluxes/cosmic_ray_fluxes.py
--rw-r--r--   0        0        0     2566 2023-04-26 01:12:34.312346 corsika_panama-0.5.2/panama/fluxes/flux.py
--rw-r--r--   0        0        0   279551 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/fluxes/gsf_data_table.txt
--rw-r--r--   0        0        0     1865 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/fluxes/muon_fluxes.py
--rw-r--r--   0        0        0     1633 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/nbstreamreader.py
--rw-r--r--   0        0        0     7529 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/prompt.py
--rw-r--r--   0        0        0    15035 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/read.py
--rw-r--r--   0        0        0     8412 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/run.py
--rw-r--r--   0        0        0     5607 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/panama/weights.py
--rw-r--r--   0        0        0     2362 2023-04-26 01:12:34.316347 corsika_panama-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 corsika_panama-0.5.2/setup.py
--rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 corsika_panama-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/LICENSE
+-rw-r--r--   0        0        0     5625 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/README.md
+-rw-r--r--   0        0        0      364 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/cli/__init__.py
+-rwxr-xr-x   0        0        0      616 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/cli/cli.py
+-rw-r--r--   0        0        0     1749 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/cli/corsika_to_hdf5.py
+-rw-r--r--   0        0        0     3984 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/cli/run.py
+-rw-r--r--   0        0        0      955 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/constants.py
+-rw-r--r--   0        0        0      264 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/fluxes/__init__.py
+-rw-r--r--   0        0        0     8983 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/fluxes/cosmic_ray_fluxes.py
+-rw-r--r--   0        0        0     2595 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/fluxes/flux.py
+-rw-r--r--   0        0        0   279551 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/fluxes/gsf_data_table.txt
+-rw-r--r--   0        0        0     1896 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/fluxes/muon_fluxes.py
+-rw-r--r--   0        0        0     1633 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/nbstreamreader.py
+-rw-r--r--   0        0        0     8520 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/prompt.py
+-rw-r--r--   0        0        0    15475 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/read.py
+-rw-r--r--   0        0        0     8412 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/run.py
+-rw-r--r--   0        0        0     5607 2023-05-15 08:39:06.845797 corsika_panama-0.5.3/panama/weights.py
+-rw-r--r--   0        0        0     2362 2023-05-15 08:39:06.849798 corsika_panama-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 corsika_panama-0.5.3/setup.py
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 corsika_panama-0.5.3/PKG-INFO
```

### Comparing `corsika_panama-0.5.2/LICENSE` & `corsika_panama-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/README.md` & `corsika_panama-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/cli/cli.py` & `corsika_panama-0.5.3/panama/cli/cli.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/cli/corsika_to_hdf5.py` & `corsika_panama-0.5.3/panama/cli/corsika_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/cli/run.py` & `corsika_panama-0.5.3/panama/cli/run.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/constants.py` & `corsika_panama-0.5.3/panama/constants.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/fluxes/cosmic_ray_fluxes.py` & `corsika_panama-0.5.3/panama/fluxes/cosmic_ray_fluxes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from abc import ABC
 from pathlib import Path
 from typing import Any
 
 import numpy as np
+from numpy.typing import ArrayLike
 from particle import PDGID, Particle
 from particle.pdgid import literals
 from scipy.interpolate import CubicSpline
 
 from .flux import Flux
 
 
@@ -19,15 +20,15 @@
         for id in validPDGIDs:
             if not (id.is_nucleus or id in self.valid_leptons):
                 raise ValueError(
                     f"{Particle.from_pdgid(id).name} (pdgid: {id}) is not a cosmic ray."
                 )
         super().__init__(validPDGIDs)
 
-    def total_p_and_n_flux(self, E: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+    def total_p_and_n_flux(self, E: ArrayLike) -> tuple[ArrayLike, ArrayLike]:
         """Returns tuple with the total number of protons and neutrons in the flux."""
 
         p_flux = np.zeros(shape=E.shape)
         n_flux = np.zeros(shape=E.shape)
 
         for id in self.validPDGIDs:
             if id in self.valid_leptons:
@@ -37,26 +38,64 @@
             )  # extra factor of A, since flux is differential in E
             p_flux += id.Z * nucleon_flux
             n_flux += (id.A - id.Z) * nucleon_flux
 
         return p_flux, n_flux
 
 
+class GlobalFitGST(CosmicRayFlux):
+    REFERENCE = "https://arxiv.org/pdf/1303.3565v1.pdf"
+    # H He CNO MgAlSi Fe
+    validPDGIDs = [
+        Particle.from_nucleus_info(z, a).pdgid
+        for z, a in [(1, 1), (2, 4), (6, 12), (14, 28), (26, 54)]
+    ]
+
+    def __init__(self) -> None:
+        super().__init__(HillasGaisser.validPDGIDs)
+        self.aij = {}
+        # see Table 3 of reference
+        self.aij[self.validPDGIDs[0]] = [7000, 150.0, 14.0]
+        self.aij[self.validPDGIDs[1]] = [3200, 65.0, 0.0]
+        self.aij[self.validPDGIDs[2]] = [100, 6.0, 0.0]
+        self.aij[self.validPDGIDs[3]] = [130, 7.0, 0.0]
+        self.aij[self.validPDGIDs[4]] = [60, 2.3, 0.025]
+
+        self.gammaij = {}
+        self.gammaij[self.validPDGIDs[0]] = [1.66, 1.4, 1.4]
+        self.gammaij[self.validPDGIDs[1]] = [1.58, 1.3, 0]
+        self.gammaij[self.validPDGIDs[2]] = [1.4, 1.3, 0]
+        self.gammaij[self.validPDGIDs[3]] = [1.4, 1.3, 0]
+        self.gammaij[self.validPDGIDs[4]] = [1.3, 1.2, 1.2]
+
+        self.rigidity_cutoff = [120e3, 4e6, 1.3e9]  # GeV
+
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
+        flux = np.zeros(E.shape)
+
+        for j in range(3):
+            flux += (
+                self.aij[id][j]
+                * E ** (-self.gammaij[id][j] - 1.0)
+                * np.exp(-E / id.Z / self.rigidity_cutoff[j])
+            )
+        return flux
+
+
 class HillasGaisser(CosmicRayFlux):
     """Gaisser, T.K., Astroparticle Physics 35, 801 (2012)."""
 
     REFERENCE = "https://doi.org/10.1016/j.astropartphys.2012.02.010"
     # H He CNO MgAlSi Fe
     validPDGIDs = [
         Particle.from_nucleus_info(z, a).pdgid
         for z, a in [(1, 1), (2, 4), (6, 12), (14, 28), (26, 54)]
     ]
-    rigidity_cutoff = [4e6, 30e6, 2e9]  # GeV
 
-    def __init__(self, ai3: list[float], gamma_pop_3: float) -> None:
+    def __init__(self, ai3: list[float], gamma_pop_3: float, r_pop_3: float) -> None:
         super().__init__(HillasGaisser.validPDGIDs)
         self.aij = {}
         # see Table 1 of reference
         self.aij[self.validPDGIDs[0]] = [7860.0, 20.0]
         self.aij[self.validPDGIDs[1]] = [3550, 20]
         self.aij[self.validPDGIDs[2]] = [2200, 13.4]
         self.aij[self.validPDGIDs[3]] = [1430, 13.4]
@@ -65,41 +104,43 @@
         self.gammaij = {}
         self.gammaij[self.validPDGIDs[0]] = [1.66, 1.4]
         self.gammaij[self.validPDGIDs[1]] = [1.58, 1.4]
         self.gammaij[self.validPDGIDs[2]] = [1.63, 1.4]
         self.gammaij[self.validPDGIDs[3]] = [1.67, 1.4]
         self.gammaij[self.validPDGIDs[4]] = [1.63, 1.4]
 
+        self.rigidity_cutoff = [4e6, 30e6, r_pop_3]  # GeV
+
         # These will come from the instances
         for id in self.validPDGIDs:
             self.gammaij[id].append(gamma_pop_3)
 
         for id, ai3_ in zip(self.validPDGIDs, ai3):
             self.aij[id].append(ai3_)
 
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         flux = np.zeros(E.shape)
 
         for j in range(3):
             flux += (
                 self.aij[id][j]
                 * E ** (-self.gammaij[id][j] - 1.0)
                 * np.exp(-E / id.Z / self.rigidity_cutoff[j])
             )
         return flux
 
 
 class H3a(HillasGaisser):
     def __init__(self) -> None:
-        super().__init__([1.7, 1.7, 1.14, 1.14, 1.14], 1.4)
+        super().__init__([1.7, 1.7, 1.14, 1.14, 1.14], 1.4, 2e9)
 
 
 class H4a(HillasGaisser):
     def __init__(self) -> None:
-        super().__init__([200, 0, 0, 0, 0], 1.6)
+        super().__init__([200, 0, 0, 0, 0], 1.6, 60e9)
 
 
 class BrokenPowerLaw(CosmicRayFlux):
     def __init__(
         self,
         validPDGIDs: list[PDGID],
         gammas: dict[PDGID, list[float]],
@@ -124,15 +165,15 @@
                 )
 
         self.gammas = gammas
         self.normalizations = normalizations
         self.energies = energies
         self.cutoff = cutoff
 
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         flux = np.empty(shape=E.shape)
 
         lowest_mask = self.energies[id][0] >= E
         flux[lowest_mask] = self.normalizations[id][0] * E[lowest_mask] ** (
             -self.gammas[id][0]
         )
 
@@ -230,13 +271,13 @@
 
         validPDGIDs = []
         for i in range(self.elements.shape[0]):
             z = i + 1
             validPDGIDs.append(Particle.from_nucleus_info(z, self.z_to_a[z]).pdgid)
         super().__init__(validPDGIDs)
 
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         return self.splines[id.Z - 1](E)
 
-    def flux_all_particles(self, E: np.ndarray) -> np.ndarray:
+    def flux_all_particles(self, E: ArrayLike) -> ArrayLike:
         """Will be removed in panama 6.x"""
         return self.spline(E)
```

### Comparing `corsika_panama-0.5.2/panama/fluxes/flux.py` & `corsika_panama-0.5.3/panama/fluxes/flux.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 import numpy as np
+from numpy.typing import ArrayLike
 from particle import PDGID, Particle
 
 from ..constants import PDGID_PROTON_1, PDGID_PROTON_2
 
 
 class Flux(ABC):
     """
@@ -22,26 +23,26 @@
 
     REFERENCE = ""
 
     def __init__(self, validPDGIDs: list[PDGID]):
         self.validPDGIDs = validPDGIDs
 
     @abstractmethod
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         """Return a numpy array of the flux in $\frac{1}{m^2 s sr GeV}$
         This should not be used directly and should not throw any error for non-valid PDGids.
         This is handled by Flux.flux
         """
         raise NotImplementedError(
             "Derived class from Flux does not implement the _flux method, which is required."
         )
 
     def flux(
-        self, id: PDGID, E: np.ndarray, check_valid_pdgid: bool = True, **kwargs: Any
-    ) -> np.ndarray:
+        self, id: PDGID, E: ArrayLike, check_valid_pdgid: bool = True, **kwargs: Any
+    ) -> ArrayLike:
         """Returns the differential flux in $\frac{1}{m^2 s sr GeV}$ for particle with PDGid id."""
 
         # the proton has 2 valid PDGIDs: as a proton (2212) or as a Hydrogen nucleus (1000010010)
         # correct for that fact
         if (
             id == PDGID_PROTON_1
             and id not in self.validPDGIDs
@@ -61,14 +62,14 @@
                     f"PDGid {id} ({Particle.from_pdgid(id).name}) not valid for model {self.__class__}. If you want to return flux 0 for invalid PDGids use `check_valid_pdgid = False`."
                 )
             else:
                 return np.zeros(shape=E.shape)
 
         return self._flux(id, E=E, **kwargs)
 
-    def total_flux(self, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def total_flux(self, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         """Returns the total differential flux in $\frac{1}{m^2 s sr GeV}$."""
         total_flux = np.zeros(E.shape)
         for id in self.validPDGIDs:
             total_flux += self._flux(id, E=E, **kwargs)
 
         return total_flux
```

### Comparing `corsika_panama-0.5.2/panama/fluxes/gsf_data_table.txt` & `corsika_panama-0.5.3/panama/fluxes/gsf_data_table.txt`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/fluxes/muon_fluxes.py` & `corsika_panama-0.5.3/panama/fluxes/muon_fluxes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Any
 
 import numpy as np
+from numpy.typing import ArrayLike
 from particle import PDGID, pdgid
 from scipy.special import gamma
 
 from .flux import Flux
 
 
 class MuonFlux(Flux):
@@ -16,15 +17,15 @@
 
 class GaisserFlatEarthHighEnergy(MuonFlux):
     REFERENCE = "ISBN: 978-0521016469, Page 134, Eq. 6.41"
 
     def __init__(self) -> None:
         super().__init__()
 
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         theta = kwargs["theta"] if "theta" in kwargs else 0
 
         return (
             0.5
             * 10_000
             * 0.14
             * E ** (-2.7)
@@ -43,15 +44,15 @@
     gamma = 2.7
     LambdaN = 100  # g/cm^2 (VERY rough! ref: p. 123 of Gaisser, table 5.4)
     epsilon_mu = 1  # GeV table 5.3
 
     def __init__(self) -> None:
         super().__init__()
 
-    def _flux(self, id: PDGID, E: np.ndarray, **kwargs: Any) -> np.ndarray:
+    def _flux(self, id: PDGID, E: ArrayLike, **kwargs: Any) -> ArrayLike:
         theta = kwargs["theta"] if "theta" in kwargs else 0
 
         p1 = self.epsilon_mu / (E * np.cos(theta) + self.alphaX0)
         s = (
             (self.LambdaN * np.cos(theta) / self.X0) ** p1
             * (E / (E + self.alphaX0 / np.cos(theta))) ** (p1 + self.gamma + 1)
             * gamma(p1 + 1)
```

### Comparing `corsika_panama-0.5.2/panama/nbstreamreader.py` & `corsika_panama-0.5.3/panama/nbstreamreader.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/prompt.py` & `corsika_panama-0.5.3/panama/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from math import inf
 
 import numpy as np
 import pandas as pd
+from numpy.typing import ArrayLike
 from particle import Particle
 
 from .constants import D0_LIFETIME, PDGID_ERROR_VAL
 
 
 def is_prompt_lifetime_limit(
     df_particles: pd.DataFrame, lifetime_limit_ns: float = D0_LIFETIME * 10
-) -> np.ndarray:
+) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by the lifetime of the mother particle.
 
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
     lifetime_limit_ns:
         The lifetime limit in nanoseconds above which a particle is considered conventional.
@@ -88,15 +89,15 @@
             df_particles["mother_pdgid_cleaned"].to_numpy(copy=False) == PDGID_ERROR_VAL
         ] = inf
         df_particles["mother_energy_cleaned"] = energy_cleaned
 
 
 def is_prompt_lifetime_limit_cleaned(
     df_particles: pd.DataFrame, lifetime_limit_ns: float = D0_LIFETIME * 10
-) -> np.ndarray:
+) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by lifetime of the mother particle.
     It considers the cleaned particle type of the mother.
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
     Returns
     -------
@@ -109,15 +110,15 @@
     lifetimes = df_particles["mother_lifetime_cleaned"].to_numpy(copy=False)
 
     is_prompt[lifetimes >= lifetime_limit_ns] = False
 
     return is_prompt
 
 
-def is_prompt_energy(df_particles: pd.DataFrame, s: float = 2) -> np.ndarray:
+def is_prompt_energy(df_particles: pd.DataFrame, s: float = 2) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by energy of the mother particle,
        with considering the cleaned particle type of the mother.
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
     s: scaling factor. How much bigger does the decay length has to be compared to the interaction length
     Returns
@@ -138,15 +139,15 @@
     is_prompt = df_particles["mother_energy_cleaned"].to_numpy(
         copy=False
     ) < limit.to_numpy(copy=False)
 
     return is_prompt
 
 
-def is_prompt_pion_kaon(df_particles: pd.DataFrame) -> np.ndarray:
+def is_prompt_pion_kaon(df_particles: pd.DataFrame) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by the pdgid (cleaned)
     of the mother particle. If the mother is a pion or a kaon it is not prompt, otherwise it is.
 
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
 
@@ -160,15 +161,41 @@
     pdgidc = np.abs(df_particles["mother_pdgid_cleaned"].to_numpy(copy=False))
 
     is_prompt[(pdgidc == 211) | (pdgidc == 321) | (pdgidc == PDGID_ERROR_VAL)] = False
 
     return is_prompt
 
 
-def is_prompt_pion_kaon_wrong_pdgid(df_particles: pd.DataFrame) -> np.ndarray:
+def is_prompt_pion_kaon_grandmother(df_particles: pd.DataFrame) -> ArrayLike:
+    """Return a numpy array of prompt labels for the input dataframe differentiating it by the pdgid (cleaned)
+    of the mother particle. If the mother is a pion or a kaon it is not prompt, otherwise it is.
+
+    Parameters
+    ----------
+    df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
+
+    Returns
+    -------
+    A numpy boolean array, True for prompt, False for conventional
+    """
+
+    is_prompt = np.ones(df_particles.shape[0], dtype=bool)
+
+    pdgidc = np.abs(df_particles["mother_pdgid_cleaned"].to_numpy(copy=False))
+    pdgidgm = np.abs(df_particles["grandmother_pdgid"].to_numpy(copy=False))
+
+    is_prompt[(pdgidc == 211) | (pdgidc == 321) | (pdgidc == PDGID_ERROR_VAL)] = False
+    is_prompt[
+        (pdgidgm == 211) | (pdgidgm == 321) | (pdgidgm == PDGID_ERROR_VAL)
+    ] = False
+
+    return is_prompt
+
+
+def is_prompt_pion_kaon_wrong_pdgid(df_particles: pd.DataFrame) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by the pdgid (cleaned)
     of the mother particle. If the mother is a pion or a kaon it is not prompt, otherwise it is.
 
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
 
@@ -182,17 +209,15 @@
     pdgidc = np.abs(df_particles["mother_pdgid"].to_numpy(copy=False))
 
     is_prompt[(pdgidc == 211) | (pdgidc == 321) | (pdgidc == PDGID_ERROR_VAL)] = False
 
     return is_prompt
 
 
-def is_prompt_energy_wrong_pdgid(
-    df_particles: pd.DataFrame, s: float = 2
-) -> np.ndarray:
+def is_prompt_energy_wrong_pdgid(df_particles: pd.DataFrame, s: float = 2) -> ArrayLike:
     """Return a numpy array of prompt labels for the input dataframe differentiating it by energy of the mother particle.
 
     Parameters
     ----------
     df_particles: dataframe with the corsika particles, additional_columns have to be present when running `read_DAT`
     s: scaling factor. How much bigger does the decay length has to be compared to the interaction length
```

### Comparing `corsika_panama-0.5.2/panama/read.py` & `corsika_panama-0.5.3/panama/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             - `mass`
             - `energy`
             - `zenith`
     mother_columns: bool
         Weather to add columns related to the mother/grandmother
         output of the EHIST option.
         They take more time to calculate, since the
-        columns are dependent of each other.
+        rows are dependent of each other.
     drop_mothers: bool
         Weather to remove all mother rows (default: True)
     drop_non_particles: bool
         Weather to remove all rows not representing a real particle (like muon additional information)
         (default: True)
     noparse:
         Use the "noparse" feature of pycorsikaio, which theoretically
@@ -297,111 +297,15 @@
                 mass_map[pdgid] = mass / 1000 if mass is not None else 0  # GeV
 
         df_particles["mass"] = df_particles["pdgid"].map(mass_map, na_action=None)
         df_particles["energy"] = df_particles.eval("sqrt(mass**2+px**2+py**2+pz**2)")
         df_particles["zenith"] = df_particles.eval("arccos(pz/sqrt(px**2+py**2+pz**2))")
 
         if mother_columns:
-            mother_index = np.arange(-2, df_particles.shape[0] - 2)
-            mother_index[0] = df_particles.shape[0] - 2
-            mother_index[1] = df_particles.shape[0] - 1
-
-            grandmother_index = np.arange(-1, df_particles.shape[0] - 1)
-            grandmother_index[0] = df_particles.shape[0] - 1
-
-            df_particles["has_mother"] = df_particles["is_mother"].iloc[
-                mother_index
-            ].to_numpy(copy=False) & df_particles["is_mother"].iloc[
-                grandmother_index
-            ].to_numpy(
-                copy=False
-            )
-
-            df_particles["mother_hadr_gen"] = (
-                np.abs(df_particles["particle_description"].iloc[mother_index].array)
-                % 100
-            )
-            df_particles.loc[
-                ~df_particles["has_mother"].array, "mother_hadr_gen"
-            ] = pd.NA
-
-            # copy mother values to daughter columns so we can drop them later
-            for name, error_val in (
-                ("pdgid", PDGID_ERROR_VAL),
-                ("energy", pd.NA),
-                ("mass", pd.NA),
-            ):
-                df_particles[f"mother_{name}"] = (
-                    df_particles[name].iloc[mother_index].to_numpy(copy=False)
-                )
-                df_particles.loc[
-                    ~df_particles["has_mother"].array, f"mother_{name}"
-                ] = error_val
-
-            has_charm = {
-                pdgid: "c" in Particle.from_pdgid(pdgid).quarks.lower()
-                if pdgid != PDGID_ERROR_VAL
-                else False
-                for pdgid in pdgids
-            }
-
-            # this follows the MCEq definition
-            lifetimes = {
-                pdgid: Particle.from_pdgid(pdgid).lifetime
-                if pdgid != PDGID_ERROR_VAL
-                else inf
-                for pdgid in pdgids
-            }
-            for pdgid in lifetimes:
-                if lifetimes[pdgid] is None:
-                    lifetimes[pdgid] = 0
-
-            is_resonance = {
-                pdgid: "*" in Particle.from_pdgid(pdgid).name
-                if pdgid != PDGID_ERROR_VAL
-                else False
-                for pdgid in pdgids
-            }
-
-            df_particles["mother_has_charm"] = df_particles["mother_pdgid"].map(
-                has_charm, na_action=None
-            )
-            df_particles["mother_lifetimes"] = (
-                df_particles["mother_pdgid"].map(lifetimes, na_action=None).array
-            )
-            df_particles["mother_is_resonance"] = df_particles["mother_pdgid"].map(
-                is_resonance, na_action=None
-            )
-
-            dif = df_particles["hadron_gen"].to_numpy(copy=False) - df_particles[
-                "mother_hadr_gen"
-            ].to_numpy(copy=False)
-
-            is_pion_decay = (dif == 51) & (
-                (df_particles["mother_pdgid"].to_numpy(copy=False) == 111)
-                | (df_particles["mother_pdgid"].to_numpy(copy=False) == 211)
-                | (df_particles["mother_pdgid"].to_numpy(copy=False) == -211)
-            )
-
-            # this adds a cleaned version of the mother_pdgid
-            # where the pdgid is replaced with the pdg error value
-            # if we can't tell the motherpdgid for sure
-            df_particles["mother_pdgid_cleaned"] = df_particles["mother_pdgid"]
-            no_true_mother_idxs = ~(
-                ((dif == 1) | (dif == 0))
-                & ~df_particles["mother_is_resonance"].to_numpy(copy=False)
-                | df_particles["mother_has_charm"].to_numpy(copy=False)
-                | is_pion_decay
-            )
-            df_particles.loc[
-                no_true_mother_idxs,
-                "mother_pdgid_cleaned",
-            ] = PDGID_ERROR_VAL
-
-            df_particles["is_prompt"] = is_prompt_lifetime_limit(df_particles)
+            add_mother_columns(df_particles, pdgids)
 
     if drop_mothers:
         df_particles.drop(
             index=df_particles.query("particle_description < 0").index.array,
             inplace=True,
         )
 
@@ -411,7 +315,126 @@
         )
 
     df_particles.set_index(
         keys=["run_number", "event_number", "particle_number"], inplace=True
     )
 
     return df_run_headers, df_event_headers, df_particles
+
+
+def add_mother_columns(df_particles: pd.DataFrame, pdgids: list[int] | None) -> None:
+    """
+    Adds the information from mother and grandmother rows to
+    the particle column.
+
+    This looks so complicated, since in the table different rows
+    depend on each other. To do this in a numpy-friendly way is not
+    that trivial. (We do not want to iterate through the rows -> python loops)
+    So this is done via a shifted index array.
+
+    Parameters
+    ----------
+    df_particles : DataFrame
+        the particle dataframe with additional columns from read_DAT
+    pdgids : list[int] | None
+        The unique pdgids in the dataframe. If none, they are calculated.
+    """
+    if pdgids is None:
+        pdgids = df_particles["pdgid"].unique()
+
+    mother_index = np.arange(-2, df_particles.shape[0] - 2)
+    mother_index[0] = df_particles.shape[0] - 2
+    mother_index[1] = df_particles.shape[0] - 1
+
+    grandmother_index = np.arange(-1, df_particles.shape[0] - 1)
+    grandmother_index[0] = df_particles.shape[0] - 1
+
+    df_particles["has_mother"] = df_particles["is_mother"].iloc[mother_index].to_numpy(
+        copy=False
+    ) & df_particles["is_mother"].iloc[grandmother_index].to_numpy(copy=False)
+
+    df_particles["mother_hadr_gen"] = (
+        np.abs(df_particles["particle_description"].iloc[mother_index].array) % 100
+    )
+    df_particles.loc[~df_particles["has_mother"].array, "mother_hadr_gen"] = pd.NA
+
+    # copy mother values to daughter columns so we can drop them later
+    for name, error_val in (
+        ("pdgid", PDGID_ERROR_VAL),
+        ("energy", pd.NA),
+        ("mass", pd.NA),
+    ):
+        df_particles[f"mother_{name}"] = (
+            df_particles[name].iloc[mother_index].to_numpy(copy=False)
+        )
+        df_particles.loc[
+            ~df_particles["has_mother"].array, f"mother_{name}"
+        ] = error_val
+
+    # copy grandmother values to daughter columns so we can drop them later
+    for name, error_val in (("pdgid", PDGID_ERROR_VAL),):
+        df_particles[f"grandmother_{name}"] = (
+            df_particles[name].iloc[grandmother_index].to_numpy(copy=False)
+        )
+        df_particles.loc[
+            ~df_particles["has_mother"].array, f"mother_{name}"
+        ] = error_val
+
+    has_charm = {
+        pdgid: "c" in Particle.from_pdgid(pdgid).quarks.lower()
+        if pdgid != PDGID_ERROR_VAL
+        else False
+        for pdgid in pdgids
+    }
+
+    # this follows the MCEq definition
+    lifetimes = {
+        pdgid: Particle.from_pdgid(pdgid).lifetime if pdgid != PDGID_ERROR_VAL else inf
+        for pdgid in pdgids
+    }
+    for pdgid in lifetimes:
+        if lifetimes[pdgid] is None:
+            lifetimes[pdgid] = 0
+
+    is_resonance = {
+        pdgid: "*" in Particle.from_pdgid(pdgid).name
+        if pdgid != PDGID_ERROR_VAL
+        else False
+        for pdgid in pdgids
+    }
+
+    df_particles["mother_has_charm"] = df_particles["mother_pdgid"].map(
+        has_charm, na_action=None
+    )
+    df_particles["mother_lifetimes"] = (
+        df_particles["mother_pdgid"].map(lifetimes, na_action=None).array
+    )
+    df_particles["mother_is_resonance"] = df_particles["mother_pdgid"].map(
+        is_resonance, na_action=None
+    )
+
+    dif = df_particles["hadron_gen"].to_numpy(copy=False) - df_particles[
+        "mother_hadr_gen"
+    ].to_numpy(copy=False)
+
+    is_pion_decay = (dif == 51) & (
+        (df_particles["mother_pdgid"].to_numpy(copy=False) == 111)
+        | (df_particles["mother_pdgid"].to_numpy(copy=False) == 211)
+        | (df_particles["mother_pdgid"].to_numpy(copy=False) == -211)
+    )
+
+    # this adds a cleaned version of the mother_pdgid
+    # where the pdgid is replaced with the pdg error value
+    # if we can't tell the motherpdgid for sure
+    df_particles["mother_pdgid_cleaned"] = df_particles["mother_pdgid"]
+    no_true_mother_idxs = ~(
+        ((dif == 1) | (dif == 0))
+        & ~df_particles["mother_is_resonance"].to_numpy(copy=False)
+        | df_particles["mother_has_charm"].to_numpy(copy=False)
+        | is_pion_decay
+    )
+    df_particles.loc[
+        no_true_mother_idxs,
+        "mother_pdgid_cleaned",
+    ] = PDGID_ERROR_VAL
+
+    df_particles["is_prompt"] = is_prompt_lifetime_limit(df_particles)
```

### Comparing `corsika_panama-0.5.2/panama/run.py` & `corsika_panama-0.5.3/panama/run.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/panama/weights.py` & `corsika_panama-0.5.3/panama/weights.py`

 * *Files identical despite different names*

### Comparing `corsika_panama-0.5.2/pyproject.toml` & `corsika_panama-0.5.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corsika-panama"
-version = "0.5.2"
+version = "0.5.3"
 description = "PANdas And Multicore utils for corsikA7"
 authors = ["Ludwig Neste <ludwig.neste@tu-dortmund.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "panama" }]
 homepage = "https://github.com/The-Ludwig/PANAMA"
 repository = "https://github.com/The-Ludwig/PANAMA"
```

### Comparing `corsika_panama-0.5.2/setup.py` & `corsika_panama-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tqdm>=4.64.1,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['panama = panama.cli:cli']}
 
 setup_kwargs = {
     'name': 'corsika-panama',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'PANdas And Multicore utils for corsikA7',
     'long_description': '# PAN*das* A*nd* M*ulticore utils for corsik*A*7*\n\n[Documentation ![Read the Docs](https://img.shields.io/readthedocs/panama?style=for-the-badge)](https://panama.readthedocs.io/en/latest/)\n\n[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/The-Ludwig/PANAMA/ci.yml?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/actions/workflows/ci.yml)\n[![Codecov](https://img.shields.io/codecov/c/github/The-Ludwig/PANAMA?label=test%20coverage&style=for-the-badge)](https://app.codecov.io/gh/The-Ludwig/PANAMA)\n[![PyPI](https://img.shields.io/pypi/v/corsika-panama?style=for-the-badge)](https://pypi.org/project/corsika-panama/)\n\n[![GitHub issues](https://img.shields.io/github/issues-raw/The-Ludwig/PANAMA?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/issues)\n[![GitHub](https://img.shields.io/github/license/The-Ludwig/PANAMA?style=for-the-badge)](https://github.com/The-Ludwig/PANAMA/blob/main/LICENSE)\n[![Codestyle](https://img.shields.io/badge/codesyle-Black-black.svg?style=for-the-badge)](https://github.com/psf/black)\n\nThanks [@Jean1995](https://github.com/Jean1995) for the silly naming idea.\n\n## Installation\n\n```\npip install corsika-panama\n```\n\n## Features\n\n### Run CORSIKA7 on multiple cores\n\nYou need to have [`CORSIKA7`](https://www.iap.kit.edu/corsika/79.php) installed to run this.\n\nRunning 100 showers on 4 cores with primary being proton:\n\n```sh\n$ panama run --corsika path/to/corsika7/executable -j4 ./tests/files/example_corsika.template\n83%|████████████████████████████████████████████████████▋        | 83.0/100 [00:13<00:02, 6.36shower/s]\nJobs should be nearly finished, now we wait for them to exit\nAll jobs terminated, cleanup now\n```\n\nInjecting 5 different primaries (Proton, Helium-4, Carbon-12, Silicon-28, Iron-54 roughly aligning with grouping in H3a) with each primary shower taking 10 jobs:\n\n```sh\n$ panama run --corsika corsika-77420/run/corsika77420Linux_SIBYLL_urqmd --jobs 10 --primary ""{2212: 500, 1000020040: 250, 1000060120: 50, 1000140280: 50, 1000260540: 50}"" ./tests/files/example_corsika.template\n...\n```\n\n### Convert CORSIKA7 DAT files to hdf5 files\n\n```sh\n$ panama hdf5 path/to/corsika/dat/files/DAT* output.hdf5\n```\n\nThe data is available under the `run_header` `event_header` and `particles` key.\n\n### Read CORSIKA7 DAT files to pandas dataframes\n\nExample: Calculate mean energy in the corsika files created in the example above:\n\n```\nIn [1]: import panama as pn\n\nIn [2]: run_header, event_header, particles = pn.read_DAT(glob="corsika_output/DAT*")\n100%|████████████████████████████████████████████████████████████| 2000/2000.0 [00:00<00:00, 10127.45it/s]\nIn [3]: particles["energy"].mean()\nOut[3]: 26525.611020413744\n```\n\n`run_header`, `event_header` and `particles` are all [pandas.DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) and can conveniently be used.\n\nIf `CORSIKA7` is compiled with the `EHIST` option, then the mother particles are automatically deleted, by default (this behaviour can be changed with`drop_mothers=False`).\nIf you want additional columns in the real particles storing the mother information use `mother_columns=True`.\n\n### Weighting to primary spectrum\n\nThis packages also provides facility to add a `weight` column to the dataframe, so you can look at corsika-output\nin physical flux in terms of $(\\mathrm{m^2} \\mathrm{s}\\ \\mathrm{sr}\\ \\mathrm{GeV})^{-1}$.\nUsing the example above, to get the whole physical flux in the complete simulated energy region:\n\n```\nIn [1]: import panama as pn\n\nIn [2]: run_header, event_header, particles = pn.read_DAT(glob="corsika_output/DAT*")\n100%|████████████████████████████████████████████████████████████| 2000/2000.0 [00:00<00:00, 10127.45it/s]\nIn [3]: pn.add_weight(run_header, event_header, particles)\n\nIn [4]: particles["weight"].sum()*(run_header["energy_max"]-run_header["energy_min"])\nOut[4]:\nrun_number\n1.0    1234.693481\n0.0    1234.693481\n3.0    1234.693481\n2.0    1234.693481\ndtype: float32\n\n```\n\nWhich is in units of $(\\mathrm{m^2}\\ \\mathrm{s}\\ \\mathrm{sr})^{-1}$. We get a result for each run, since\nin theory we could have different energy regions. Here, we do not, so the result is always equal.\n\nWeighting can be applied to different primaries, also, if they are known by the flux model.\n\n`add_weight` can also be applied to dataframes loaded in from hdf5 files produced with PANAMA.\n\nTODO: Better documentation of weighting (what is weighted, how, proton/neutrons, area...?)\n\n#### Notes:\n\nThis started a little while ago while I was looking into the `EHIST` option\nof corsika.\nI wanted a way of conveniently running CORSIKA7 on more than 1 core.\nI ended in the same place where most CORSIKA7 users end (see e.g. [fact-project/corsika_wrapper](https://github.com/fact-project/corsika_wrapper))\nand wrote a small wrapper.\n\nread_DAT made possible by [cta-observatory/pycorsikaio](https://github.com/cta-observatory/pycorsikaio).\n\n#### Pitfalls\n\n- The whole `run` folder of CORSIKA7 must be copied for each process, so very high parallel runs have high overhead\n- If you simulate to low energies, python can\'t seem to hold up with the corsika output to `stdin` and essentially slows down corsika this is still a bug in investigation #1\n\n## What this is not\n\nBug-free or stable\n',
     'author': 'Ludwig Neste',
     'author_email': 'ludwig.neste@tu-dortmund.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/The-Ludwig/PANAMA',
```

### Comparing `corsika_panama-0.5.2/PKG-INFO` & `corsika_panama-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corsika-panama
-Version: 0.5.2
+Version: 0.5.3
 Summary: PANdas And Multicore utils for corsikA7
 Home-page: https://github.com/The-Ludwig/PANAMA
 License: MIT
 Author: Ludwig Neste
 Author-email: ludwig.neste@tu-dortmund.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

