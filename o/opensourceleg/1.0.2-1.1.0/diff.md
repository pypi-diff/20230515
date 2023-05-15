# Comparing `tmp/opensourceleg-1.0.2.tar.gz` & `tmp/opensourceleg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.0.2.tar", max compression
+gzip compressed data, was "opensourceleg-1.1.0.tar", max compression
```

## Comparing `opensourceleg-1.0.2.tar` & `opensourceleg-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.0.2/LICENSE
--rw-r--r--   0        0        0     1432 2023-01-26 01:08:26.114716 opensourceleg-1.0.2/README.md
--rw-r--r--   0        0        0      461 2023-02-01 15:15:21.335009 opensourceleg-1.0.2/opensourceleg/__init__.py
--rw-r--r--   0        0        0      309 2023-01-26 01:08:26.115550 opensourceleg-1.0.2/opensourceleg/example.py
--rw-r--r--   0        0        0    76562 2023-03-19 23:39:10.334409 opensourceleg-1.0.2/opensourceleg/hardware.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.0.2/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     4400 2023-03-19 23:25:30.419747 opensourceleg-1.0.2/opensourceleg/statemachine.py
--rw-r--r--   0        0        0    18518 2023-03-19 23:25:36.020569 opensourceleg-1.0.2/opensourceleg/tui.py
--rw-r--r--   0        0        0    11463 2023-02-07 16:16:11.168776 opensourceleg-1.0.2/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-03-19 23:39:26.881688 opensourceleg-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 opensourceleg-1.0.2/setup.py
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 opensourceleg-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.1.0/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.1.0/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    17769 2023-05-11 19:00:34.462414 opensourceleg-1.1.0/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.1.0/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.1.0/opensourceleg/control.py
+-rw-r--r--   0        0        0     3628 2023-05-15 19:07:24.503566 opensourceleg-1.1.0/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.1.0/opensourceleg/example.py
+-rw-r--r--   0        0        0    10266 2023-05-11 18:11:48.618013 opensourceleg-1.1.0/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.1.0/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8887 2023-05-11 18:11:49.772102 opensourceleg-1.1.0/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.1.0/opensourceleg/logger.py
+-rw-r--r--   0        0        0    31248 2023-05-15 18:56:33.702009 opensourceleg-1.1.0/opensourceleg/osl.py
+-rw-r--r--   0        0        0     6705 2023-05-15 18:56:33.342899 opensourceleg-1.1.0/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.1.0/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    18739 2023-04-13 17:07:02.837138 opensourceleg-1.1.0/opensourceleg/tui.py
+-rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.1.0/opensourceleg/units.py
+-rw-r--r--   0        0        0    11463 2023-05-11 15:28:34.400165 opensourceleg-1.1.0/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-05-15 19:21:12.714425 opensourceleg-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.1.0/PKG-INFO
```

### Comparing `opensourceleg-1.0.2/LICENSE` & `opensourceleg-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.0.2/README.md` & `opensourceleg-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# opensourceleg
-
 <div align="center">
 
