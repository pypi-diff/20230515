# Comparing `tmp/neuromllite-0.5.3.tar.gz` & `tmp/neuromllite-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neuromllite-0.5.3.tar", last modified: Mon Oct 17 16:13:14 2022, max compression
+gzip compressed data, was "neuromllite-0.5.4.tar", last modified: Mon May 15 10:59:11 2023, max compression
```

## Comparing `neuromllite-0.5.3.tar` & `neuromllite-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2022-10-17 16:13:14.000000 neuromllite-0.5.3/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     9747 2022-10-17 16:13:14.000000 neuromllite-0.5.3/PKG-INFO
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7493 2022-10-17 15:26:13.000000 neuromllite-0.5.3/README.md
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    14680 2022-03-17 14:53:37.000000 neuromllite-0.5.3/neuromllite/ArborHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    10849 2021-12-08 09:54:21.000000 neuromllite-0.5.3/neuromllite/BBPConnectomeReader.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7015 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/BindsNETHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7024 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/ConnectivityHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7193 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/DefaultNetworkHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    33672 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/GraphVizHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    14690 2022-08-31 08:17:50.000000 neuromllite-0.5.3/neuromllite/MDFHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    19527 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/MatrixHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    88923 2022-10-17 15:26:13.000000 neuromllite-0.5.3/neuromllite/NetworkGenerator.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     9097 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/NeuronHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     8734 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/PsyNeuLinkHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    12045 2021-12-08 09:54:21.000000 neuromllite-0.5.3/neuromllite/PsyNeuLinkReader.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     8984 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/PyNNHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     7993 2022-10-17 15:26:13.000000 neuromllite-0.5.3/neuromllite/SonataHandler.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    51976 2021-12-08 09:54:21.000000 neuromllite-0.5.3/neuromllite/SonataReader.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    17099 2022-10-17 16:12:53.000000 neuromllite-0.5.3/neuromllite/__init__.py
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite/gui/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    45226 2022-08-18 11:13:22.000000 neuromllite-0.5.3/neuromllite/gui/NMLliteUI.py
--rw-r--r--   0 padraig   (1000) padraig   (1000)        0 2021-05-18 14:46:47.000000 neuromllite-0.5.3/neuromllite/gui/__init__.py
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite/sweep/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1158 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/sweep/GenerateTests.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)    27090 2021-12-02 14:41:04.000000 neuromllite-0.5.3/neuromllite/sweep/ParameterSweep.py
--rw-r--r--   0 padraig   (1000) padraig   (1000)        0 2021-05-18 14:46:47.000000 neuromllite-0.5.3/neuromllite/sweep/__init__.py
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     8026 2022-08-18 11:13:22.000000 neuromllite-0.5.3/neuromllite/utils.py
-drwxrwxr-x   0 padraig   (1000) padraig   (1000)        0 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     9747 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/PKG-INFO
--rw-rw-r--   0 padraig   (1000) padraig   (1000)      895 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/SOURCES.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)        1 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/dependency_links.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       63 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/entry_points.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       60 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/requires.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       12 2022-10-17 16:13:14.000000 neuromllite-0.5.3/neuromllite.egg-info/top_level.txt
--rw-rw-r--   0 padraig   (1000) padraig   (1000)       38 2022-10-17 16:13:14.000000 neuromllite-0.5.3/setup.cfg
--rw-rw-r--   0 padraig   (1000) padraig   (1000)     1445 2022-10-17 15:26:13.000000 neuromllite-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.855770 neuromllite-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-15 10:59:01.000000 neuromllite-0.5.4/LICENSE.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-15 10:59:11.855770 neuromllite-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-15 10:59:01.000000 neuromllite-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite/
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/ArborHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/BBPConnectomeReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/BindsNETHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/ConnectivityHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/DefaultNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33672 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/GraphVizHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22883 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/MDFHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/MatrixHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89346 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/NetworkGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/NeuronHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PsyNeuLinkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PsyNeuLinkReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/PyNNHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/SonataHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51976 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/SonataReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)    45481 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/gui/NMLliteUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.855770 neuromllite-0.5.4/neuromllite/sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/GenerateTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27090 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/ParameterSweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-15 10:59:01.000000 neuromllite-0.5.4/neuromllite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:59:11.851770 neuromllite-0.5.4/neuromllite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 10:59:11.000000 neuromllite-0.5.4/neuromllite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:59:11.855770 neuromllite-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-15 10:59:01.000000 neuromllite-0.5.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neuromllite-0.5.3/PKG-INFO` & `neuromllite-0.5.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,193 +1,193 @@
 Metadata-Version: 2.1
 Name: neuromllite
-Version: 0.5.3
+Version: 0.5.4
 Summary: A common JSON/YAML based format for compact network specification, closely tied to NeuroML v2
 Home-page: https://github.com/NeuroML/NeuroMLlite
 Author: Padraig Gleeson
 Author-email: p.gleeson@gmail.com
 License: LICENSE.lesser
