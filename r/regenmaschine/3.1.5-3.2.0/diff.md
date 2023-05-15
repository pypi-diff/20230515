# Comparing `tmp/regenmaschine-3.1.5.tar.gz` & `tmp/regenmaschine-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regenmaschine-3.1.5.tar", max compression
+gzip compressed data, was "regenmaschine-3.2.0.tar", max compression
```

## Comparing `regenmaschine-3.1.5.tar` & `regenmaschine-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1077 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/LICENSE
--rw-r--r--   0        0        0    11338 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/README.md
--rw-r--r--   0        0        0     2021 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/pyproject.toml
--rw-r--r--   0        0        0       53 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/__init__.py
--rw-r--r--   0        0        0      486 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/api.py
--rw-r--r--   0        0        0     5597 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/client.py
--rw-r--r--   0        0        0     3688 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/controller.py
--rw-r--r--   0        0        0      641 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/diagnostics.py
--rw-r--r--   0        0        0      773 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/errors.py
--rw-r--r--   0        0        0      551 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/parser.py
--rw-r--r--   0        0        0     2017 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/program.py
--rw-r--r--   0        0        0      814 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/provision.py
--rw-r--r--   0        0        0        0 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/py.typed
--rw-r--r--   0        0        0     1099 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/restriction.py
--rw-r--r--   0        0        0      937 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/stats.py
--rw-r--r--   0        0        0     2126 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/watering.py
--rw-r--r--   0        0        0     2513 2021-07-27 03:24:54.486899 regenmaschine-3.1.5/regenmaschine/zone.py
--rw-r--r--   0        0        0    12386 2021-07-27 03:25:03.065557 regenmaschine-3.1.5/setup.py
--rw-r--r--   0        0        0    12235 2021-07-27 03:25:03.066262 regenmaschine-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/LICENSE
+-rw-r--r--   0        0        0    11616 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/README.md
+-rw-r--r--   0        0        0     2021 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0       53 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/__init__.py
+-rw-r--r--   0        0        0      486 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/api.py
+-rw-r--r--   0        0        0     5597 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/client.py
+-rw-r--r--   0        0        0     3688 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/controller.py
+-rw-r--r--   0        0        0      641 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/diagnostics.py
+-rw-r--r--   0        0        0      773 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/errors.py
+-rw-r--r--   0        0        0      938 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/parser.py
+-rw-r--r--   0        0        0     2017 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/program.py
+-rw-r--r--   0        0        0      814 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/provision.py
+-rw-r--r--   0        0        0        0 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/py.typed
+-rw-r--r--   0        0        0     1099 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/restriction.py
+-rw-r--r--   0        0        0      937 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/stats.py
+-rw-r--r--   0        0        0     2126 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/watering.py
+-rw-r--r--   0        0        0     2513 2021-10-04 19:57:04.209931 regenmaschine-3.2.0/regenmaschine/zone.py
+-rw-r--r--   0        0        0    12670 2021-10-04 19:57:19.440081 regenmaschine-3.2.0/setup.py
+-rw-r--r--   0        0        0    12564 2021-10-04 19:57:19.440690 regenmaschine-3.2.0/PKG-INFO
```

### Comparing `regenmaschine-3.1.5/LICENSE` & `regenmaschine-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/README.md` & `regenmaschine-3.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,16 @@
     async with ClientSession() as session:
         client = Client(session=session)
 
 
 asyncio.run(main())
 ```
 
+## Loading Local (Accessible Over the LAN) Controllers
+
 Once you have a client, you can load a local controller (i.e., one that is
 accessible over the LAN) very easily:
 
 ```python
 import asyncio
 
 from aiohttp import ClientSession
@@ -105,14 +107,16 @@
         controllers = client.controllers
         # >>> {'ab:cd:ef:12:34:56': <LocalController>}
 
 
 asyncio.run(main())
 ```
 
+## Loading Remote (Accessible Over the RainMachine Cloud) Controllers
+
 If you have 1, 2 or 100 other local controllers, you can load them in the same
 way – `client.controllers` will keep your controllers all organized.
 
 What if you have controllers around the world and can't access them all over
 the same local network? No problem! `regenmaschine` allows you to load remote
 controllers very easily, as well:
 
@@ -137,14 +141,16 @@
 
 asyncio.run(main())
 ```
 
 Bonus tip: `client.load_remote` will load _all_ controllers owned by that email
 address.
 