+# opensourceleg
+
 [![Build status](https://github.com/imsenthur/opensourceleg/workflows/build/badge.svg?branch=master&event=push)](https://github.com/imsenthur/opensourceleg/actions?query=workflow%3Abuild)
 [![Documentation Status](https://readthedocs.org/projects/opensourceleg/badge/?version=latest)](https://opensourceleg.readthedocs.io/en/latest/?badge=latest)
 [![Python Version](https://img.shields.io/pypi/pyversions/opensourceleg.svg)](https://pypi.org/project/opensourceleg/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/imsenthur/opensourceleg/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/imsenthur/opensourceleg/blob/master/.pre-commit-config.yaml)
 [![License](https://img.shields.io/github/license/imsenthur/opensourceleg)](https://github.com/imsenthur/opensourceleg/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
-An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
+An open-source software library for numerical computation, data acquisition, <br>and control of lower-limb robotic prostheses.
+
+<img src="assets/images/banner.gif" width="800" title="Open-Source Leg">
```

### Comparing `opensourceleg-1.0.2/opensourceleg/statemachine.py` & `opensourceleg-1.1.0/opensourceleg/state_machine.py`

 * *Files 27% similar despite different names*

```diff
@@ -44,41 +44,21 @@
     def on_entry(self, callback: Callable[[Any], None]):
         self._entry_callbacks.append(callback)
 
     def on_exit(self, callback: Callable[[Any], None]):
         self._exit_callbacks.append(callback)
 
     def start(self, data: Any):
-        print("Entering: ", self._name)
         for c in self._entry_callbacks:
             c(data)
 
     def stop(self, data: Any):
-        print("Exiting: ", self._name)
         for c in self._exit_callbacks:
             c(data)
 
-    def increase_theta(self, increment=45.5111):
-        self._theta = self._theta + increment
-
-    def decrease_theta(self, decrement=45.5111):
-        self._theta = self._theta - decrement
-
-    def increase_stiffness(self, increment=10):
-        self._k = self._k + increment
-
-    def decrease_stiffness(self, decrement=10):
-        self._k = self._k - decrement
-
-    def increase_damping(self, increment=10):
-        self._b = self._b + increment
-
-    def decrease_damping(self, decrement=10):
-        self._b = self._b - decrement
-
     @property
     def name(self):
         return self._name
 
     @property
     def equilibrium_angle(self):
         return self._theta
@@ -185,7 +165,102 @@
 
             self._from.stop(data)
             self._to.start(data)
 
             return self._to
         else:
             return self._from
+
+
+class StateMachine:
+    def __init__(self, osl=None) -> None:
+        # State Machine Variables
+        self._states: list[State] = []
+        self._events: list[Event] = []
+        self._transitions: list[Transition] = []
+        self._initial_state: Optional[State] = None
+        self._current_state: Optional[State] = None
+        self._exit_callback: Optional[Callable[[Idle, Any], None]] = None
+        self._exit_state = Idle()
+        self.add_state(self._exit_state)
+        self._exited = True
+
+        self._osl = osl
+
+    def add_state(self, state: State, initial_state: bool = False):
+        if state in self._states:
+            raise ValueError("State already exists.")
+
+        self._states.append(state)
+
+        if not self._initial_state and initial_state:
+            self._initial_state = state
+
+    def add_event(self, event: Event):
+        self._events.append(event)
+
+    def add_transition(
+        self,
+        source: State,
+        destination: State,
+        event: Event,
+        callback: Callable[[Any], bool] = None,
+    ) -> Optional[Transition]:
+        transition = None
+
+        if (
+            source in self._states
+            and destination in self._states
+            and event in self._events
+        ):
+            transition = FromToTransition(event, source, destination, callback)
+            self._transitions.append(transition)
+
+        return transition
+
+    def update(self, data: Any = None):
+        validity = False
+
+        if not (self._initial_state or self._current_state):
+            raise ValueError("OSL isn't active.")
+
+        for transition in self._transitions:
+            if transition.source_state == self._current_state:
+                self._current_state = transition(self._osl)
+
+                if isinstance(self._current_state, Idle) and not self._exited:
+                    self._exited = True
+
+                    if self._exit_callback:
+                        self._exit_callback(self._current_state, data)
+
+                validity = True
+                break
+
+        if not validity:
+            self._osl.log.warn(f"Event isn't valid at {self._current_state.name}")
+
+    def start(self, data: Any = None):
+        if not self._initial_state:
+            raise ValueError("Initial state not set.")
+
+        self._current_state = self._initial_state
+        self._exited = False
+        self._current_state.start(data)
+
+    def stop(self, data: Any = None):
+        if not (self._initial_state or self._current_state):
+            raise ValueError("OSL isn't active.")
+
+        self._current_state.stop(data)
+        self._current_state = self._exit_state
+        self._exited = True
+
+    def is_on(self) -> bool:
+        if self._current_state and self._current_state != self._exit_state:
+            return True
+        else:
+            return False
+
+    @property
+    def current_state(self):
+        return self._current_state
```

### Comparing `opensourceleg-1.0.2/opensourceleg/tui.py` & `opensourceleg-1.1.0/opensourceleg/tui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from typing import Callable
 
-import random
-
-import numpy as np
 import TermTk as ttk
 from attr import dataclass
 
 
 # create a dataclass for various colors (str: hex codes)
 @dataclass
 class Colors:
@@ -181,15 +178,15 @@
         self._attribute = attribute
 
     def set_plot_value(self, value: float):
         self._pvalue = [value]
 
     def add_knee(self, knee):
         self._knee = knee
-    
+
     def add_ankle(self, ankle):
         self._ankle = ankle
 
     def run(self):
         self._is_running = True
         self.root_ttk.mainloop()
 
@@ -448,16 +445,20 @@
         Adds a radio button to the TUI
 
         Args:
             name (str): Name of the radio button. Defaults to "radio_button".
             category (str): Category of the radio button; only one radio button can be checked in a category.
                             Defaults to "Attributes".
             parent (str): Parent of the radio button. Defaults to "root".
+            callback (Callable): Callback function for the radio button. Defaults to None.
+            callback_args (list): Arguments for the callback function. Defaults to [].
             color (str): Color of the radio button. Defaults to COLORS.white.
             is_checked (bool): Is the radio button checked? Defaults to False.
+            row (int): Row of the radio button. Defaults to 0.
+            col (int): Column of the radio button. Defaults to 0.
         """
 
         _name = " ".join(name.split("_")).title()
 
         if (
             self._groups[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
@@ -607,26 +608,22 @@
     ):
         name = kwargs["name"]
         args = kwargs["args"]
         category = args[0]
 
         self._categories[category] = name
 
-    def set_active_joint(
-        self, 
-        **kwargs
-    ):
+    def set_active_joint(self, **kwargs):
         name = kwargs["name"]
         parent = kwargs["parent"]
 
         _name = (name + parent).lower()
 
         if "knee" in _name:
             self._joint = self._knee
-        
         elif "ankle" in _name:
             self._joint = self._ankle
 
     def set_loadcell(
         self,
         loadcell,
     ):
@@ -663,35 +660,35 @@
     @property
     def joint(self):
         return self._joint
 
     @property
     def loadcell(self):
         return self._loadcell
-    
+
     @property
     def attribute(self):
         return self._attribute
 
     @property
     def categories(self):
         return self._categories
-    
+
     @property
     def values(self):
         return self._values
 
     @property
     def dropdowns(self):
         return self._dropdowns
-    
+
     @property
     def control_modes(self):
         return self._modes
-    
+
     @property
     def is_running(self):
         return self._is_running
 
 
 if __name__ == "__main__":
     tui = TUI()
```

### Comparing `opensourceleg-1.0.2/opensourceleg/utilities.py` & `opensourceleg-1.1.0/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.0.2/pyproject.toml` & `opensourceleg-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.0.2"
+version = "1.1.0"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.0.2/setup.py` & `opensourceleg-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,49 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: opensourceleg
+Version: 1.1.0
+Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
+Home-page: https://github.com/neurobionics/opensourceleg
+License: GNU GPL v3.0
+Author: Open-source Leg
+Author-email: opensourceleg@gmail.com
+Requires-Python: >=3.9,<4.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: flexsea (>=8.0.1,<9.0.0)
+Requires-Dist: numpy (>=1.22.3,<2.0.0)
+Requires-Dist: pyserial (>=3.5,<4.0)
+Requires-Dist: pytermtk (>=0.22.0a4,<0.23.0)
+Requires-Dist: smbus2 (>=0.4.2,<0.5.0)
+Requires-Dist: sphinx (>=6.1.3,<7.0.0)
+Project-URL: Repository, https://github.com/neurobionics/opensourceleg
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# opensourceleg
+
+[![Build status](https://github.com/imsenthur/opensourceleg/workflows/build/badge.svg?branch=master&event=push)](https://github.com/imsenthur/opensourceleg/actions?query=workflow%3Abuild)
+[![Documentation Status](https://readthedocs.org/projects/opensourceleg/badge/?version=latest)](https://opensourceleg.readthedocs.io/en/latest/?badge=latest)
+[![Python Version](https://img.shields.io/pypi/pyversions/opensourceleg.svg)](https://pypi.org/project/opensourceleg/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/imsenthur/opensourceleg/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/imsenthur/opensourceleg/blob/master/.pre-commit-config.yaml)
+[![License](https://img.shields.io/github/license/imsenthur/opensourceleg)](https://github.com/imsenthur/opensourceleg/blob/master/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
 
-packages = \
-['opensourceleg']
+An open-source software library for numerical computation, data acquisition, <br>and control of lower-limb robotic prostheses.
 
-package_data = \
-{'': ['*']}
+<img src="assets/images/banner.gif" width="800" title="Open-Source Leg">
 
-install_requires = \
-['flexsea>=8.0.1,<9.0.0',
- 'numpy>=1.22.3,<2.0.0',
- 'pyserial>=3.5,<4.0',
- 'pytermtk>=0.22.0a4,<0.23.0',
- 'smbus2>=0.4.2,<0.5.0',
- 'sphinx>=6.1.3,<7.0.0']
-
-setup_kwargs = {
-    'name': 'opensourceleg',
-    'version': '1.0.2',
-    'description': 'An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.',
-    'long_description': '# opensourceleg\n\n<div align="center">\n\n[![Build status](https://github.com/imsenthur/opensourceleg/workflows/build/badge.svg?branch=master&event=push)](https://github.com/imsenthur/opensourceleg/actions?query=workflow%3Abuild)\n[![Documentation Status](https://readthedocs.org/projects/opensourceleg/badge/?version=latest)](https://opensourceleg.readthedocs.io/en/latest/?badge=latest)\n[![Python Version](https://img.shields.io/pypi/pyversions/opensourceleg.svg)](https://pypi.org/project/opensourceleg/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/imsenthur/opensourceleg/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/imsenthur/opensourceleg/blob/master/.pre-commit-config.yaml)\n[![License](https://img.shields.io/github/license/imsenthur/opensourceleg)](https://github.com/imsenthur/opensourceleg/blob/master/LICENSE)\n![Coverage Report](assets/images/coverage.svg)\n\nAn open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.\n',
-    'author': 'Open-source Leg',
-    'author_email': 'opensourceleg@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/neurobionics/opensourceleg',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

