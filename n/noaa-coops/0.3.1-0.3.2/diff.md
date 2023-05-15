# Comparing `tmp/noaa_coops-0.3.1.tar.gz` & `tmp/noaa_coops-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaa_coops-0.3.1.tar", max compression
+gzip compressed data, was "noaa_coops-0.3.2.tar", max compression
```

## Comparing `noaa_coops-0.3.1.tar` & `noaa_coops-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11345 2023-04-19 16:48:21.778836 noaa_coops-0.3.1/LICENSE
--rw-r--r--   0        0        0     5746 2023-04-19 17:05:24.060617 noaa_coops-0.3.1/README.md
--rw-r--r--   0        0        0      101 2023-04-28 07:40:26.252516 noaa_coops-0.3.1/noaa_coops/__init__.py
--rw-r--r--   0        0        0    31293 2023-04-28 07:40:26.253391 noaa_coops-0.3.1/noaa_coops/station.py
--rw-r--r--   0        0        0     1567 2023-04-28 07:40:26.254125 noaa_coops-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 noaa_coops-0.3.1/setup.py
--rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 noaa_coops-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-04-19 16:48:21.778836 noaa_coops-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5746 2023-04-19 17:05:24.060617 noaa_coops-0.3.2/README.md
+-rw-r--r--   0        0        0      101 2023-05-15 05:16:09.256841 noaa_coops-0.3.2/noaa_coops/__init__.py
+-rw-r--r--   0        0        0    31293 2023-05-15 05:33:46.631831 noaa_coops-0.3.2/noaa_coops/station.py
+-rw-r--r--   0        0        0     1549 2023-05-15 05:15:06.058642 noaa_coops-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6724 1970-01-01 00:00:00.000000 noaa_coops-0.3.2/setup.py
+-rw-r--r--   0        0        0     6610 1970-01-01 00:00:00.000000 noaa_coops-0.3.2/PKG-INFO
```

### Comparing `noaa_coops-0.3.1/LICENSE` & `noaa_coops-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.3.1/README.md` & `noaa_coops-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.3.1/noaa_coops/station.py` & `noaa_coops-0.3.2/noaa_coops/station.py`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.3.1/pyproject.toml` & `noaa_coops-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "noaa-coops"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python wrapper for NOAA Tides & Currents Data and Metadata."
 authors = ["Greg Clunies <greg.clunies@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/GClunies/noaa_coops"
 keywords = ["noaa", "coops", "tides", "currents", "weather", "api"]
 packages = [{include = "noaa_coops"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
-numpy = "^1.24.1"
 pandas = "^1.5.3"
 zeep = "^4.2.1"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.0.1"
 black = "^23.1.0"
 flake8 = {version = "^6", python = "^3.8.1"}
```

### Comparing `noaa_coops-0.3.1/setup.py` & `noaa_coops-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 packages = \
 ['noaa_coops']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.1,<2.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'zeep>=4.2.1,<5.0.0']
+['pandas>=1.5.3,<2.0.0', 'requests>=2.28.2,<3.0.0', 'zeep>=4.2.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'noaa-coops',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Python wrapper for NOAA Tides & Currents Data and Metadata.',
     'long_description': '# noaa_coops\n\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed via [PyPi](https://pypi.org/project/noaa-coops/) and can be installed using , `pip`, `poetry`, etc.\n```bash\n# Install with pip\n❯ pip install noaa_coops\n\n# Install with poetry\n❯ poetry add noaa_coops\n```\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n### Data Retrieval\nAvailable data products can be found in NOAA CO-OPS Data API docs.\n\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.\n\nThe example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The corresponding [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150131",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                         v      s        f  q\nt\n2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v\n\n```\n\n![image](https://user-images.githubusercontent.com/28986302/233147224-765fbe05-372c-40f3-8bbe-4102536e7ff3.png)\n\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
     'author': 'Greg Clunies',
     'author_email': 'greg.clunies@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GClunies/noaa_coops',
```

### Comparing `noaa_coops-0.3.1/PKG-INFO` & `noaa_coops-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: noaa-coops
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python wrapper for NOAA Tides & Currents Data and Metadata.
 Home-page: https://github.com/GClunies/noaa_coops
 License: Apache-2.0
 Keywords: noaa,coops,tides,currents,weather,api
 Author: Greg Clunies
 Author-email: greg.clunies@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: zeep (>=4.2.1,<5.0.0)
 Project-URL: Repository, https://github.com/GClunies/noaa_coops
 Description-Content-Type: text/markdown
 
 # noaa_coops
```