+## Using the Controller
+
 Regardless of the type of controller you have loaded (local or remote), the
 same properties and methods are available to each:
 
 ```python
 import asyncio
 import datetime
 
@@ -263,15 +269,15 @@
             await controller.watering.stop_all()
 
 
 asyncio.run(main())
 ```
 
 Check out `example.py`, the tests, and the source files themselves for method
-signatures and more examples.
+signatures and more examples. For additional reference, the full RainMachine™ API documentation is available [here](https://rainmachine.docs.apiary.io/).
 
 # Loading Controllers Multiple Times
 
 It is technically possible to load a controller multiple times. Let's pretend
 for a moment that:
 
 * We have a local controller named `Home` (available at `192.168.1.101`).
```

### Comparing `regenmaschine-3.1.5/pyproject.toml` & `regenmaschine-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.poetry]
 name = "regenmaschine"
-version = "3.1.5"
+version = "3.2.0"
 description = "A simple API for RainMachine sprinkler controllers"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/regenmaschine"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -64,9 +64,9 @@
 
 [tool.poetry.dev-dependencies]
 aresponses = "^2.0.0"
 asynctest = "^0.13.0"
 pre-commit = "^2.0.1"
 pytest = "^6.0.0"
 pytest-aiohttp = "^0.3.0"
-pytest-cov = "^2.8.1"
+pytest-cov = "^3.0.0"
 pytest-mock = "^3.0.0"
```

### Comparing `regenmaschine-3.1.5/regenmaschine/client.py` & `regenmaschine-3.2.0/regenmaschine/client.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/controller.py` & `regenmaschine-3.2.0/regenmaschine/controller.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/diagnostics.py` & `regenmaschine-3.2.0/regenmaschine/diagnostics.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/errors.py` & `regenmaschine-3.2.0/regenmaschine/errors.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/parser.py` & `regenmaschine-3.2.0/regenmaschine/provision.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-"""Define an object to interact with RainMachine weather parsers."""
+"""Define an object to interact with provisioning info."""
 from typing import Any, Awaitable, Callable, Dict, cast
 
 
-class Parser:  # pylint: disable=too-few-public-methods
-    """Define a parser object."""
+class Provision:
+    """Define a provisioning object."""
 
     def __init__(self, request: Callable[..., Awaitable[Dict[str, Any]]]) -> None:
         """Initialize."""
         self._request = request
 
-    async def current(self) -> Dict[str, Any]:
-        """Get current diagnostics."""
-        data = await self._request("get", "parser")
-        return cast(Dict[str, Any], data["parsers"])
+    @property
+    async def device_name(self) -> str:
+        """Get the name of the device."""
+        data = await self._request("get", "provision/name")
+        return cast(str, data["name"])
+
+    async def settings(self) -> Dict[str, Any]:
+        """Get a multitude of settings info."""
+        return await self._request("get", "provision")
+
+    async def wifi(self) -> Dict[str, Any]:
+        """Get wifi info from the device."""
+        return await self._request("get", "provision/wifi")
```

### Comparing `regenmaschine-3.1.5/regenmaschine/program.py` & `regenmaschine-3.2.0/regenmaschine/program.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/restriction.py` & `regenmaschine-3.2.0/regenmaschine/restriction.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/stats.py` & `regenmaschine-3.2.0/regenmaschine/stats.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/watering.py` & `regenmaschine-3.2.0/regenmaschine/watering.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/regenmaschine/zone.py` & `regenmaschine-3.2.0/regenmaschine/zone.py`

 * *Files identical despite different names*

### Comparing `regenmaschine-3.1.5/setup.py` & `regenmaschine-3.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'regenmaschine',
-    'version': '3.1.5',
+    'version': '3.2.0',
     'description': 'A simple API for RainMachine sprinkler controllers',