-Description: ## NeuroMLlite: a common framework for reading/writing/generating network specifications based on NeuroML
-        
-        [![Continuous builds](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml)
-        [![PyPI](https://img.shields.io/pypi/v/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
-        [![GitHub](https://img.shields.io/github/license/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/blob/master/LICENSE.lesser)
-        [![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/pulls)
-        [![GitHub issues](https://img.shields.io/github/issues/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/issues)
-        [![GitHub Org's stars](https://img.shields.io/github/stars/NeuroML?style=social)](https://github.com/NeuroML)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
-        
-        
-        NeuroMLlite is in active development. This will evolve into a framework for more portable, concise network specifications which will form an important part of [NeuroML v3](https://docs.neuroml.org/NeuroMLOrg/History.html#the-future).
-        
-        For some more background to this package see here: https://github.com/NeuroML/NetworkShorthand.
-        
-        ![Architecture](images/NetworkShorthand.png)
-        
-        
-        ## Examples
-        The best way to see the currently proposed structure is to look at the examples
-        
-        ### Ex. 1: Simple network, 2 populations & projection
-        ![Ex1](examples/images/Ex1.png)
-        
-        [JSON](examples/Example1_TestNetwork.json) | [Python script](examples/Example1.py)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        ### Ex. 2: Simple network, 2 populations, projection & inputs
-        ![Ex2](examples/images/Ex2.png)
-        
-        [JSON](examples/Example2_TestNetwork.json) | [Python script](examples/Example2.py) | [Generated NeuroML2](examples/Example2_TestNetwork.net.nml)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        ### Ex. 3: As above, with simulation specification
-        
-        [JSON for network](examples/Example3_Network.json) | [JSON for simulation](examples/SimExample3.json) | [Python script](examples/Example3.py) | [Generated NeuroML2](examples/Example3_Network.net.nml) | [Generated LEMS](examples/LEMS_SimExample3.xml)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see Ex2) 
-        
-        Can be simulated using:
-        - **NetPyNE**
-        - **jNeuroML**
-        - **NEURON** generated from **jNeuroML**
-        - **NetPyNE** generated from **jNeuroML**
-        
-        
-        ### Ex. 4: A network with PyNN cells & inputs
-        <img alt="Ex4" src="examples/images/Ex4.png" height="250"/>
-        
-        [JSON](examples/Example4_PyNN.json) | [Python script](examples/Example4.py) | [Generated NeuroML2](examples/Example4_PyNN.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        Can be simulated using:
-        - **NEST** via **PyNN**
-        - **NEURON** via **PyNN**
-        - **Brian** via **PyNN**
-        - **jNeuroML**
-        - **NEURON** generated from **jNeuroML**
-        - **NetPyNE** generated from **jNeuroML**
-        
-        
-        ### Ex. 5: A network with the Blue Brain Project connectivity data
-        <img alt="Ex5" src="examples/images/Ex5_BBP_5percent.png" height="150"/> 
-        
-        <img alt="Ex5_1" src="examples/images/bbp1.png" height="200"/>  <img alt="Ex5_2" src="examples/images/bbp2.png" height="200"/> <img alt="Ex5_3" src="examples/images/bbp3.png" height="200"/> 
-        
-        [JSON](examples/BBP_5percent.json) | [Python script](examples/Example5.py) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        - **Matrix** (see above) 
-        
-        Can be simulated using:
-        - **NetPyNE**
-        
-        ### Ex. 6: A network based on Potjans and Diesmann 2014 (work in progress)
-        <img alt="Ex6d" src="examples/images/Ex6.dot.png" height="100"/> <img alt="Ex6f" src="examples/images/Ex6.fdp.png" height="100"/>  <img alt="Ex6c" src="examples/images/Ex6.circo.png" height="100"/> 
-        <img alt="Ex6matrix" src="examples/images/Ex6matrix.png" height="300"/> 
-        
-        [JSON](examples/Example6_PyNN.json) | [Python script](examples/Example6.py) | [Generated NeuroML2](examples/Example6_PyNN.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        - **Matrix** (see above) 
-        
-        ### Ex. 7: A network based on Brunel 2000 (work in progress)
-        <img alt="Ex7" src="examples/images/Ex7.png" height="250"/> 
-        
-        [JSON](examples/Example7_Brunel2000.json) | [Python script](examples/Example7.py) | [Generated NeuroML2](examples/Example7_Brunel2000.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        Can be simulated using:
-        - **jNeuroML**
-        
-        ## Installation & usage
-        
-        Installation of the basic framework should be fairly straightforward:
-        
-        ```
-        git clone https://github.com/NeuroML/NeuroMLlite.git
-        cd NeuroMLlite
-        sudo python setup.py install
-        ```
-        
-        Then simple examples can be run:
-        
-        ```
-        cd examples
-        python Example1.py  #  Generates the JSON representation of the network (console & save to file)
-        ```
-        
-        To generate the NeuroML 2 version of the network, first install pyNeuroML, then use the -nml flag:
-        ```
-        sudo pip install pyNeuroML
-        python Example2.py -nml       # Saves the network structure to a *net.nml XML file
-        ```
-        
-        Other options (which will require [Neuron](https://neuron.yale.edu/neuron/), [NetPyNE](http://www.netpyne.org/), 
-        [PyNN](http://neuralensemble.org/PyNN/), [NEST](http://www.nest-simulator.org/), [Brain](http://briansimulator.org/) etc. to be installed) include:
-        
-        ```
-        python Example4.py -jnml       # Generate NeuroML2 & LEMS simulation & run using jNeuroML
-        python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate Neuron code (py/hoc/mod), then run in Neuron
-        python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate NetPyNE code (py/hoc/mod), then run in NetPyNE
-        python Example4.py -netpyne    # Generate network in NetPyNE directly & run simulation
-        python Example4.py -pynnnrn    # Generate network in PyNN, run using simulator Neuron
-        python Example4.py -pynnnest   # Generate network in PyNN, run using simulator NEST
-        python Example4.py -pynnbrian  # Generate network in PyNN, run using simulator Brian
-        ```
-        
-        Graphs of the network structure can be generated at many levels of detail (1-6) and 
-        laid out using [GraphViz](http://graphviz.org/) engines (d - dot (default); c - circo;
-         n - neato; f - fdp). See above images for generated examples.
-        
-            python Example6.py -graph3d
-            python Example6.py -graph2f
-            python Example6.py -graph1n
-        
-        
-        ## Other examples
-        
-        NeuroMLlite is being tested/used in the following repositories on OSB:
-        
-        - [Wilson & Cowan](https://github.com/OpenSourceBrain/WilsonCowan/blob/master/NeuroML2/GenerateNetworkOverview.py)
-        - [Mejias et al. 2016](https://github.com/OpenSourceBrain/MejiasEtAl2016/blob/master/NeuroML2/GenerateNeuroMLlite.py)
-        - [Pospischil et al. 2008](https://github.com/OpenSourceBrain/PospischilEtAl2008/tree/master/NeuroML2/cells/summary)
-        - [Bezaire et al. 2016](https://github.com/mbezaire/ca1/tree/development/NeuroML2/network/nmllite)
-        - [PING networks](https://github.com/OpenSourceBrain/PINGnets/tree/master/NeuroML2) 
-        - [PsyNeuLink tests](https://github.com/OpenSourceBrain/PsyNeuLinkShowcase/tree/master/NeuroML2)
-        - [OpenWorm - c302](https://github.com/openworm/c302/tree/master/examples/parametersweep)
-        
-        See also:
-        - [ModECI MDF](https://github.com/ModECI/MDF)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE.lesser
+
+## NeuroMLlite: a common framework for reading/writing/generating network specifications based on NeuroML
+
+[![Continuous builds](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
+[![GitHub](https://img.shields.io/github/license/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/blob/master/LICENSE.lesser)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/issues)
+[![GitHub Org's stars](https://img.shields.io/github/stars/NeuroML?style=social)](https://github.com/NeuroML)
+[![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
+
+
+NeuroMLlite is in active development. This will evolve into a framework for more portable, concise network specifications which will form an important part of [NeuroML v3](https://docs.neuroml.org/NeuroMLOrg/History.html#the-future).
+
+For some more background to this package see here: https://github.com/NeuroML/NetworkShorthand.
+
+![Architecture](images/NetworkShorthand.png)
+
+
+## Examples
+The best way to see the currently proposed structure is to look at the examples
+
+### Ex. 1: Simple network, 2 populations & projection
+![Ex1](examples/images/Ex1.png)
+
+[JSON](examples/Example1_TestNetwork.json) | [Python script](examples/Example1.py)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+### Ex. 2: Simple network, 2 populations, projection & inputs
+![Ex2](examples/images/Ex2.png)
+
+[JSON](examples/Example2_TestNetwork.json) | [Python script](examples/Example2.py) | [Generated NeuroML2](examples/Example2_TestNetwork.net.nml)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+### Ex. 3: As above, with simulation specification
+
+[JSON for network](examples/Example3_Network.json) | [JSON for simulation](examples/SimExample3.json) | [Python script](examples/Example3.py) | [Generated NeuroML2](examples/Example3_Network.net.nml) | [Generated LEMS](examples/LEMS_SimExample3.xml)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see Ex2) 
+
+Can be simulated using:
+- **NetPyNE**
+- **jNeuroML**
+- **NEURON** generated from **jNeuroML**
+- **NetPyNE** generated from **jNeuroML**
+
+
+### Ex. 4: A network with PyNN cells & inputs
+<img alt="Ex4" src="examples/images/Ex4.png" height="250"/>
+
+[JSON](examples/Example4_PyNN.json) | [Python script](examples/Example4.py) | [Generated NeuroML2](examples/Example4_PyNN.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+Can be simulated using:
+- **NEST** via **PyNN**
+- **NEURON** via **PyNN**
+- **Brian** via **PyNN**
+- **jNeuroML**
+- **NEURON** generated from **jNeuroML**
+- **NetPyNE** generated from **jNeuroML**
+
+
+### Ex. 5: A network with the Blue Brain Project connectivity data
+<img alt="Ex5" src="examples/images/Ex5_BBP_5percent.png" height="150"/> 
+
+<img alt="Ex5_1" src="examples/images/bbp1.png" height="200"/>  <img alt="Ex5_2" src="examples/images/bbp2.png" height="200"/> <img alt="Ex5_3" src="examples/images/bbp3.png" height="200"/> 
+
+[JSON](examples/BBP_5percent.json) | [Python script](examples/Example5.py) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+- **Matrix** (see above) 
+
+Can be simulated using:
+- **NetPyNE**
+
+### Ex. 6: A network based on Potjans and Diesmann 2014 (work in progress)
+<img alt="Ex6d" src="examples/images/Ex6.dot.png" height="100"/> <img alt="Ex6f" src="examples/images/Ex6.fdp.png" height="100"/>  <img alt="Ex6c" src="examples/images/Ex6.circo.png" height="100"/> 
+<img alt="Ex6matrix" src="examples/images/Ex6matrix.png" height="300"/> 
+
+[JSON](examples/Example6_PyNN.json) | [Python script](examples/Example6.py) | [Generated NeuroML2](examples/Example6_PyNN.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+- **Matrix** (see above) 
+
+### Ex. 7: A network based on Brunel 2000 (work in progress)
+<img alt="Ex7" src="examples/images/Ex7.png" height="250"/> 
+
+[JSON](examples/Example7_Brunel2000.json) | [Python script](examples/Example7.py) | [Generated NeuroML2](examples/Example7_Brunel2000.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+Can be simulated using:
+- **jNeuroML**
+
+## Installation & usage
+
+Installation of the basic framework should be fairly straightforward:
+
+```
+git clone https://github.com/NeuroML/NeuroMLlite.git
+cd NeuroMLlite
+sudo python setup.py install
+```
+
+Then simple examples can be run:
+
+```
+cd examples
+python Example1.py  #  Generates the JSON representation of the network (console & save to file)
+```
+
+To generate the NeuroML 2 version of the network, first install pyNeuroML, then use the -nml flag:
+```
+sudo pip install pyNeuroML
+python Example2.py -nml       # Saves the network structure to a *net.nml XML file
+```
+
+Other options (which will require [Neuron](https://neuron.yale.edu/neuron/), [NetPyNE](http://www.netpyne.org/), 
+[PyNN](http://neuralensemble.org/PyNN/), [NEST](http://www.nest-simulator.org/), [Brain](http://briansimulator.org/) etc. to be installed) include:
+
+```
+python Example4.py -jnml       # Generate NeuroML2 & LEMS simulation & run using jNeuroML
+python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate Neuron code (py/hoc/mod), then run in Neuron
+python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate NetPyNE code (py/hoc/mod), then run in NetPyNE
+python Example4.py -netpyne    # Generate network in NetPyNE directly & run simulation
+python Example4.py -pynnnrn    # Generate network in PyNN, run using simulator Neuron
+python Example4.py -pynnnest   # Generate network in PyNN, run using simulator NEST
+python Example4.py -pynnbrian  # Generate network in PyNN, run using simulator Brian
+```
+
+Graphs of the network structure can be generated at many levels of detail (1-6) and 
+laid out using [GraphViz](http://graphviz.org/) engines (d - dot (default); c - circo;
+ n - neato; f - fdp). See above images for generated examples.
+
+    python Example6.py -graph3d
+    python Example6.py -graph2f
+    python Example6.py -graph1n
+
+
+## Other examples
+
+NeuroMLlite is being tested/used in the following repositories on OSB:
+
+- [Wilson & Cowan](https://github.com/OpenSourceBrain/WilsonCowan/blob/master/NeuroML2/GenerateNetworkOverview.py)
+- [Mejias et al. 2016](https://github.com/OpenSourceBrain/MejiasEtAl2016/blob/master/NeuroML2/GenerateNeuroMLlite.py)
+- [Pospischil et al. 2008](https://github.com/OpenSourceBrain/PospischilEtAl2008/tree/master/NeuroML2/cells/summary)
+- [Bezaire et al. 2016](https://github.com/mbezaire/ca1/tree/development/NeuroML2/network/nmllite)
+- [PING networks](https://github.com/OpenSourceBrain/PINGnets/tree/master/NeuroML2) 
+- [PsyNeuLink tests](https://github.com/OpenSourceBrain/PsyNeuLinkShowcase/tree/master/NeuroML2)
+- [OpenWorm - c302](https://github.com/openworm/c302/tree/master/examples/parametersweep)
+
+See also:
+- [ModECI MDF](https://github.com/ModECI/MDF)
+
+
```

### Comparing `neuromllite-0.5.3/README.md` & `neuromllite-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/ArborHandler.py` & `neuromllite-0.5.4/neuromllite/ArborHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/BBPConnectomeReader.py` & `neuromllite-0.5.4/neuromllite/BBPConnectomeReader.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/BindsNETHandler.py` & `neuromllite-0.5.4/neuromllite/BindsNETHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/ConnectivityHandler.py` & `neuromllite-0.5.4/neuromllite/ConnectivityHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/DefaultNetworkHandler.py` & `neuromllite-0.5.4/neuromllite/DefaultNetworkHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/GraphVizHandler.py` & `neuromllite-0.5.4/neuromllite/GraphVizHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/MDFHandler.py` & `neuromllite-0.5.4/neuromllite/MDFHandler.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 #
 #   A class to write to the MDF format (https://github.com/ModECI/MDF)...
 #
 #
 
 from neuromllite.DefaultNetworkHandler import DefaultNetworkHandler
 from neuromllite.utils import print_v
+from neuromllite.NetworkGenerator import _extract_pynn_components_to_neuroml
+
 from modelspec.utils import save_to_json_file
 from modelspec.utils import save_to_yaml_file
 from modelspec.utils import locate_file
 from modelspec.utils import evaluate
 from pyneuroml.pynml import get_value_in_si
 
 import lems.api as lems  # from pylems
 
+import numpy
+
 
 class MDFHandler(DefaultNetworkHandler):
+
     def __init__(self, nl_network):
         print_v("Initiating MDF handler")
         self.nl_network = nl_network
 
         self.input_list_vs_comps = {}
         self.input_list_vs_pops = {}
 
     def handle_document_start(self, id, notes):
 
-        print_v("Parsing for PsyNeuLink export: %s" % id)
+        print_v("Parsing for MDF export: %s" % id)
         self.id = id
 
         self.mdf_info = {}
 
         # from modeci_mdf import MODECI_MDF_VERSION
-        MODECI_MDF_VERSION = "0.3"
+        MODECI_MDF_VERSION = "0.4"
 
         self.mdf_info[self.id] = {}
         self.mdf_info[self.id]["format"] = "ModECI MDF v%s" % MODECI_MDF_VERSION
         self.mdf_info[self.id]["graphs"] = {}
 
         self.pnl_additions = False
 
@@ -82,37 +87,27 @@
         if size >= 0:
             sizeInfo = ", size: " + str(size) + " cells"
         if component_obj:
             compInfo = " (%s)" % component_obj.__class__.__name__
         else:
             compInfo = ""
 
-        print_v(
-            "Population: "
-            + population_id
-            + ", component: "
-            + component
-            + compInfo
-            + sizeInfo
-            + ", properties: %s"% properties
-        )
+        info = "Population: " + population_id + ", component: " + component + compInfo + sizeInfo + ", properties: %s"% properties
 
-        if size >= 0:
-            for i in range(size):
-                node_id = "%s_%i" % (population_id, i)
+        node_id = "%s" % (population_id)
 
-                cell_comp = self.nl_network.get_child(component, "cells")
+        cell_comp = self.nl_network.get_child(component, "cells")
 
-                if cell_comp is not None:
-                    node = self._comp_to_mdf_node(cell_comp, component, node_id, properties)
+        if cell_comp is not None:
+            node = self._comp_to_mdf_node(cell_comp, component, node_id, size, properties)
 
-                self.mdf_graph["nodes"][node_id] = node
+        self.mdf_graph["nodes"][node_id] = node
 
 
-    def _comp_to_mdf_node(self, nmllite_comp, lems_comp_id, node, properties=None):
+    def _comp_to_mdf_node(self, nmllite_comp, lems_comp_id, node, pop_size, properties=None):
 
        base_dir = "./"  # for now...
 
        node = {}
        if properties:
            node["metadata"] = properties
 
@@ -122,149 +117,299 @@
 
        if nmllite_comp.lems_source_file:
            print_v("  It's defined in custom lems..." )
            fname = locate_file(nmllite_comp.lems_source_file, base_dir)
            model = MDFHandler._load_lems_file_with_neuroml2_types(fname)
            lems_comp = model.components.get(lems_comp_id)
 
-       elif hasattr(nmllite_comp,'neuroml2_cell'):
-           print_v("  It's a cell..." )
+       elif hasattr(nmllite_comp,'neuroml2_cell') and nmllite_comp.neuroml2_cell is not None:
+           print_v("  It is a NeuroML2 cell (%s, %s)..." %(nmllite_comp.id, nmllite_comp.neuroml2_cell))
            model = MDFHandler._get_lems_model_with_neuroml2_types()
            lems_comp = lems.Component(
                id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
            )
-           for p in nmllite_comp.parameters:
-               lems_comp.set_parameter(
-                   p,
-                   evaluate(
-                       nmllite_comp.parameters[p], self.nl_network.parameters
-                   ),
-               )
+           if nmllite_comp.parameters is not None: 
+                for p in nmllite_comp.parameters:
+                    lems_comp.set_parameter(
+                        p,
+                        evaluate(
+                            nmllite_comp.parameters[p], self.nl_network.parameters
+                        ),
+                    )
+       elif nmllite_comp.neuroml2_source_file is not None:
+           print_v("  It is a NeuroML2 cell (%s, %s)..." %(nmllite_comp.id, nmllite_comp.neuroml2_source_file))
+           model = MDFHandler._get_lems_model_with_neuroml2_types()
+           lems_comp = lems.Component(
+               id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_cell
+           )
+           if nmllite_comp.parameters is not None: 
+                for p in nmllite_comp.parameters:
+                    lems_comp.set_parameter(
+                        p,
+                        evaluate(
+                            nmllite_comp.parameters[p], self.nl_network.parameters
+                        ),
+                    )
+
+        
+       elif hasattr(nmllite_comp,'pynn_cell'):
+            print_v("  It's a PyNN cell..." )
+            
+            nml2_doc_temp = _extract_pynn_components_to_neuroml(self.nl_network)
+
+            model = MDFHandler._get_lems_model_with_neuroml2_types(nml2_doc_temp)
+
+            lems_comp = model.components[nmllite_comp.id]
+            
+            for p in nmllite_comp.parameters:
+                lems_comp.set_parameter(
+                    p,
+                    evaluate(
+                        nmllite_comp.parameters[p], self.nl_network.parameters
+                    ),
+                )
 
-       elif hasattr(nmllite_comp,'neuroml2_input'):
-           print_v("  It's an input..." )
+       elif hasattr(nmllite_comp,'neuroml2_input') and nmllite_comp.neuroml2_input is not None:
+           print_v("  It's a NeuroML input..." )
            model = MDFHandler._get_lems_model_with_neuroml2_types()
            lems_comp = lems.Component(
                id_=nmllite_comp.id, type_=nmllite_comp.neuroml2_input
            )
            for p in nmllite_comp.parameters:
                lems_comp.set_parameter(
                    p,
                    evaluate(
                        nmllite_comp.parameters[p], self.nl_network.parameters
                    ),
                )
 
-       print_v("All LEMS comps in model: %s" % model.components.keys())
+       elif hasattr(nmllite_comp,'pynn_input'):
+            print_v("  It's a PyNN input: %s - %s..."%(nmllite_comp.id, nmllite_comp.pynn_input) )
+            
+            nml2_doc_temp = _extract_pynn_components_to_neuroml(self.nl_network)
+
+            model = MDFHandler._get_lems_model_with_neuroml2_types(nml2_doc_temp)
+
+            lems_comp = model.components[nmllite_comp.id]
+            '''
+            for p in nmllite_comp.parameters:
+                lems_comp.set_parameter(
+                    p,
+                    evaluate(
+                        nmllite_comp.parameters[p], self.nl_network.parameters
+                    ),
+                )'''
+
+       print_v("All LEMS comps in model: %s" % list(model.components.keys()))
        print_v("This comp: %s" % lems_comp)
        comp_type_name = lems_comp.type
        lems_comp_type = model.component_types.get(comp_type_name)
        print_v("lems_comp_type: %s" % lems_comp_type)
        notes = "Cell: [%s] is defined in %s and in Lems is: %s" % (
            nmllite_comp,
            nmllite_comp.lems_source_file,
            lems_comp,
        )
 
        node["notes"] = notes
 
        for p in lems_comp.parameters:
            node["parameters"][p] = {
-               "value": get_value_in_si(evaluate(lems_comp.parameters[p]))
+               "value": [get_value_in_si(evaluate(lems_comp.parameters[p]))]*pop_size
            }
 
-       for c in lems_comp_type.constants:
-           node["parameters"][c.name] = {"value": get_value_in_si(c.value)}
-
-       for sv in lems_comp_type.dynamics.state_variables:
-           node["parameters"][sv.name] = {}
-           if sv.exposure:
-               node["output_ports"][sv.exposure] = {"value": sv.name}
-
-       for dv in lems_comp_type.dynamics.derived_variables:
-
-           print_v(
-               "Converting: %s (exp: %s) = [%s] or [%s]"
-               % (dv.name, dv.exposure, dv.value, dv.select)
-           )
-           if dv.name == "INPUT":
-               node["input_ports"][dv.name] = {}
-           else:
-               if dv.value is not None:
-                   node["parameters"][dv.name] = {
-                       "value": self._convert_value(dv.value)
-                   }
-                   if dv.exposure:
-                       node["output_ports"][dv.exposure] = {
-                           "value": dv.name
-                       }
-               if dv.select is not None:
-                   in_port = dv.select.replace("[*]/", "_")
-                   node["input_ports"][in_port] = {}
-                   node["parameters"][dv.name] = {"value": in_port}
-
-       conditions = 0
-       for eh in lems_comp_type.dynamics.event_handlers:
-
-           print_v("Converting: %s (type: %s)" % (eh, type(eh)))
-           if type(eh) == lems.OnStart:
-               for a in eh.actions:
-                   if type(a) == lems.StateAssignment:
-                       node["parameters"][a.variable][
-                           "default_initial_value"
-                       ] = a.value
-           if type(eh) == lems.OnCondition:
-               test = (
-                   eh.test.replace(".gt.", ">")
-                   .replace(".geq.", ">=")
-                   .replace(".lt.", "<")
-                   .replace(".leq.", "<=")
-                   .replace(".eq.", "==")
-                   .replace(".and.", "and")
-               )
-               for a in eh.actions:
-                   if type(a) == lems.StateAssignment:
-                       if (
-                           not "conditions"
-                           in node["parameters"][a.variable]
-                       ):
-                           node["parameters"][a.variable][
-                               "conditions"
-                           ] = {}
-
-                       node["parameters"][a.variable]["conditions"][
-                           "condition_%i" % conditions
-                       ] = {"test": test, "value": a.value}
-               conditions += 1
-
-       for td in lems_comp_type.dynamics.time_derivatives:
-           node["parameters"][td.variable][
-               "time_derivative"
-           ] = self._convert_value(td.value)
+       consts = self._get_all_elements_in_lems(lems_comp_type, model, 'constants')
+       for c in consts:
+            node["parameters"][c.name] = {"value": [get_value_in_si(c.value)]*pop_size}
+
+
+       if hasattr(lems_comp_type,'dynamics'): 
+            
+            for sv in lems_comp_type.dynamics.state_variables:
+                node["parameters"][sv.name] = {}
+
+            for reg in lems_comp_type.dynamics.regimes:
+
+                node['parameters']['ACTIVE_REGIME']={'value': [1]*pop_size}
+                node['parameters']['INACTIVE_REGIME']={'value': [0]*pop_size}
+
+                reg_param = "REGIME_%s"%reg.name
+                #node["parameters"][reg_param] = {"value": 'ACTIVE_REGIME' if reg.initial else 'INACTIVE_REGIME'}
+                
+                if not reg_param in node["parameters"]:
+                    node["parameters"][reg_param] = {}
+                node["parameters"][reg_param]["value"] = reg_param
+                node["parameters"][reg_param]["default_initial_value"] = 'ACTIVE_REGIME' if reg.initial else 'INACTIVE_REGIME'
+
+                node["output_ports"][reg_param] = {"value": reg_param}
+
+                for td in reg.time_derivatives:
+                    node["parameters"][td.variable][
+                        "time_derivative"
+                    ] = self._convert_value("%s * (%s)"%(reg_param,td.value))
+
+                for eh in reg.event_handlers:
+
+                    print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+
+                    if type(eh) == lems.OnCondition:
+                                        
+                        # TODO: remove when global t available
+                        node['parameters']['t']={'default_initial_value': 0, 'time_derivative': '1'}
+
+                        test = "(%s == ACTIVE_REGIME) * (%s)" % (reg_param, self._replace_in_condition_test(eh.test))
+                        #test = "%s == ACTIVE_REGIME" % (reg_param)
+                        if (
+                            not "conditions"
+                            in node["parameters"][reg_param]
+                        ):
+                            node["parameters"][reg_param][
+                                "conditions"
+                            ] = {}
+
+                        node["parameters"][reg_param]["conditions"][
+                            "regime_exit_condition"
+                        ] = {"test": test, "value": 'INACTIVE_REGIME'}
+                        
+                        for a in eh.actions:
+                            if type(a) == lems.Transition:
+                                reg_to_id = a.regime
+                                print_v("  Transition: %s -> %s" % (reg_param, reg_to_id))
+                                reg_to_param = "REGIME_%s"%reg_to_id
+                                if not reg_to_param in node["parameters"]:
+                                    node["parameters"][reg_to_param] = {}
+                                reg_to = lems_comp_type.dynamics.regimes[reg_to_id]
+                                if (
+                                    not "conditions"
+                                    in node["parameters"][reg_to_param]
+                                ):
+                                    node["parameters"][reg_to_param][
+                                        "conditions"
+                                    ] = {}
+
+                                node["parameters"][reg_to_param]["conditions"][
+                                    "regime_entry_condition"
+                                ] = {"test": test, "value": 'ACTIVE_REGIME'}
+
+                                for eh in reg_to.event_handlers:
+
+                                    print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+
+                                    if type(eh) == lems.OnEntry:
+                                        for a in eh.actions:
+                                            if type(a) == lems.StateAssignment:
+                                                if (
+                                                    not "conditions"
+                                                    in node["parameters"][a.variable]
+                                                ):
+                                                    node["parameters"][a.variable][
+                                                        "conditions"
+                                                    ] = {}
+
+                                                node["parameters"][a.variable]["conditions"][
+                                                    "entering_regime_%s"%reg_to_id
+                                                ] = {"test": test, "value": a.value}
+
+
+            for sv in lems_comp_type.dynamics.state_variables:
+                #node["parameters"][sv.name]["value"] = [0]*pop_size
+
+                node["output_ports"][sv.name] = {"value": sv.name}
+                if sv.exposure:
+                    node["output_ports"][sv.exposure] = {"value": sv.name}
+            
+
+            for dv in lems_comp_type.dynamics.derived_variables:
+
+                print_v(
+                    "Converting: %s (exp: %s) = [%s] or [%s]"
+                    % (dv.name, dv.exposure, dv.value, dv.select)
+                )
+                if dv.name == "INPUT":
+                    node["input_ports"][dv.name] = {}
+                else:
+                    if dv.value is not None:
+                        node["parameters"][dv.name] = {
+                            "value": self._convert_value(dv.value)
+                        }
+                        if dv.exposure:
+                            node["output_ports"][dv.exposure] = {
+                                "value": dv.name
+                            }
+                    if dv.select is not None:
+                        in_port = dv.select.replace("[*]/", "_")
+                        node["input_ports"][in_port] = {}
+                        node["parameters"][dv.name] = {"value": in_port}
+
+            conditions = 0
+            for eh in lems_comp_type.dynamics.event_handlers:
+
+                print_v("Converting: %s (type: %s)" % (eh, type(eh)))
+
+                if type(eh) == lems.OnStart:
+                    for a in eh.actions:
+                        if type(a) == lems.StateAssignment:
+                            node["parameters"][a.variable][
+                                "default_initial_value"
+                            ] = a.value
+                        if "value" in node["parameters"][a.variable]:
+                            node["parameters"][a.variable].pop("value")
+                if type(eh) == lems.OnCondition:
+                    test = self._replace_in_condition_test(eh.test)
+
+                    for a in eh.actions:
+                        if type(a) == lems.StateAssignment:
+                            if (
+                                not "conditions"
+                                in node["parameters"][a.variable]
+                            ):
+                                node["parameters"][a.variable][
+                                    "conditions"
+                                ] = {}
+
+                            node["parameters"][a.variable]["conditions"][
+                                "condition_%i" % conditions
+                            ] = {"test": test, "value": a.value}
+                    conditions += 1
+
+            for td in lems_comp_type.dynamics.time_derivatives:
+                node["parameters"][td.variable][
+                    "time_derivative"
+                ] = self._convert_value(td.value)
 
        return node
 
+    def _replace_in_condition_test(self, test):
+        return (test.replace(".gt.", ">")
+                    .replace(".geq.", ">=")
+                    .replace(".lt.", "<")
+                    .replace(".leq.", "<=")
+                    .replace(".eq.", "==")
+                    .replace(".and.", "and"))
 
     # TODO: move to pylems!
     @classmethod
-    def _get_all_children_in_lems(cls, component_type, model, child_type):
-        c = []
+    def _get_all_elements_in_lems(cls, component_type, model, child_type):
+        ee = []
         if child_type == "exposure":
             for e in component_type.exposures:
-                c.append(e)
+                ee.append(e)
+        if child_type == "constants":
+            for c in component_type.constants:
+                ee.append(c)
 
         if component_type.extends:
             ect = model.component_types[component_type.extends]
-            c.extend(cls._get_all_children_in_lems(ect, model, child_type))
+            ee.extend(cls._get_all_elements_in_lems(ect, model, child_type))
 
-        return c
+        return ee
 
     # TODO: move to pyneuroml!
     @classmethod
-    def _get_lems_model_with_neuroml2_types(cls):
+    def _get_lems_model_with_neuroml2_types(cls, nml_doc=None):
 
         from pyneuroml.pynml import get_path_to_jnml_jar
         from pyneuroml.pynml import read_lems_file
         from lems.parser.LEMS import LEMSFileParser
         import zipfile
 
         lems_model = lems.Model(include_includes=False)
@@ -286,14 +431,30 @@
         new_lems = jar.read("NeuroML2CoreTypes/Synapses.xml")
         parser.parse(new_lems)
         new_lems = jar.read("NeuroML2CoreTypes/PyNN.xml")
         parser.parse(new_lems)
         new_lems = jar.read("NeuroML2CoreTypes/Inputs.xml")
         parser.parse(new_lems)
 
+        if nml_doc is not None:
+
+            import io
+            sf = io.StringIO()
+
+            from neuroml.writers import NeuroMLWriter
+
+            
+            print("Adding nml elements from this doc to new lems model: %s"%nml_doc.summary())
+
+            NeuroMLWriter.write(nml_doc, sf, close=False)
+            sf.seek(0)
+            parser.parse(sf.read())
+
+
+
         return lems_model
 
     # TODO: move to pyneuroml!
     @classmethod
     def _load_lems_file_with_neuroml2_types(cls, lems_filename):
 
         from pyneuroml.pynml import read_lems_file
@@ -309,22 +470,69 @@
 
         for cid, c in model.components.items():
             lems_model.components[cid] = c
         for ctid, ct in model.component_types.items():
             lems_model.component_types[ctid] = ct
 
         return lems_model
-
+    
     def handle_location(self, id, population_id, component, x, y, z):
         pass
 
     def finalise_population(self, population_id):
 
         pass
 
+    def handle_projection(
+        self,
+        projName,
+        prePop,
+        postPop,
+        synapse,
+        hasWeights=False,
+        hasDelays=False,
+        type="projection",
+        synapse_obj=None,
+        pre_synapse_obj=None,
+    ):
+        
+        synInfo = ""
+        if synapse_obj:
+            synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
+
+        if pre_synapse_obj:
+            synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
+
+        print_v(
+            "Projection: "
+            + projName
+            + " ("
+            + type
+            + ") from "
+            + prePop
+            + " to "
+            + postPop
+            + " with syn: "
+            + synapse
+            + synInfo
+        )
+
+        pre_node_id = "%s" % (prePop)
+        post_node_id = "%s" % (postPop)
+        edge_id = "Edge %s to %s" % (pre_node_id, post_node_id)
+        edge = {}
+        edge["name"] = edge_id
+        
+        edge["sender_port"] = "OUTPUT"
+        edge["receiver_port"] = "INPUT"
+        edge["sender"] = pre_node_id
+        edge["receiver"] = post_node_id
+
+        self.mdf_graph["edges"][edge_id] = edge
+
     #
     #  Should be overridden to handle network connection
     #
     def handle_connection(
         self,
         projName,
         id,
@@ -352,35 +560,14 @@
                 postSegId,
                 postFract,
                 weight,
                 delay,
             )
         )
 
-        pre_node_id = "%s_%i" % (prePop, preCellId)
-        post_node_id = "%s_%i" % (postPop, postCellId)
-        edge_id = "Edge %s to %s" % (pre_node_id, post_node_id)
-        edge = {}
-        edge["name"] = edge_id
-        # edge['type'] = {}
-        # edge['type']['NeuroML'] = synapseType
-        # edge['parameters'] = {}
-        # edge['functions'] = {}
-        edge["sender_port"] = "OUTPUT"
-        edge["receiver_port"] = "INPUT"
-        edge["sender"] = pre_node_id
-        edge["receiver"] = post_node_id
-        edge["weight"] = weight
-
-        """edge['type'] =  {
-                        "PNL": "MappingProjection",
-                        "generic": None
-                    }"""
-
-        self.mdf_graph["edges"][edge_id] = edge
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
@@ -400,23 +587,23 @@
             % (inputListId, id, cellId, segId, fract, weight, component)
         )
 
         node_id = "Input_%s_%i" % (inputListId, id)
 
         comp = self.nl_network.get_child(component, "input_sources")
 
-        node = self._comp_to_mdf_node(comp, component, node_id)
+        node = self._comp_to_mdf_node(comp, component, node_id, 1)
 
         # TODO: remove when global t available
         node['parameters']['t']={'default_initial_value': 0, 'time_derivative': '1'}
 
         self.mdf_graph["nodes"][node_id] = node
 
         pre_node_id = node_id
-        post_node_id = "%s_%i" % (self.input_list_vs_pops[inputListId], cellId)
+        post_node_id = "%s" % (self.input_list_vs_pops[inputListId])
         edge_id = "Edge %s to %s" % (pre_node_id, post_node_id)
         edge = {}
         edge["name"] = edge_id
         edge["sender_port"] = "i"
         edge["receiver_port"] = "synapses_i"
         edge["sender"] = pre_node_id
         edge["receiver"] = post_node_id
```

### Comparing `neuromllite-0.5.3/neuromllite/MatrixHandler.py` & `neuromllite-0.5.4/neuromllite/MatrixHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/NetworkGenerator.py` & `neuromllite-0.5.4/neuromllite/NetworkGenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1683,14 +1683,21 @@
             pynn_handler.sim.end()
 
             traces = {}
             events = {}
 
             if not "NeuroML" in simulator:
 
+                # Temp! See https://github.com/NeuralEnsemble/PyNN/pull/762
+                def get_source_id(spiketrain):
+                    if 'source_id' in spiketrain.annotations:
+                        return spiketrain.annotations['source_id']
+                    elif 'channel_id' in spiketrain.annotations: # See https://github.com/NeuralEnsemble/PyNN/pull/762
+                        return spiketrain.annotations['channel_id']
+
                 for pop_id in trace_pop_indices_seg_ids:
                     pynn_pop = pynn_handler.populations[pop_id]
                     indices = trace_pop_indices_seg_ids[pop_id].keys()
 
                     filename = "%s.%s.v.dat" % (simulation.id, pop_id)
                     all_columns = []
 
@@ -1744,16 +1751,16 @@
 
                     data = pynn_pop.get_data("spikes", gather=False)
                     spiketrains = data.segments[0].spiketrains
 
                     ff = open(filename, "w")
 
                     for spiketrain in spiketrains:
-                        source_id = spiketrain.annotations["source_id"]
-                        source_index = spiketrain.annotations["source_index"]
+                        source_id = get_source_id(spiketrain)
+                        source_index = pynn_pop.id_to_index(source_id)
                         if source_index in indices:
                             # print_v("Writing spike data for cell %s[%s] (gid: %i): %i spikes "%(pynn_pop.label,source_index, source_id, len(spiketrain)), self.verbose)
                             ref = "%s/%i/???" % (pynn_pop.label, source_index)
                             events[ref] = [t.magnitude / 1000.0 for t in spiketrain]
                             for t in spiketrain:
                                 # ff.write('%s\t%i\n'%(t.magnitude/1000.,source_index))
                                 ff.write(
```

### Comparing `neuromllite-0.5.3/neuromllite/NeuronHandler.py` & `neuromllite-0.5.4/neuromllite/NeuronHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/PsyNeuLinkHandler.py` & `neuromllite-0.5.4/neuromllite/PsyNeuLinkHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/PsyNeuLinkReader.py` & `neuromllite-0.5.4/neuromllite/PsyNeuLinkReader.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/PyNNHandler.py` & `neuromllite-0.5.4/neuromllite/PyNNHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/SonataHandler.py` & `neuromllite-0.5.4/neuromllite/SonataHandler.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/SonataReader.py` & `neuromllite-0.5.4/neuromllite/SonataReader.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/__init__.py` & `neuromllite-0.5.4/neuromllite/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 # import pyNN
 # import nest
 
 from typing import List, Dict, Any, Optional, Union, Tuple, Callable, TypeVar, Type
 
 import modelspec
```

### Comparing `neuromllite-0.5.3/neuromllite/gui/NMLliteUI.py` & `neuromllite-0.5.4/neuromllite/gui/NMLliteUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from os.path import dirname
 from os.path import realpath
 import sys
 
-from PyQt5.QtGui import *
-from PyQt5.QtWidgets import *
+from PyQt6.QtGui import *
+from PyQt6.QtWidgets import *
 
 from matplotlib.backends.backend_qt5agg import FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
 import matplotlib
 from matplotlib.figure import Figure
 
 from neuromllite.utils import load_network_json
 from neuromllite.utils import load_simulation_json
 from neuromllite.utils import evaluate
 from neuromllite.utils import print_v, print_
 from neuromllite.utils import is_spiking_input_population
-from pyneuroml.pynml import get_next_hex_color
+from pyneuroml.utils.plot import get_next_hex_color
 
 from functools import partial
 
 
 class ParameterSpinBox(QDoubleSpinBox):
 
     value_type=float
@@ -166,21 +166,21 @@
                 if toolbar:
                     topLayout.addWidget(thisToolbar)
 
         if image:
             label = QLabel(
                 "An image will be generated here. Push the appropriate button on the left"
             )
-            label.setBackgroundRole(QPalette.Base)
-            label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Ignored)
+            #label.setBackgroundRole(QPalette.Base)
+            #label.setSizePolicy(QSizePolicy.Ignored, QSizePolicy.Ignored)
             label.setScaledContents(True)
             self.all_image_qlabels[name] = label
 
             scrollArea = QScrollArea()
-            scrollArea.setBackgroundRole(QPalette.Light)
+            #scrollArea.setBackgroundRole(QPalette.Light)
             scrollArea.setWidget(label)
             scrollArea.setVisible(True)
 
             scroolLayout = QGridLayout()
             topLayout.addLayout(scroolLayout, 1, 0)
             scroolLayout.addWidget(scrollArea, 0, 0)
 
@@ -265,18 +265,18 @@
             % (name, value, entry, entry.text()),
             self.verbose,
         )
         return entry
 
     def dialog_popup(self, message):
         dialog = QMessageBox()
-        dialog.setIcon(QMessageBox.Warning)
+        dialog.setIcon(QMessageBox.Icon.Warning)
         dialog.setWindowTitle("Message")
         dialog.setText(message)
-        dialog.exec_()
+        dialog.exec()
 
     def __init__(self, nml_sim_file, parent=None):
         """Constructor for the GUI"""
 
         super(NMLliteUI, self).__init__(parent)
 
         self.SPIKES_RASTERPLOT = "Rasterplot"
@@ -749,15 +749,15 @@
         run_jneuroml("", nml_file_name, post_args, verbose=True)
 
         nml_view_file = nml_file_name.replace(".nml", ".png")
 
         self.add_image(nml_view_file, self.IMAGE_3D_TAB)
 
     def showGraph(self):
-        """Generate graph buttom has been pressed"""
+        """Generate graph button has been pressed"""
 
         print_v("Graph button was clicked.")
 
         self.update_net_sim()
         self.tabs.setCurrentWidget(self.all_tabs[self.GRAPH_TAB])
 
         from neuromllite.GraphVizHandler import GraphVizHandler
@@ -802,15 +802,19 @@
 
             self.add_image(genFile, self.GRAPH_TAB)
 
     def update_net_sim(self):
         """Set the parameters in the network/simulation from the GUI values"""
 
         for p in self.param_entries:
-            v = self.param_entries[p].final_value()
+            #print("Updating: %s to %s (%s)" % (p, self.param_entries[p], type(self.param_entries[p])))
+            if type(self.param_entries[p])==QLineEdit:
+                v = self.param_entries[p].text()
+            else:
+                v = self.param_entries[p].final_value()
 
             print_("Setting param %s to %s" % (p, v), self.verbose)
             if p == "seed":
                 self.network.seed = v
             elif p == "temperature":
                 self.network.temperature = v
             else:
@@ -888,15 +892,15 @@
             "traceSelect button was clicked. Traces shown: %s; colours: %s"
             % (self.current_traces_shown, self.current_traces_colours)
         )
 
         dialog = QDialog(self)
         dialog.setWindowTitle("Select which traces to plot")
 
-        QBtn = QDialogButtonBox.Ok  # | QDialogButtonBox.Cancel
+        QBtn = QDialogButtonBox.StandardButton.Ok  # | QDialogButtonBox.Cancel
 
         buttonBox = QDialogButtonBox(QBtn)
         buttonBox.accepted.connect(dialog.accept)
 
         layout = QGridLayout()
         dialog.setLayout(layout)
 
@@ -918,15 +922,15 @@
                 color_button.setStyleSheet(style)
 
                 layout.addWidget(color_button, count, 0)
                 layout.addWidget(self.all_cbs[key], count, 1)
                 count += 1
 
         layout.addWidget(buttonBox, count, 1)
-        dialog.exec_()
+        dialog.exec()
         self.replotSimResults()
 
     def traceSelectClicked(self, key):
 
         cb = self.all_cbs[key]
         # print('Clicked: %s, %s, key: %s'%(cb.text(),cb.isChecked(), key))
         self.current_traces_shown[key] = cb.isChecked()
@@ -1321,15 +1325,15 @@
 
     app = QApplication(sys.argv)
     nml_sim_file = sys.argv[1]
 
     nmlui = NMLliteUI(nml_sim_file)
     nmlui.show()
 
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
 
 
 def usage():
 
     from neuromllite import __version__ as version
 
     MAIN_CLA = "nmllite-ui"
```

### Comparing `neuromllite-0.5.3/neuromllite/sweep/GenerateTests.py` & `neuromllite-0.5.4/neuromllite/sweep/GenerateTests.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/sweep/ParameterSweep.py` & `neuromllite-0.5.4/neuromllite/sweep/ParameterSweep.py`

 * *Files identical despite different names*

### Comparing `neuromllite-0.5.3/neuromllite/utils.py` & `neuromllite-0.5.4/neuromllite/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     net.temperature = temperature  # degC
     if parameters:
         net.parameters = parameters
 
     ################################################################################
     ###   Add some regions
 
-    if default_region:
+    if default_region is not None:
         if type(default_region) == str:
             r1 = RectangularRegion(
                 id=default_region, x=0, y=0, z=0, width=1000, height=100, depth=1000
             )
             net.regions.append(r1)
             default_region = r1
         else:
@@ -237,17 +237,15 @@
         pop = Population(
             id="pop_%s" % cell_for_default_population.id,
             size=1,
             component=cell_for_default_population.id,
             properties={"color": color_for_default_population},
         )
 
-        if default_region:
-            pop.region = default_region
-
+        if default_region is not None:
             pop.random_layout = RandomLayout(region=default_region.id)
 
         net.populations.append(pop)
 
     ################################################################################
     ###   Add a projection
```

### Comparing `neuromllite-0.5.3/neuromllite.egg-info/PKG-INFO` & `neuromllite-0.5.4/neuromllite.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,193 +1,193 @@
 Metadata-Version: 2.1
 Name: neuromllite
-Version: 0.5.3
+Version: 0.5.4
 Summary: A common JSON/YAML based format for compact network specification, closely tied to NeuroML v2
 Home-page: https://github.com/NeuroML/NeuroMLlite
 Author: Padraig Gleeson
 Author-email: p.gleeson@gmail.com
 License: LICENSE.lesser
-Description: ## NeuroMLlite: a common framework for reading/writing/generating network specifications based on NeuroML
-        
-        [![Continuous builds](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml)
-        [![PyPI](https://img.shields.io/pypi/v/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
-        [![GitHub](https://img.shields.io/github/license/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/blob/master/LICENSE.lesser)
-        [![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/pulls)
-        [![GitHub issues](https://img.shields.io/github/issues/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/issues)
-        [![GitHub Org's stars](https://img.shields.io/github/stars/NeuroML?style=social)](https://github.com/NeuroML)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
-        
-        
-        NeuroMLlite is in active development. This will evolve into a framework for more portable, concise network specifications which will form an important part of [NeuroML v3](https://docs.neuroml.org/NeuroMLOrg/History.html#the-future).
-        
-        For some more background to this package see here: https://github.com/NeuroML/NetworkShorthand.
-        
-        ![Architecture](images/NetworkShorthand.png)
-        
-        
-        ## Examples
-        The best way to see the currently proposed structure is to look at the examples
-        
-        ### Ex. 1: Simple network, 2 populations & projection
-        ![Ex1](examples/images/Ex1.png)
-        
-        [JSON](examples/Example1_TestNetwork.json) | [Python script](examples/Example1.py)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        ### Ex. 2: Simple network, 2 populations, projection & inputs
-        ![Ex2](examples/images/Ex2.png)
-        
-        [JSON](examples/Example2_TestNetwork.json) | [Python script](examples/Example2.py) | [Generated NeuroML2](examples/Example2_TestNetwork.net.nml)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        ### Ex. 3: As above, with simulation specification
-        
-        [JSON for network](examples/Example3_Network.json) | [JSON for simulation](examples/SimExample3.json) | [Python script](examples/Example3.py) | [Generated NeuroML2](examples/Example3_Network.net.nml) | [Generated LEMS](examples/LEMS_SimExample3.xml)
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see Ex2) 
-        
-        Can be simulated using:
-        - **NetPyNE**
-        - **jNeuroML**
-        - **NEURON** generated from **jNeuroML**
-        - **NetPyNE** generated from **jNeuroML**
-        
-        
-        ### Ex. 4: A network with PyNN cells & inputs
-        <img alt="Ex4" src="examples/images/Ex4.png" height="250"/>
-        
-        [JSON](examples/Example4_PyNN.json) | [Python script](examples/Example4.py) | [Generated NeuroML2](examples/Example4_PyNN.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        Can be simulated using:
-        - **NEST** via **PyNN**
-        - **NEURON** via **PyNN**
-        - **Brian** via **PyNN**
-        - **jNeuroML**
-        - **NEURON** generated from **jNeuroML**
-        - **NetPyNE** generated from **jNeuroML**
-        
-        
-        ### Ex. 5: A network with the Blue Brain Project connectivity data
-        <img alt="Ex5" src="examples/images/Ex5_BBP_5percent.png" height="150"/> 
-        
-        <img alt="Ex5_1" src="examples/images/bbp1.png" height="200"/>  <img alt="Ex5_2" src="examples/images/bbp2.png" height="200"/> <img alt="Ex5_3" src="examples/images/bbp3.png" height="200"/> 
-        
-        [JSON](examples/BBP_5percent.json) | [Python script](examples/Example5.py) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        - **Matrix** (see above) 
-        
-        Can be simulated using:
-        - **NetPyNE**
-        
-        ### Ex. 6: A network based on Potjans and Diesmann 2014 (work in progress)
-        <img alt="Ex6d" src="examples/images/Ex6.dot.png" height="100"/> <img alt="Ex6f" src="examples/images/Ex6.fdp.png" height="100"/>  <img alt="Ex6c" src="examples/images/Ex6.circo.png" height="100"/> 
-        <img alt="Ex6matrix" src="examples/images/Ex6matrix.png" height="300"/> 
-        
-        [JSON](examples/Example6_PyNN.json) | [Python script](examples/Example6.py) | [Generated NeuroML2](examples/Example6_PyNN.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        - **Matrix** (see above) 
-        
-        ### Ex. 7: A network based on Brunel 2000 (work in progress)
-        <img alt="Ex7" src="examples/images/Ex7.png" height="250"/> 
-        
-        [JSON](examples/Example7_Brunel2000.json) | [Python script](examples/Example7.py) | [Generated NeuroML2](examples/Example7_Brunel2000.net.nml) 
-        
-        Can be exported to:
-        - **NeuroML 2** (XML or HDF5 format)
-        - **Graph** (see above) 
-        
-        Can be simulated using:
-        - **jNeuroML**
-        
-        ## Installation & usage
-        
-        Installation of the basic framework should be fairly straightforward:
-        
-        ```
-        git clone https://github.com/NeuroML/NeuroMLlite.git
-        cd NeuroMLlite
-        sudo python setup.py install
-        ```
-        
-        Then simple examples can be run:
-        
-        ```
-        cd examples
-        python Example1.py  #  Generates the JSON representation of the network (console & save to file)
-        ```
-        
-        To generate the NeuroML 2 version of the network, first install pyNeuroML, then use the -nml flag:
-        ```
-        sudo pip install pyNeuroML
-        python Example2.py -nml       # Saves the network structure to a *net.nml XML file
-        ```
-        
-        Other options (which will require [Neuron](https://neuron.yale.edu/neuron/), [NetPyNE](http://www.netpyne.org/), 
-        [PyNN](http://neuralensemble.org/PyNN/), [NEST](http://www.nest-simulator.org/), [Brain](http://briansimulator.org/) etc. to be installed) include:
-        
-        ```
-        python Example4.py -jnml       # Generate NeuroML2 & LEMS simulation & run using jNeuroML
-        python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate Neuron code (py/hoc/mod), then run in Neuron
-        python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate NetPyNE code (py/hoc/mod), then run in NetPyNE
-        python Example4.py -netpyne    # Generate network in NetPyNE directly & run simulation
-        python Example4.py -pynnnrn    # Generate network in PyNN, run using simulator Neuron
-        python Example4.py -pynnnest   # Generate network in PyNN, run using simulator NEST
-        python Example4.py -pynnbrian  # Generate network in PyNN, run using simulator Brian
-        ```
-        
-        Graphs of the network structure can be generated at many levels of detail (1-6) and 
-        laid out using [GraphViz](http://graphviz.org/) engines (d - dot (default); c - circo;
-         n - neato; f - fdp). See above images for generated examples.
-        
-            python Example6.py -graph3d
-            python Example6.py -graph2f
-            python Example6.py -graph1n
-        
-        
-        ## Other examples
-        
-        NeuroMLlite is being tested/used in the following repositories on OSB:
-        
-        - [Wilson & Cowan](https://github.com/OpenSourceBrain/WilsonCowan/blob/master/NeuroML2/GenerateNetworkOverview.py)
-        - [Mejias et al. 2016](https://github.com/OpenSourceBrain/MejiasEtAl2016/blob/master/NeuroML2/GenerateNeuroMLlite.py)
-        - [Pospischil et al. 2008](https://github.com/OpenSourceBrain/PospischilEtAl2008/tree/master/NeuroML2/cells/summary)
-        - [Bezaire et al. 2016](https://github.com/mbezaire/ca1/tree/development/NeuroML2/network/nmllite)
-        - [PING networks](https://github.com/OpenSourceBrain/PINGnets/tree/master/NeuroML2) 
-        - [PsyNeuLink tests](https://github.com/OpenSourceBrain/PsyNeuLinkShowcase/tree/master/NeuroML2)
-        - [OpenWorm - c302](https://github.com/openworm/c302/tree/master/examples/parametersweep)
-        
-        See also:
-        - [ModECI MDF](https://github.com/ModECI/MDF)
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
+License-File: LICENSE.lesser
+
+## NeuroMLlite: a common framework for reading/writing/generating network specifications based on NeuroML
+
+[![Continuous builds](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuroML/NeuroMLlite/actions/workflows/ci.yml)
+[![PyPI](https://img.shields.io/pypi/v/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NeuroMLlite)](https://pypi.org/project/NeuroMLlite/)
+[![GitHub](https://img.shields.io/github/license/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/blob/master/LICENSE.lesser)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/NeuroML/NeuroMLlite)](https://github.com/NeuroML/NeuroMLlite/issues)
+[![GitHub Org's stars](https://img.shields.io/github/stars/NeuroML?style=social)](https://github.com/NeuroML)
+[![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
+
+
+NeuroMLlite is in active development. This will evolve into a framework for more portable, concise network specifications which will form an important part of [NeuroML v3](https://docs.neuroml.org/NeuroMLOrg/History.html#the-future).
+
+For some more background to this package see here: https://github.com/NeuroML/NetworkShorthand.
+
+![Architecture](images/NetworkShorthand.png)
+
+
+## Examples
+The best way to see the currently proposed structure is to look at the examples
+
+### Ex. 1: Simple network, 2 populations & projection
+![Ex1](examples/images/Ex1.png)
+
+[JSON](examples/Example1_TestNetwork.json) | [Python script](examples/Example1.py)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+### Ex. 2: Simple network, 2 populations, projection & inputs
+![Ex2](examples/images/Ex2.png)
+
+[JSON](examples/Example2_TestNetwork.json) | [Python script](examples/Example2.py) | [Generated NeuroML2](examples/Example2_TestNetwork.net.nml)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+### Ex. 3: As above, with simulation specification
+
+[JSON for network](examples/Example3_Network.json) | [JSON for simulation](examples/SimExample3.json) | [Python script](examples/Example3.py) | [Generated NeuroML2](examples/Example3_Network.net.nml) | [Generated LEMS](examples/LEMS_SimExample3.xml)
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see Ex2) 
+
+Can be simulated using:
+- **NetPyNE**
+- **jNeuroML**
+- **NEURON** generated from **jNeuroML**
+- **NetPyNE** generated from **jNeuroML**
+
+
+### Ex. 4: A network with PyNN cells & inputs
+<img alt="Ex4" src="examples/images/Ex4.png" height="250"/>
+
+[JSON](examples/Example4_PyNN.json) | [Python script](examples/Example4.py) | [Generated NeuroML2](examples/Example4_PyNN.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+Can be simulated using:
+- **NEST** via **PyNN**
+- **NEURON** via **PyNN**
+- **Brian** via **PyNN**
+- **jNeuroML**
+- **NEURON** generated from **jNeuroML**
+- **NetPyNE** generated from **jNeuroML**
+
+
+### Ex. 5: A network with the Blue Brain Project connectivity data
+<img alt="Ex5" src="examples/images/Ex5_BBP_5percent.png" height="150"/> 
+
+<img alt="Ex5_1" src="examples/images/bbp1.png" height="200"/>  <img alt="Ex5_2" src="examples/images/bbp2.png" height="200"/> <img alt="Ex5_3" src="examples/images/bbp3.png" height="200"/> 
+
+[JSON](examples/BBP_5percent.json) | [Python script](examples/Example5.py) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+- **Matrix** (see above) 
+
+Can be simulated using:
+- **NetPyNE**
+
+### Ex. 6: A network based on Potjans and Diesmann 2014 (work in progress)
+<img alt="Ex6d" src="examples/images/Ex6.dot.png" height="100"/> <img alt="Ex6f" src="examples/images/Ex6.fdp.png" height="100"/>  <img alt="Ex6c" src="examples/images/Ex6.circo.png" height="100"/> 
+<img alt="Ex6matrix" src="examples/images/Ex6matrix.png" height="300"/> 
+
+[JSON](examples/Example6_PyNN.json) | [Python script](examples/Example6.py) | [Generated NeuroML2](examples/Example6_PyNN.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+- **Matrix** (see above) 
+
+### Ex. 7: A network based on Brunel 2000 (work in progress)
+<img alt="Ex7" src="examples/images/Ex7.png" height="250"/> 
+
+[JSON](examples/Example7_Brunel2000.json) | [Python script](examples/Example7.py) | [Generated NeuroML2](examples/Example7_Brunel2000.net.nml) 
+
+Can be exported to:
+- **NeuroML 2** (XML or HDF5 format)
+- **Graph** (see above) 
+
+Can be simulated using:
+- **jNeuroML**
+
+## Installation & usage
+
+Installation of the basic framework should be fairly straightforward:
+
+```
+git clone https://github.com/NeuroML/NeuroMLlite.git
+cd NeuroMLlite
+sudo python setup.py install
+```
+
+Then simple examples can be run:
+
+```
+cd examples
+python Example1.py  #  Generates the JSON representation of the network (console & save to file)
+```
+
+To generate the NeuroML 2 version of the network, first install pyNeuroML, then use the -nml flag:
+```
+sudo pip install pyNeuroML
+python Example2.py -nml       # Saves the network structure to a *net.nml XML file
+```
+
+Other options (which will require [Neuron](https://neuron.yale.edu/neuron/), [NetPyNE](http://www.netpyne.org/), 
+[PyNN](http://neuralensemble.org/PyNN/), [NEST](http://www.nest-simulator.org/), [Brain](http://briansimulator.org/) etc. to be installed) include:
+
+```
+python Example4.py -jnml       # Generate NeuroML2 & LEMS simulation & run using jNeuroML
+python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate Neuron code (py/hoc/mod), then run in Neuron
+python Example4.py -jnmlnrn    # Generate NeuroML2 & LEMS simulation, use jNeuroML to generate NetPyNE code (py/hoc/mod), then run in NetPyNE
+python Example4.py -netpyne    # Generate network in NetPyNE directly & run simulation
+python Example4.py -pynnnrn    # Generate network in PyNN, run using simulator Neuron
+python Example4.py -pynnnest   # Generate network in PyNN, run using simulator NEST
+python Example4.py -pynnbrian  # Generate network in PyNN, run using simulator Brian
+```
+
+Graphs of the network structure can be generated at many levels of detail (1-6) and 
+laid out using [GraphViz](http://graphviz.org/) engines (d - dot (default); c - circo;
+ n - neato; f - fdp). See above images for generated examples.
+
+    python Example6.py -graph3d
+    python Example6.py -graph2f
+    python Example6.py -graph1n
+
+
+## Other examples
+
+NeuroMLlite is being tested/used in the following repositories on OSB:
+
+- [Wilson & Cowan](https://github.com/OpenSourceBrain/WilsonCowan/blob/master/NeuroML2/GenerateNetworkOverview.py)
+- [Mejias et al. 2016](https://github.com/OpenSourceBrain/MejiasEtAl2016/blob/master/NeuroML2/GenerateNeuroMLlite.py)
+- [Pospischil et al. 2008](https://github.com/OpenSourceBrain/PospischilEtAl2008/tree/master/NeuroML2/cells/summary)
+- [Bezaire et al. 2016](https://github.com/mbezaire/ca1/tree/development/NeuroML2/network/nmllite)
+- [PING networks](https://github.com/OpenSourceBrain/PINGnets/tree/master/NeuroML2) 
+- [PsyNeuLink tests](https://github.com/OpenSourceBrain/PsyNeuLinkShowcase/tree/master/NeuroML2)
+- [OpenWorm - c302](https://github.com/openworm/c302/tree/master/examples/parametersweep)
+
+See also:
+- [ModECI MDF](https://github.com/ModECI/MDF)
+
+
```

### Comparing `neuromllite-0.5.3/neuromllite.egg-info/SOURCES.txt` & `neuromllite-0.5.4/neuromllite.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.lesser
 README.md
 setup.py
 neuromllite/ArborHandler.py
 neuromllite/BBPConnectomeReader.py
 neuromllite/BindsNETHandler.py
 neuromllite/ConnectivityHandler.py
 neuromllite/DefaultNetworkHandler.py
```

### Comparing `neuromllite-0.5.3/setup.py` & `neuromllite-0.5.4/setup.py`

 * *Files identical despite different names*