-    'long_description': '# 💧 Regenmaschine: A Simple Python Library for RainMachine™\n\n[![CI](https://github.com/bachya/regenmaschine/workflows/CI/badge.svg)](https://github.com/bachya/regenmaschine/actions)\n[![PyPi](https://img.shields.io/pypi/v/regenmaschine.svg)](https://pypi.python.org/pypi/regenmaschine)\n[![Version](https://img.shields.io/pypi/pyversions/regenmaschine.svg)](https://pypi.python.org/pypi/regenmaschine)\n[![License](https://img.shields.io/pypi/l/regenmaschine.svg)](https://github.com/bachya/regenmaschine/blob/master/LICENSE)\n[![Code Coverage](https://codecov.io/gh/bachya/regenmaschine/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/regenmaschine)\n[![Maintainability](https://api.codeclimate.com/v1/badges/a99a88d28ad37a79dbf6/maintainability)](https://codeclimate.com/github/bachya/regenmaschine/maintainability)\n[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)\n\n`regenmaschine` (German for "rain machine") is a simple, clean, well-tested\nPython library for interacting with\n[RainMachine™ smart sprinkler controllers](http://www.rainmachine.com/).\nIt gives developers an easy API to manage their controllers over their local\nLAN or remotely via the RainMachine™ cloud.\n\n- [Python Versions](#python-versions)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Loading Controllers Multiple Times](#loading-controllers-multiple-times)\n- [Contributing](#contributing)\n\n# Python Versions\n\n`regenmaschine` is currently supported on:\n\n* Python 3.6\n* Python 3.7\n* Python 3.8\n* Python 3.9\n\n# Installation\n\n```python\npip install regenmaschine\n```\n\n# Usage\n\nCreating a `regenmaschine` `Client` might be the easiest thing you do all day:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    client = Client()\n\n    # ...\n\n\nasyncio.run(main())\n```\n\nBy default, the library creates a new connection to the sprinkler controller with each\ncoroutine. If you are calling a large number of coroutines (or merely want to squeeze\nout every second of runtime savings possible), an\n[`aiohttp`](https://github.com/aio-libs/aiohttp) `ClientSession` can be used for connection\npooling:\n\nSee the module docstrings throughout the library for full info on all parameters, return\ntypes, etc.\n\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n\nasyncio.run(main())\n```\n\nOnce you have a client, you can load a local controller (i.e., one that is\naccessible over the LAN) very easily:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        await client.load_local("192.168.1.101", "my_password", port=8080, ssl=True)\n\n        controllers = client.controllers\n        # >>> {\'ab:cd:ef:12:34:56\': <LocalController>}\n\n\nasyncio.run(main())\n```\n\nIf you have 1, 2 or 100 other local controllers, you can load them in the same\nway – `client.controllers` will keep your controllers all organized.\n\nWhat if you have controllers around the world and can\'t access them all over\nthe same local network? No problem! `regenmaschine` allows you to load remote\ncontrollers very easily, as well:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        await client.load_remote("rainmachine_email@host.com", "my_password")\n\n        controllers = client.controllers\n        # >>> {\'xx:xx:xx:xx:xx:xx\': <RemoteController>, ...}\n\n\nasyncio.run(main())\n```\n\nBonus tip: `client.load_remote` will load _all_ controllers owned by that email\naddress.\n\nRegardless of the type of controller you have loaded (local or remote), the\nsame properties and methods are available to each:\n\n```python\nimport asyncio\nimport datetime\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load a local controller:\n        await client.load_local("192.168.1.101", "my_password", port=8080, ssl=True)\n\n        # Load all remote controllers associated with an account:\n        await client.load_remote("rainmachine_email@host.com", "my_password")\n\n        # They all act the same! The only difference is that remote API calls\n        # will pass through the RainMachine™ cloud:\n        for mac_address, controller in client.controllers:\n            # Print some client properties:\n            print(f"Name: {controller.name}")\n            print(f"Host: {controller.host}")\n            print(f"MAC Address: {controller.mac}")\n            print(f"API Version: {controller.api_version}")\n            print(f"Software Version: {controller.software_version}")\n            print(f"Hardware Version: {controller.hardware_version}")\n\n            # Get all diagnostic information:\n            diagnostics = await controller.diagnostics.current()\n\n            # Get all weather parsers:\n            parsers = await controller.parsers.current()\n\n            # Get all programs:\n            programs = await controller.programs.all()\n\n            # Include inactive programs:\n            programs = await controller.programs.all(include_inactive=True)\n\n            # Get a specific program:\n            program_1 = await controller.programs.get(1)\n\n            # Enable or disable a specific program:\n            await controller.programs.enable(1)\n            await controller.programs.disable(1)\n\n            # Get the next run time for all programs:\n            runs = await controller.programs.next()\n\n            # Get all running programs:\n            programs = await controller.programs.running()\n\n            # Start and stop a program:\n            await controller.programs.start(1)\n            await controller.programs.stop(1)\n\n            # Get basic details about all zones:\n            zones = await controller.zones.all()\n\n            # Get advanced details about all zones:\n            zones = await controller.zones.all(details=True)\n\n            # Include inactive zones:\n            zones = await controller.zones.all(include_inactive=True)\n\n            # Get basic details about a specific zone:\n            zone_1 = await controller.zones.get(1)\n\n            # Get advanced details about a specific zone:\n            zone_1 = await controller.zones.get(1, details=True)\n\n            # Enable or disable a specific zone:\n            await controller.zones.enable(1)\n            await controller.zones.disable(1)\n\n            # Start a zone for 60 seconds:\n            await controller.zones.start(1, 60)\n\n            # ...and stop it:\n            await controller.zones.stop(1)\n\n            # Get the device name:\n            name = await controller.provisioning.device_name\n\n            # Get all provisioning settings:\n            settings = await controller.provisioning.settings()\n\n            # Get all networking info related to the device:\n            wifi = await controller.provisioning.wifi()\n\n            # Get various types of active watering restrictions:\n            current = await controller.restrictions.current()\n            universal = await controller.restrictions.universal()\n            hourly = await controller.restrictions.hourly()\n            raindelay = await controller.restrictions.raindelay()\n\n            # Get watering stats:\n            today = await controller.stats.on_date(datetime.date.today())\n            upcoming_days = await controller.stats.upcoming(details=True)\n\n            # Get info on various watering activities not already covered:\n            log = await controller.watering.log(datetime.date.today(), 2)\n            queue = await controller.watering.queue()\n            runs = await controller.watering.runs(datetime.date.today())\n\n            # Pause all watering activities for 30 seconds:\n            await controller.watering.pause_all(30)\n\n            # Unpause all watering activities:\n            await controller.watering.unpause_all()\n\n            # Stop all watering activities:\n            await controller.watering.stop_all()\n\n\nasyncio.run(main())\n```\n\nCheck out `example.py`, the tests, and the source files themselves for method\nsignatures and more examples.\n\n# Loading Controllers Multiple Times\n\nIt is technically possible to load a controller multiple times. Let\'s pretend\nfor a moment that:\n\n* We have a local controller named `Home` (available at `192.168.1.101`).\n* We have a remote controller named `Grandma\'s House`.\n* Both controllers live under our email address: `user@host.com`\n\nIf we load them thus:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load "Home" locally:\n        await client.load_local("192.168.1.101", "my_password")\n\n        # Load all of my controllers remotely:\n        await client.load_remote("user@host.com", "my_password")\n\n\nasyncio.run(main())\n```\n\n...then we will have the following:\n\n1. `Home` will be a `LocalController` and accessible over the LAN.\n2. `Grandma\'s House` will be a `RemoteController` and accessible only over the\nRainMachine™ cloud.\n\nNotice that `regenmaschine` is smart enough to not overwrite a controller that\nalready exists: even though `Home` exists as a remote controller owned by\n`user@host.com`, it had already been loaded locally. By default,\n`regenmaschine` will only load a controller if it hasn\'t been loaded before\n(locally _or_ remotely). If you want to change this behavior, both `load_local`\nand `load_remote` accept an optional `skip_existing` parameter:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load all of my controllers remotely:\n        await client.load_remote("user@host.com", "my_password")\n\n        # Load "Home" locally, overwriting the existing remote controller:\n        await client.load_local("192.168.1.101", "my_password", skip_existing=False)\n\n\nasyncio.run(main())\n```\n\n# Contributing\n\n1. [Check for open features/bugs](https://github.com/bachya/regenmaschine/issues)\n  or [initiate a discussion on one](https://github.com/bachya/regenmaschine/issues/new).\n2. [Fork the repository](https://github.com/bachya/regenmaschine/fork).\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `script/test`\n9. Update `README.md` with any new documentation.\n10. Add yourself to `AUTHORS.md`.\n11. Submit a pull request!\n',
+    'long_description': '# 💧 Regenmaschine: A Simple Python Library for RainMachine™\n\n[![CI](https://github.com/bachya/regenmaschine/workflows/CI/badge.svg)](https://github.com/bachya/regenmaschine/actions)\n[![PyPi](https://img.shields.io/pypi/v/regenmaschine.svg)](https://pypi.python.org/pypi/regenmaschine)\n[![Version](https://img.shields.io/pypi/pyversions/regenmaschine.svg)](https://pypi.python.org/pypi/regenmaschine)\n[![License](https://img.shields.io/pypi/l/regenmaschine.svg)](https://github.com/bachya/regenmaschine/blob/master/LICENSE)\n[![Code Coverage](https://codecov.io/gh/bachya/regenmaschine/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/regenmaschine)\n[![Maintainability](https://api.codeclimate.com/v1/badges/a99a88d28ad37a79dbf6/maintainability)](https://codeclimate.com/github/bachya/regenmaschine/maintainability)\n[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)\n\n`regenmaschine` (German for "rain machine") is a simple, clean, well-tested\nPython library for interacting with\n[RainMachine™ smart sprinkler controllers](http://www.rainmachine.com/).\nIt gives developers an easy API to manage their controllers over their local\nLAN or remotely via the RainMachine™ cloud.\n\n- [Python Versions](#python-versions)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Loading Controllers Multiple Times](#loading-controllers-multiple-times)\n- [Contributing](#contributing)\n\n# Python Versions\n\n`regenmaschine` is currently supported on:\n\n* Python 3.6\n* Python 3.7\n* Python 3.8\n* Python 3.9\n\n# Installation\n\n```python\npip install regenmaschine\n```\n\n# Usage\n\nCreating a `regenmaschine` `Client` might be the easiest thing you do all day:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    client = Client()\n\n    # ...\n\n\nasyncio.run(main())\n```\n\nBy default, the library creates a new connection to the sprinkler controller with each\ncoroutine. If you are calling a large number of coroutines (or merely want to squeeze\nout every second of runtime savings possible), an\n[`aiohttp`](https://github.com/aio-libs/aiohttp) `ClientSession` can be used for connection\npooling:\n\nSee the module docstrings throughout the library for full info on all parameters, return\ntypes, etc.\n\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n\nasyncio.run(main())\n```\n\n## Loading Local (Accessible Over the LAN) Controllers\n\nOnce you have a client, you can load a local controller (i.e., one that is\naccessible over the LAN) very easily:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        await client.load_local("192.168.1.101", "my_password", port=8080, ssl=True)\n\n        controllers = client.controllers\n        # >>> {\'ab:cd:ef:12:34:56\': <LocalController>}\n\n\nasyncio.run(main())\n```\n\n## Loading Remote (Accessible Over the RainMachine Cloud) Controllers\n\nIf you have 1, 2 or 100 other local controllers, you can load them in the same\nway – `client.controllers` will keep your controllers all organized.\n\nWhat if you have controllers around the world and can\'t access them all over\nthe same local network? No problem! `regenmaschine` allows you to load remote\ncontrollers very easily, as well:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        await client.load_remote("rainmachine_email@host.com", "my_password")\n\n        controllers = client.controllers\n        # >>> {\'xx:xx:xx:xx:xx:xx\': <RemoteController>, ...}\n\n\nasyncio.run(main())\n```\n\nBonus tip: `client.load_remote` will load _all_ controllers owned by that email\naddress.\n\n## Using the Controller\n\nRegardless of the type of controller you have loaded (local or remote), the\nsame properties and methods are available to each:\n\n```python\nimport asyncio\nimport datetime\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load a local controller:\n        await client.load_local("192.168.1.101", "my_password", port=8080, ssl=True)\n\n        # Load all remote controllers associated with an account:\n        await client.load_remote("rainmachine_email@host.com", "my_password")\n\n        # They all act the same! The only difference is that remote API calls\n        # will pass through the RainMachine™ cloud:\n        for mac_address, controller in client.controllers:\n            # Print some client properties:\n            print(f"Name: {controller.name}")\n            print(f"Host: {controller.host}")\n            print(f"MAC Address: {controller.mac}")\n            print(f"API Version: {controller.api_version}")\n            print(f"Software Version: {controller.software_version}")\n            print(f"Hardware Version: {controller.hardware_version}")\n\n            # Get all diagnostic information:\n            diagnostics = await controller.diagnostics.current()\n\n            # Get all weather parsers:\n            parsers = await controller.parsers.current()\n\n            # Get all programs:\n            programs = await controller.programs.all()\n\n            # Include inactive programs:\n            programs = await controller.programs.all(include_inactive=True)\n\n            # Get a specific program:\n            program_1 = await controller.programs.get(1)\n\n            # Enable or disable a specific program:\n            await controller.programs.enable(1)\n            await controller.programs.disable(1)\n\n            # Get the next run time for all programs:\n            runs = await controller.programs.next()\n\n            # Get all running programs:\n            programs = await controller.programs.running()\n\n            # Start and stop a program:\n            await controller.programs.start(1)\n            await controller.programs.stop(1)\n\n            # Get basic details about all zones:\n            zones = await controller.zones.all()\n\n            # Get advanced details about all zones:\n            zones = await controller.zones.all(details=True)\n\n            # Include inactive zones:\n            zones = await controller.zones.all(include_inactive=True)\n\n            # Get basic details about a specific zone:\n            zone_1 = await controller.zones.get(1)\n\n            # Get advanced details about a specific zone:\n            zone_1 = await controller.zones.get(1, details=True)\n\n            # Enable or disable a specific zone:\n            await controller.zones.enable(1)\n            await controller.zones.disable(1)\n\n            # Start a zone for 60 seconds:\n            await controller.zones.start(1, 60)\n\n            # ...and stop it:\n            await controller.zones.stop(1)\n\n            # Get the device name:\n            name = await controller.provisioning.device_name\n\n            # Get all provisioning settings:\n            settings = await controller.provisioning.settings()\n\n            # Get all networking info related to the device:\n            wifi = await controller.provisioning.wifi()\n\n            # Get various types of active watering restrictions:\n            current = await controller.restrictions.current()\n            universal = await controller.restrictions.universal()\n            hourly = await controller.restrictions.hourly()\n            raindelay = await controller.restrictions.raindelay()\n\n            # Get watering stats:\n            today = await controller.stats.on_date(datetime.date.today())\n            upcoming_days = await controller.stats.upcoming(details=True)\n\n            # Get info on various watering activities not already covered:\n            log = await controller.watering.log(datetime.date.today(), 2)\n            queue = await controller.watering.queue()\n            runs = await controller.watering.runs(datetime.date.today())\n\n            # Pause all watering activities for 30 seconds:\n            await controller.watering.pause_all(30)\n\n            # Unpause all watering activities:\n            await controller.watering.unpause_all()\n\n            # Stop all watering activities:\n            await controller.watering.stop_all()\n\n\nasyncio.run(main())\n```\n\nCheck out `example.py`, the tests, and the source files themselves for method\nsignatures and more examples. For additional reference, the full RainMachine™ API documentation is available [here](https://rainmachine.docs.apiary.io/).\n\n# Loading Controllers Multiple Times\n\nIt is technically possible to load a controller multiple times. Let\'s pretend\nfor a moment that:\n\n* We have a local controller named `Home` (available at `192.168.1.101`).\n* We have a remote controller named `Grandma\'s House`.\n* Both controllers live under our email address: `user@host.com`\n\nIf we load them thus:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load "Home" locally:\n        await client.load_local("192.168.1.101", "my_password")\n\n        # Load all of my controllers remotely:\n        await client.load_remote("user@host.com", "my_password")\n\n\nasyncio.run(main())\n```\n\n...then we will have the following:\n\n1. `Home` will be a `LocalController` and accessible over the LAN.\n2. `Grandma\'s House` will be a `RemoteController` and accessible only over the\nRainMachine™ cloud.\n\nNotice that `regenmaschine` is smart enough to not overwrite a controller that\nalready exists: even though `Home` exists as a remote controller owned by\n`user@host.com`, it had already been loaded locally. By default,\n`regenmaschine` will only load a controller if it hasn\'t been loaded before\n(locally _or_ remotely). If you want to change this behavior, both `load_local`\nand `load_remote` accept an optional `skip_existing` parameter:\n\n```python\nimport asyncio\n\nfrom aiohttp import ClientSession\n\nfrom regenmaschine import Client\n\n\nasync def main() -> None:\n    """Run!"""\n    async with ClientSession() as session:\n        client = Client(session=session)\n\n        # Load all of my controllers remotely:\n        await client.load_remote("user@host.com", "my_password")\n\n        # Load "Home" locally, overwriting the existing remote controller:\n        await client.load_local("192.168.1.101", "my_password", skip_existing=False)\n\n\nasyncio.run(main())\n```\n\n# Contributing\n\n1. [Check for open features/bugs](https://github.com/bachya/regenmaschine/issues)\n  or [initiate a discussion on one](https://github.com/bachya/regenmaschine/issues/new).\n2. [Fork the repository](https://github.com/bachya/regenmaschine/fork).\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `script/test`\n9. Update `README.md` with any new documentation.\n10. Add yourself to `AUTHORS.md`.\n11. Submit a pull request!\n',
     'author': 'Aaron Bach',
     'author_email': 'bachya1208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/bachya/regenmaschine',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `regenmaschine-3.1.5/PKG-INFO` & `regenmaschine-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: regenmaschine
-Version: 3.1.5
+Version: 3.2.0
 Summary: A simple API for RainMachine sprinkler controllers
 Home-page: https://github.com/bachya/regenmaschine
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.6.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
@@ -102,14 +103,16 @@
     async with ClientSession() as session:
         client = Client(session=session)
 
 
 asyncio.run(main())
 ```
 
+## Loading Local (Accessible Over the LAN) Controllers
+
 Once you have a client, you can load a local controller (i.e., one that is
 accessible over the LAN) very easily:
 
 ```python
 import asyncio
 
 from aiohttp import ClientSession
@@ -127,14 +130,16 @@
         controllers = client.controllers
         # >>> {'ab:cd:ef:12:34:56': <LocalController>}
 
 
 asyncio.run(main())
 ```
 
+## Loading Remote (Accessible Over the RainMachine Cloud) Controllers
+
 If you have 1, 2 or 100 other local controllers, you can load them in the same
 way – `client.controllers` will keep your controllers all organized.
 
 What if you have controllers around the world and can't access them all over
 the same local network? No problem! `regenmaschine` allows you to load remote
 controllers very easily, as well:
 
@@ -159,14 +164,16 @@
 
 asyncio.run(main())
 ```
 
 Bonus tip: `client.load_remote` will load _all_ controllers owned by that email
 address.
 
+## Using the Controller
+
 Regardless of the type of controller you have loaded (local or remote), the
 same properties and methods are available to each:
 
 ```python
 import asyncio
 import datetime
 
@@ -285,15 +292,15 @@
             await controller.watering.stop_all()
 
 
 asyncio.run(main())
 ```
 
 Check out `example.py`, the tests, and the source files themselves for method
-signatures and more examples.
+signatures and more examples. For additional reference, the full RainMachine™ API documentation is available [here](https://rainmachine.docs.apiary.io/).
 
 # Loading Controllers Multiple Times
 
 It is technically possible to load a controller multiple times. Let's pretend
 for a moment that:
 
 * We have a local controller named `Home` (available at `192.168.1.101`).
```

