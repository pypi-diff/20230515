# Comparing `tmp/usbid-2.1.tar.gz` & `tmp/usbid-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/usbid-2.1.tar", last modified: Mon Jul 18 12:08:24 2022, max compression
+gzip compressed data, was "usbid-2.2.tar", last modified: Mon May 15 12:09:57 2023, max compression
```

## Comparing `usbid-2.1.tar` & `usbid-2.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-07-18 12:08:24.000000 usbid-2.1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2022-07-18 12:07:24.000000 usbid-2.1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1220 2022-07-18 12:06:49.000000 usbid-2.1/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)       66 2022-07-18 12:05:33.000000 usbid-2.1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)      711 2022-07-18 12:07:14.000000 usbid-2.1/HISTORY.rst
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-07-18 12:08:24.000000 usbid-2.1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      393 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       29 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)        6 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8910 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid.egg-info/PKG-INFO
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    19421 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/fs.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9234 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/fs.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1296 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-07-18 12:08:24.000000 usbid-2.1/src/usbid/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   158443 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/testing/1.tgz
--rw-r--r--   0 rnix      (1000) rnix      (1000)   179446 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/testing/3.tgz
--rw-r--r--   0 rnix      (1000) rnix      (1000)   143295 2022-07-18 12:05:33.000000 usbid-2.1/src/usbid/testing/2.tgz
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4249 2022-07-18 12:05:33.000000 usbid-2.1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2022-07-18 12:08:24.000000 usbid-2.1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8910 2022-07-18 12:08:24.000000 usbid-2.1/PKG-INFO
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:09:57.566799 usbid-2.2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1028 2023-05-15 12:09:57.000000 usbid-2.2/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2023-05-15 12:09:57.000000 usbid-2.2/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       66 2023-05-15 12:09:57.000000 usbid-2.2/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7420 2023-05-15 12:09:57.566799 usbid-2.2/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4084 2023-05-15 12:09:57.000000 usbid-2.2/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-05-15 12:09:57.566799 usbid-2.2/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1338 2023-05-15 12:09:57.000000 usbid-2.2/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:09:57.562800 usbid-2.2/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:09:57.566799 usbid-2.2/src/usbid/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      107 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9334 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/fs.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:09:57.566799 usbid-2.2/src/usbid/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   158443 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/testing/1.tgz
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   143295 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/testing/2.tgz
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   179446 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/testing/3.tgz
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25033 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid/tests.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:09:57.566799 usbid-2.2/src/usbid.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7420 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      386 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       28 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        6 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/top_level.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:09:57.000000 usbid-2.2/src/usbid.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `usbid-2.1/LICENSE.rst` & `usbid-2.2/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 License
 =======
 
-Copyright (c) 2013-2022, BlueDynamics Alliance, Austria, Germany, Switzerland
+Copyright (c) 2013-2023, BlueDynamics Alliance, Austria, Germany, Switzerland
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this 
   list of conditions and the following disclaimer.
```

### Comparing `usbid-2.1/src/usbid/fs.rst` & `usbid-2.2/src/usbid/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,640 +1,646 @@
-Linux USB file system
-=====================
-
-Container
----------
-
-::
-
-    >>> from usbid.fs import Container
-    >>> container = Container()
-    >>> container.keys()
-    Traceback (most recent call last):
-      ...
-    NotImplementedError
-
-    >>> container['key']
-    Traceback (most recent call last):
-      ...
-    NotImplementedError
-
-    >>> class TestContainer(Container):
-    ...     def __iter__(self):
-    ...         return iter(['1', '2'])
-    ...     def __getitem__(self, key):
-    ...         return key
-
-    >>> test_container = TestContainer()
-    >>> test_container.keys()
-    ['1', '2']
-
-    >>> test_container['1']
-    '1'
-
-
-FileAttributes
---------------
-
-::
-
-    >>> import os
-
-    >>> with open(os.path.join(TEMPDIR, 'file_attribute'), 'wt') as file:
-    ...     file.write('File attribute value')
-
-    >>> from usbid.fs import FileAttributes
-
-    >>> class TestFileAttributes(FileAttributes):
-    ...     __file_attributes__ = ['file_attribute']
-    ...     fs_path = TEMPDIR
-    ...     class_attribute = 'Class Attribute'
-
-    >>> test_file_attributes = TestFileAttributes()
-    >>> test_file_attributes.class_attribute
-    'Class Attribute'
-
-    >>> test_file_attributes.file_attribute
-    'File attribute value'
-
-    >>> test_file_attributes.no_attribute
-    Traceback (most recent call last):
-      ...
-    AttributeError: 'TestFileAttributes' object has no attribute 'no_attribute'
-
-    >>> def get_file_attribues(obj):
-    ...    ret = []
-    ...    for attr_name in obj.__file_attributes__:
-    ...        ret.append((attr_name, getattr(obj, attr_name)))
-    ...    return ret
-
-    >>> get_file_attribues(test_file_attributes)
-    [('file_attribute', 'File attribute value')]
-
-
-USB
----
-
-::
-
-    >>> from usbid import USB
-
-    >>> test_data_1_dir = os.path.join(
-    ...     TEMPDIR, '1', 'sys', 'bus', 'usb', 'devices')
-
-    >>> usb = USB(fs_path=test_data_1_dir)
-    >>> usb
-    <usbid.fs.USB [/.../1/sys/bus/usb/devices] at ...>
-
-    >>> usb.fs_path
-    '.../1/sys/bus/usb/devices'
-
-    >>> usb.fs_name
-    'devices'
-
-    >>> usb.fs_parent
-    '.../1/sys/bus/usb'
-
-    >>> sorted(usb.keys())
-    ['1', '2', '3', '4']
-
-    >>> usb['0']
-    Traceback (most recent call last):
-      ...
-    KeyError: '0'
-
-    >>> usb['1']
-    <usbid.fs.Bus [usb1] at ...>
-
-    >>> sorted(usb.values(), key=lambda x: x.fs_name)
-    [<usbid.fs.Bus [usb1] at ...>, 
-    <usbid.fs.Bus [usb2] at ...>, 
-    <usbid.fs.Bus [usb3] at ...>, 
-    <usbid.fs.Bus [usb4] at ...>]
-
-    >>> sorted(usb.items())
-    [('1', <usbid.fs.Bus [usb1] at ...>), 
-    ('2', <usbid.fs.Bus [usb2] at ...>), 
-    ('3', <usbid.fs.Bus [usb3] at ...>), 
-    ('4', <usbid.fs.Bus [usb4] at ...>)]
-
-    >>> MARKER = object()
-    >>> usb.get('0', default=MARKER) is MARKER
-    True
-
-    >>> usb.get('1', default=MARKER) is MARKER
-    False
-
-
-Bus
----
-
-::
-
-    >>> from usbid import Bus
-    >>> Bus(name=None, parent=None, fs_path='inexistent')
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid path given
-
-    >>> bus = usb['3']
-    >>> bus
-    <usbid.fs.Bus [usb3] at ...>
-
-    >>> bus.name
-    '3'
-
-    >>> sorted(bus.keys())
-    ['2', '4']
-
-    >>> bus['1']
-    Traceback (most recent call last):
-      ...
-    KeyError: '1'
-
-    >>> bus['2']
-    <usbid.fs.Port [3-2] at ...>
-
-    >>> sorted(bus.values(), key=lambda x: x.name)
-    [<usbid.fs.Port [3-2] at ...>, 
-    <usbid.fs.Port [3-4] at ...>]
-
-    >>> sorted(bus.items(), key=lambda x: x[0])
-    [('2', <usbid.fs.Port [3-2] at ...>), 
-    ('4', <usbid.fs.Port [3-4] at ...>)]
-
-    >>> get_file_attribues(bus)
-    [('authorized', '1'), 
-    ('authorized_default', '1'), 
-    ('avoid_reset_quirk', '0'), 
-    ('bcdDevice', '0313'), 
-    ('bConfigurationValue', '1'), 
-    ('bDeviceClass', '09'), 
-    ('bDeviceProtocol', '01'), 
-    ('bDeviceSubClass', '00'), 
-    ('bmAttributes', 'e0'), 
-    ('bMaxPacketSize0', '64'), 
-    ('bMaxPower', '0mA'), 
-    ('bNumConfigurations', '1'), 
-    ('bNumInterfaces', '1'), 
-    ('busnum', '3'), 
-    ('dev', '189:256'), 
-    ('devnum', '1'), 
-    ('devpath', '0'), 
-    ('idProduct', '0002'), 
-    ('idVendor', '1d6b'), 
-    ('ltm_capable', 'no'), 
-    ('manufacturer', 'Linux 3.13.0-48-generic xhci_hcd'), 
-    ('maxchild', '4'), 
-    ('product', 'xHCI Host Controller'), 
-    ('quirks', '0x0'), 
-    ('removable', 'unknown'), 
-    ('serial', '0000:00:14.0'), 
-    ('speed', '480'), 
-    ('uevent', 'MAJOR=189\nMINOR=256\nDEVNAME=bus/usb/003/001\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=1d6b/2/313\nTYPE=9/0/1\nBUSNUM=003\nDEVNUM=001'), 
-    ('urbnum', '884'), 
-    ('version', '2.00')]
-
-    >>> bus.interfaces
-    [<usbid.fs.Interface [3-0:1.0] at ...>]
-
-    >>> interface = bus.interfaces[0]
-    >>> get_file_attribues(interface)
-    [('bAlternateSetting', '0'), 
-    ('bInterfaceClass', '09'), 
-    ('bInterfaceNumber', '00'), 
-    ('bInterfaceProtocol', '00'), 
-    ('bInterfaceSubClass', '00'), 
-    ('bNumEndpoints', '01'), 
-    ('interface', None), 
-    ('modalias', 'usb:v1D6Bp0002d0313dc09dsc00dp01ic09isc00ip00in00'), 
-    ('supports_autosuspend', '1'), 
-    ('uevent', 'DEVTYPE=usb_interface\nDRIVER=hub\nPRODUCT=1d6b/2/313\nTYPE=9/0/1\nINTERFACE=9/0/0\nMODALIAS=usb:v1D6Bp0002d0313dc09dsc00dp01ic09isc00ip00in00')]
-
-
-Port
-----
-
-::
-
-    >>> from usbid import Port
-    >>> Port(name=None, parent=None, fs_path='inexistent')
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid path given
-
-    >>> port = bus['2']
-    >>> port
-    <usbid.fs.Port [3-2] at ...>
-
-    >>> port.fs_path
-    '.../1/sys/bus/usb/devices/usb3/3-2'
-
-    >>> port.fs_name
-    '3-2'
-
-    >>> get_file_attribues(port)
-    [('authorized', '1'), 
-    ('avoid_reset_quirk', '0'), 
-    ('bcdDevice', '0100'), 
-    ('bConfigurationValue', '1'), 
-    ('bDeviceClass', '09'), 
-    ('bDeviceProtocol', '01'), 
-    ('bDeviceSubClass', '00'), 
-    ('bmAttributes', 'e0'), 
-    ('bMaxPacketSize0', '64'), 
-    ('bMaxPower', '100mA'), 
-    ('bNumConfigurations', '1'), 
-    ('bNumInterfaces', '1'), 
-    ('busnum', '3'), 
-    ('dev', '189:378'), 
-    ('devnum', '123'), 
-    ('devpath', '2'), 
-    ('idProduct', '005a'), 
-    ('idVendor', '0409'), 
-    ('ltm_capable', 'no'), 
-    ('manufacturer', None), 
-    ('maxchild', '4'), 
-    ('product', None), 
-    ('quirks', '0x0'), 
-    ('removable', 'removable'), 
-    ('serial', None), 
-    ('speed', '480'), 
-    ('uevent', 'MAJOR=189\nMINOR=378\nDEVNAME=bus/usb/003/123\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=409/5a/100\nTYPE=9/0/1\nBUSNUM=003\nDEVNUM=123'), 
-    ('urbnum', '47'), 
-    ('version', '2.00')]
-
-    >>> port.interfaces
-    [<usbid.fs.Interface [3-2:1.0] at ...>]
-
-    >>> interface = port.interfaces[0]
-    >>> get_file_attribues(interface)
-    [('bAlternateSetting', '0'), 
-    ('bInterfaceClass', '09'), 
-    ('bInterfaceNumber', '00'), 
-    ('bInterfaceProtocol', '00'), 
-    ('bInterfaceSubClass', '00'), 
-    ('bNumEndpoints', '01'), 
-    ('interface', None), 
-    ('modalias', 'usb:v0409p005Ad0100dc09dsc00dp01ic09isc00ip00in00'), 
-    ('supports_autosuspend', '1'), 
-    ('uevent', 'DEVTYPE=usb_interface\nDRIVER=hub\nPRODUCT=409/5a/100\nTYPE=9/0/1\nINTERFACE=9/0/0\nMODALIAS=usb:v0409p005Ad0100dc09dsc00dp01ic09isc00ip00in00')]
-
-    >>> sorted(port.keys())
-    ['1', '2', '3', '4']
-
-    >>> port['0']
-    Traceback (most recent call last):
-      ...
-    KeyError: '0'
-
-    >>> sub_port = port['1']
-    >>> sub_port
-    <usbid.fs.Port [3-2.1] at ...>
-
-    >>> sub_port.fs_path
-    '.../1/sys/bus/usb/devices/usb3/3-2/3-2.1'
-
-    >>> sub_port.fs_name
-    '3-2.1'
-
-    >>> get_file_attribues(sub_port)
-    [('authorized', '1'), 
-    ('avoid_reset_quirk', '0'), 
-    ('bcdDevice', '0600'), 
-    ('bConfigurationValue', '1'), 
-    ('bDeviceClass', '00'), 
-    ('bDeviceProtocol', '00'), 
-    ('bDeviceSubClass', '00'), 
-    ('bmAttributes', 'a0'), 
-    ('bMaxPacketSize0', '8'), 
-    ('bMaxPower', '90mA'), 
-    ('bNumConfigurations', '1'), 
-    ('bNumInterfaces', '1'), 
-    ('busnum', '3'), 
-    ('dev', '189:379'), 
-    ('devnum', '124'), 
-    ('devpath', '2.1'), 
-    ('idProduct', '6001'), 
-    ('idVendor', '0403'), 
-    ('ltm_capable', 'no'), 
-    ('manufacturer', 'FTDI'), 
-    ('maxchild', '0'), 
-    ('product', 'FT232R USB UART'), 
-    ('quirks', '0x0'), 
-    ('removable', 'unknown'), 
-    ('serial', 'A7022OOQ'), 
-    ('speed', '12'), 
-    ('uevent', 'MAJOR=189\nMINOR=379\nDEVNAME=bus/usb/003/124\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=403/6001/600\nTYPE=0/0/0\nBUSNUM=003\nDEVNUM=124'), 
-    ('urbnum', '15'), 
-    ('version', '2.00')]
-
-    >>> sub_port.interfaces
-    [<usbid.fs.Interface [3-2.1:1.0] at ...>]
-
-    >>> interface = sub_port.interfaces[0]
-    >>> get_file_attribues(interface)
-    [('bAlternateSetting', '0'), 
-    ('bInterfaceClass', 'ff'), 
-    ('bInterfaceNumber', '00'), 
-    ('bInterfaceProtocol', 'ff'), 
-    ('bInterfaceSubClass', 'ff'), 
-    ('bNumEndpoints', '02'), 
-    ('interface', 'FT232R USB UART'), 
-    ('modalias', 'usb:v0403p6001d0600dc00dsc00dp00icFFiscFFipFFin00'), 
-    ('supports_autosuspend', '1'), 
-    ('uevent', 'DEVTYPE=usb_interface\nDRIVER=ftdi_sio\nPRODUCT=403/6001/600\nTYPE=0/0/0\nINTERFACE=255/255/255\nMODALIAS=usb:v0403p6001d0600dc00dsc00dp00icFFiscFFipFFin00')]
-
-
-Interface
----------
-
-::
-
-    >>> from usbid import Interface
-    >>> Interface(parent=None, fs_path='inexistent')
-    Traceback (most recent call last):
-      ...
-    ValueError: Invalid path given
-
-    >>> port = usb['3']['2']['1']
-    >>> port.interfaces
-    [<usbid.fs.Interface [3-2.1:1.0] at ...>]
-
-    >>> interface = port.interfaces[0]
-    >>> interface.parent
-    <usbid.fs.Port [3-2.1] at ...>
-
-    >>> interface.fs_name
-    '3-2.1:1.0'
-
-    >>> interface.manufacturer
-    'FTDI'
-
-    >>> interface.product
-    'FT232R USB UART'
-
-    >>> interface = usb.get_interface(interface.fs_name)
-    >>> interface
-    <usbid.fs.Interface [3-2.1:1.0] at ...>
-
-    >>> interface.parent
-    <usbid.fs.Port [3-2.1] at ...>
-
-    >>> interface.manufacturer
-    'FTDI'
-
-    >>> interface.product
-    'FT232R USB UART'
-
-
-Test data tree 1
-----------------
-
-::
-
-    >>> usb.printtree()
-    <usbid.fs.USB [/.../1/sys/bus/usb/devices] at ...>
-      <usbid.fs.Bus [usb1] at ...>
-          - Linux 3.13.0-48-generic ehci_hcd
-          - EHCI Host Controller
-        <usbid.fs.Interface [1-0:1.0] at ...>
-        <usbid.fs.Port [1-1] at ...>
-          <usbid.fs.Interface [1-1:1.0] at ...>
-          <usbid.fs.Port [1-1.2] at ...>
-              - USB Optical Mouse
-            <usbid.fs.Interface [1-1.2:1.0] at ...>
-          <usbid.fs.Port [1-1.3] at ...>
-              - Auth
-              - Biometric Coprocessor
-            <usbid.fs.Interface [1-1.3:1.0] at ...>
-          <usbid.fs.Port [1-1.4] at ...>
-              - Broadcom Corp
-              - BCM20702A0
-            <usbid.fs.Interface [1-1.4:1.0] at ...>
-            <usbid.fs.Interface [1-1.4:1.1] at ...>
-            <usbid.fs.Interface [1-1.4:1.2] at ...>
-            <usbid.fs.Interface [1-1.4:1.3] at ...>
-          <usbid.fs.Port [1-1.6] at ...>
-              - SunplusIT INC.
-              - Integrated Camera
-            <usbid.fs.Interface [1-1.6:1.0] at ...>
-            <usbid.fs.Interface [1-1.6:1.1] at ...>
-      <usbid.fs.Bus [usb2] at ...>
-          - Linux 3.13.0-48-generic ehci_hcd
-          - EHCI Host Controller
-        <usbid.fs.Interface [2-0:1.0] at ...>
-        <usbid.fs.Port [2-1] at ...>
-          <usbid.fs.Interface [2-1:1.0] at ...>
-      <usbid.fs.Bus [usb3] at ...>
-          - Linux 3.13.0-48-generic xhci_hcd
-          - xHCI Host Controller
-        <usbid.fs.Interface [3-0:1.0] at ...>
-        <usbid.fs.Port [3-2] at ...>
-          <usbid.fs.Interface [3-2:1.0] at ...>
-          <usbid.fs.Port [3-2.1] at ...>
-              - FTDI
-              - FT232R USB UART
-            <usbid.fs.Interface [3-2.1:1.0] at ...>
-              - ttyUSB0
-          <usbid.fs.Port [3-2.2] at ...>
-              - FTDI
-              - FT232R USB UART
-            <usbid.fs.Interface [3-2.2:1.0] at ...>
-              - ttyUSB1
-          <usbid.fs.Port [3-2.3] at ...>
-              - FTDI
-              - FT232R USB UART
-            <usbid.fs.Interface [3-2.3:1.0] at ...>
-              - ttyUSB2
-          <usbid.fs.Port [3-2.4] at ...>
-              - FTDI
-              - FT232R USB UART
-            <usbid.fs.Interface [3-2.4:1.0] at ...>
-              - ttyUSB3
-        <usbid.fs.Port [3-4] at ...>
-            - Lenovo
-            - H5321 gw
-          <usbid.fs.Interface [3-4:1.0] at ...>
-          <usbid.fs.Interface [3-4:1.1] at ...>
-            - ttyACM0
-          <usbid.fs.Interface [3-4:1.2] at ...>
-          <usbid.fs.Interface [3-4:1.3] at ...>
-            - ttyACM1
-          <usbid.fs.Interface [3-4:1.4] at ...>
-          <usbid.fs.Interface [3-4:1.5] at ...>
-          <usbid.fs.Interface [3-4:1.6] at ...>
-          <usbid.fs.Interface [3-4:1.7] at ...>
-          <usbid.fs.Interface [3-4:1.8] at ...>
-          <usbid.fs.Interface [3-4:1.9] at ...>
-            - ttyACM2
-      <usbid.fs.Bus [usb4] at ...>
-          - Linux 3.13.0-48-generic xhci_hcd
-          - xHCI Host Controller
-        <usbid.fs.Interface [4-0:1.0] at ...>
-
-    >>> sorted(usb.aggregated_interfaces(), key=lambda x: x.fs_path)
-    [<usbid.fs.Interface [1-0:1.0] at ...>, 
-    <usbid.fs.Interface [1-1.2:1.0] at ...>, 
-    <usbid.fs.Interface [1-1.3:1.0] at ...>, 
-    <usbid.fs.Interface [1-1.4:1.0] at ...>, 
-    <usbid.fs.Interface [1-1.4:1.1] at ...>, 
-    <usbid.fs.Interface [1-1.4:1.2] at ...>, 
-    <usbid.fs.Interface [1-1.4:1.3] at ...>, 
-    <usbid.fs.Interface [1-1.6:1.0] at ...>, 
-    <usbid.fs.Interface [1-1.6:1.1] at ...>, 
-    <usbid.fs.Interface [1-1:1.0] at ...>, 
-    <usbid.fs.Interface [2-0:1.0] at ...>, 
-    <usbid.fs.Interface [2-1:1.0] at ...>, 
-    <usbid.fs.Interface [3-0:1.0] at ...>, 
-    <usbid.fs.Interface [3-2.1:1.0] at ...>, 
-    <usbid.fs.Interface [3-2.2:1.0] at ...>, 
-    <usbid.fs.Interface [3-2.3:1.0] at ...>, 
-    <usbid.fs.Interface [3-2.4:1.0] at ...>, 
-    <usbid.fs.Interface [3-2:1.0] at ...>, 
-    <usbid.fs.Interface [3-4:1.0] at ...>, 
-    <usbid.fs.Interface [3-4:1.1] at ...>, 
-    <usbid.fs.Interface [3-4:1.2] at ...>, 
-    <usbid.fs.Interface [3-4:1.3] at ...>, 
-    <usbid.fs.Interface [3-4:1.4] at ...>, 
-    <usbid.fs.Interface [3-4:1.5] at ...>, 
-    <usbid.fs.Interface [3-4:1.6] at ...>, 
-    <usbid.fs.Interface [3-4:1.7] at ...>, 
-    <usbid.fs.Interface [3-4:1.8] at ...>, 
-    <usbid.fs.Interface [3-4:1.9] at ...>, 
-    <usbid.fs.Interface [4-0:1.0] at ...>]
-
-    >>> tty_ifaces = sorted(
-    ...     usb.aggregated_interfaces(tty=True),
-    ...     key=lambda x: x.fs_path
-    ... )
-    >>> ['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]
-    ['/.../1/sys/bus/usb/devices/usb3/3-2/3-2.1/3-2.1:1.0 - ttyUSB0', 
-    '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.2/3-2.2:1.0 - ttyUSB1', 
-    '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.3/3-2.3:1.0 - ttyUSB2', 
-    '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.4/3-2.4:1.0 - ttyUSB3', 
-    '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0', 
-    '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1', 
-    '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
-
-
-Test data tree 2
-----------------
-
-::
-
-    >>> test_data_2_dir = os.path.join(
-    ...     TEMPDIR, '2', 'sys', 'bus', 'usb', 'devices')
-
-    >>> usb = USB(fs_path=test_data_2_dir)
-    >>> usb.printtree()
-    <usbid.fs.USB [/.../2/sys/bus/usb/devices] at ...>
-      ...
-      <usbid.fs.Bus [usb3] at ...>
-          - Linux 3.13.0-48-generic xhci_hcd
-          - xHCI Host Controller
-        <usbid.fs.Interface [3-0:1.0] at ...>
-        <usbid.fs.Port [3-2] at ...>
-            - FTDI
-            - USB <-> Serial Cable
-          <usbid.fs.Interface [3-2:1.0] at ...>
-            - ttyUSB0
-          <usbid.fs.Interface [3-2:1.1] at ...>
-            - ttyUSB1
-      ...
-
-    >>> tty_ifaces = sorted(
-    ...     usb.aggregated_interfaces(tty=True),
-    ...     key=lambda x: x.fs_path
-    ... )
-    >>> ['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]
-    ['.../2/sys/bus/usb/devices/usb3/3-2/3-2:1.0 - ttyUSB0', 
-    '/.../2/sys/bus/usb/devices/usb3/3-2/3-2:1.1 - ttyUSB1', 
-    '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0', 
-    '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1', 
-    '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
-
-
-Test data tree 3
-----------------
-
-::
-
-    >>> test_data_3_dir = os.path.join(
-    ...     TEMPDIR, '3', 'sys', 'bus', 'usb', 'devices')
-
-    >>> usb = USB(fs_path=test_data_3_dir)
-    >>> usb.printtree()
-    <usbid.fs.USB [/.../3/sys/bus/usb/devices] at ...>
-      <usbid.fs.Bus [usb3] at ...>
-          - Linux 3.13.0-48-generic xhci_hcd
-          - xHCI Host Controller
-        <usbid.fs.Interface [3-0:1.0] at ...>
-        <usbid.fs.Port [3-2] at ...>
-          <usbid.fs.Interface [3-2:1.0] at ...>
-          <usbid.fs.Port [3-2.2] at ...>
-              - DMX4ALL
-              - NanoDMX Interface
-            <usbid.fs.Interface [3-2.2:1.0] at ...>
-              - ttyACM3
-            <usbid.fs.Interface [3-2.2:1.1] at ...>
-          <usbid.fs.Port [3-2.4] at ...>
-              - Prolific Technology Inc.
-              - USB-Serial Controller D
-            <usbid.fs.Interface [3-2.4:1.0] at ...>
-              - ttyUSB0
-          <usbid.fs.Port [3-2.6] at ...>
-            <usbid.fs.Interface [3-2.6:1.0] at ...>
-            <usbid.fs.Port [3-2.6.1] at ...>
-                - FTDI
-                - FT232R USB UART
-              <usbid.fs.Interface [3-2.6.1:1.0] at ...>
-                - ttyUSB3
-            <usbid.fs.Port [3-2.6.2] at ...>
-                - FTDI
-                - FT232R USB UART
-              <usbid.fs.Interface [3-2.6.2:1.0] at ...>
-                - ttyUSB4
-            <usbid.fs.Port [3-2.6.3] at ...>
-                - FTDI
-                - FT232R USB UART
-              <usbid.fs.Interface [3-2.6.3:1.0] at ...>
-                - ttyUSB5
-            <usbid.fs.Port [3-2.6.4] at ...>
-                - FTDI
-                - FT232R USB UART
-              <usbid.fs.Interface [3-2.6.4:1.0] at ...>
-                - ttyUSB6
-          <usbid.fs.Port [3-2.7] at ...>
-              - FTDI
-              - USB <-> Serial Cable
-            <usbid.fs.Interface [3-2.7:1.0] at ...>
-              - ttyUSB1
-            <usbid.fs.Interface [3-2.7:1.1] at ...>
-              - ttyUSB2
-      ...
-
-    >>> tty_ifaces = sorted(
-    ...     usb.aggregated_interfaces(tty=True),
-    ...     key=lambda x: x.fs_path
-    ... )
-    >>> ['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]
-    ['/.../3/sys/bus/usb/devices/usb3/3-2/3-2.2/3-2.2:1.0 - ttyACM3', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.4/3-2.4:1.0 - ttyUSB0', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.1/3-2.6.1:1.0 - ttyUSB3', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.2/3-2.6.2:1.0 - ttyUSB4', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.3/3-2.6.3:1.0 - ttyUSB5', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.4/3-2.6.4:1.0 - ttyUSB6', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.7/3-2.7:1.0 - ttyUSB1', 
-    '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.7/3-2.7:1.1 - ttyUSB2', 
-    '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0', 
-    '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1', 
-    '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
-
-
-Cleanup
--------
-
-::
-
-    >>> import shutil
-    >>> shutil.rmtree(TEMPDIR)
+from pkg_resources import resource_filename
+from usbid import Bus
+from usbid import Interface
+from usbid import Port
+from usbid import USB
+from usbid.fs import Container
+from usbid.fs import FileAttributes
+import doctest
+import os
+import shutil
+import sys
+import tarfile
+import tempfile
+import unittest
+
+
+def get_file_attribues(obj):
+    ret = []
+    for attr_name in obj.__file_attributes__:
+        ret.append((attr_name, getattr(obj, attr_name)))
+    return ret
+
+
+class Example(object):
+
+    def __init__(self, want):  # pragma: no cover
+        self.want = want + '\n'
+
+
+class Failure(Exception):
+    pass
+
+
+class TestUsbid(unittest.TestCase):
+
+    def __init__(self, *args, **kw):
+        unittest.TestCase.__init__(self, *args, **kw)
+        self._checker = doctest.OutputChecker()
+        self._optionflags = (
+            doctest.NORMALIZE_WHITESPACE |
+            doctest.ELLIPSIS |
+            doctest.REPORT_ONLY_FIRST_FAILURE
+        )
+
+    def checkOutput(self, want, got, optionflags=None):
+        if optionflags is None:
+            optionflags = self._optionflags
+        success = self._checker.check_output(want, got, optionflags)
+        if not success:  # pragma: no cover
+            raise Failure(self._checker.output_difference(
+                Example(want),
+                got, optionflags
+            ))
+
+    @classmethod
+    def setUpClass(cls):
+        test_data_1 = resource_filename(__name__, 'testing/1.tgz')
+        test_data_2 = resource_filename(__name__, 'testing/2.tgz')
+        test_data_3 = resource_filename(__name__, 'testing/3.tgz')
+
+        cls.tempdir = tempfile.mkdtemp()
+
+        test_data_1_dir = os.path.join(cls.tempdir, '1')
+        tgz = tarfile.open(test_data_1)
+        tgz.extractall(test_data_1_dir)
+
+        test_data_2_dir = os.path.join(cls.tempdir, '2')
+        tgz = tarfile.open(test_data_2)
+        tgz.extractall(test_data_2_dir)
+
+        test_data_3_dir = os.path.join(cls.tempdir, '3')
+        tgz = tarfile.open(test_data_3)
+        tgz.extractall(test_data_3_dir)
+
+    @classmethod
+    def tearDownClass(cls):
+        shutil.rmtree(cls.tempdir)
+
+    def test_Container(self):
+        container = Container()
+        with self.assertRaises(NotImplementedError):
+            container.keys()
+        with self.assertRaises(NotImplementedError):
+            container['key']
+
+        class TestContainer(Container):
+            def __iter__(self):
+                return iter(['1', '2'])
+            def __getitem__(self, key):
+                return key
+
+        test_container = TestContainer()
+        self.assertEqual(test_container.keys(), ['1', '2'])
+        self.assertEqual(test_container['1'], '1')
+
+    def test_FileAttributes(self):
+        with open(os.path.join(self.tempdir, 'file_attribute'), 'wt') as file:
+            file.write('File attribute value')
+
+        class TestFileAttributes(FileAttributes):
+            __file_attributes__ = ['file_attribute']
+            fs_path = self.tempdir
+            class_attribute = 'Class Attribute'
+
+        test_file_attributes = TestFileAttributes()
+        self.assertEqual(
+            test_file_attributes.class_attribute,
+            'Class Attribute'
+        )
+        self.assertEqual(
+            test_file_attributes.file_attribute,
+            'File attribute value'
+        )
+        with self.assertRaises(AttributeError):
+            test_file_attributes.no_attribute
+
+        self.assertEqual(
+            get_file_attribues(test_file_attributes),
+            [('file_attribute', 'File attribute value')]
+        )
+
+    def test_USB(self):
+        test_data_1_dir = os.path.join(
+            self.tempdir, '1', 'sys', 'bus', 'usb', 'devices'
+        )
+
+        usb = USB(fs_path=test_data_1_dir)
+        self.checkOutput(
+            '<usbid.fs.USB [/.../1/sys/bus/usb/devices] at ...>',
+            str(usb)
+        )
+        self.checkOutput('.../1/sys/bus/usb/devices', usb.fs_path)
+        self.assertEqual(usb.fs_name, 'devices')
+        self.checkOutput('.../1/sys/bus/usb', usb.fs_parent)
+        self.assertEqual(sorted(usb.keys()), ['1', '2', '3', '4'])
+        with self.assertRaises(KeyError):
+            usb['0']
+        self.checkOutput('<usbid.fs.Bus [usb1] at ...>', str(usb['1']))
+
+        self.checkOutput("""
+        [<usbid.fs.Bus [usb1] at ...>,
+        <usbid.fs.Bus [usb2] at ...>,
+        <usbid.fs.Bus [usb3] at ...>,
+        <usbid.fs.Bus [usb4] at ...>]
+        """, str(sorted(usb.values(), key=lambda x: x.fs_name)))
+
+        self.checkOutput("""
+        [('1', <usbid.fs.Bus [usb1] at ...>),
+        ('2', <usbid.fs.Bus [usb2] at ...>),
+        ('3', <usbid.fs.Bus [usb3] at ...>),
+        ('4', <usbid.fs.Bus [usb4] at ...>)]
+        """, str(sorted(usb.items())))
+
+        MARKER = object()
+        self.assertTrue(usb.get('0', default=MARKER) is MARKER)
+        self.assertFalse(usb.get('1', default=MARKER) is MARKER)
+
+    def test_Bus(self):
+        with self.assertRaises(ValueError) as arc:
+            Bus(name=None, parent=None, fs_path='inexistent')
+        self.assertEqual(str(arc.exception), 'Invalid path given')
+
+        test_data_1_dir = os.path.join(
+            self.tempdir, '1', 'sys', 'bus', 'usb', 'devices'
+        )
+
+        bus = USB(fs_path=test_data_1_dir)['3']
+        self.checkOutput('<usbid.fs.Bus [usb3] at ...>', str(bus))
+        self.assertEqual(bus.name, '3')
+        self.assertEqual(sorted(bus.keys()), ['2', '4'])
+        with self.assertRaises(KeyError):
+            bus['1']
+        self.checkOutput('<usbid.fs.Port [3-2] at ...>', str(bus['2']))
+
+        self.checkOutput("""
+        [<usbid.fs.Port [3-2] at ...>,
+        <usbid.fs.Port [3-4] at ...>]
+        """, str(sorted(bus.values(), key=lambda x: x.name)))
+
+        self.checkOutput("""
+        [('2', <usbid.fs.Port [3-2] at ...>),
+        ('4', <usbid.fs.Port [3-4] at ...>)]
+        """, str(sorted(bus.items(), key=lambda x: x[0])))
+
+        self.assertEqual(get_file_attribues(bus), [
+            ('authorized', '1'),
+            ('authorized_default', '1'),
+            ('avoid_reset_quirk', '0'),
+            ('bcdDevice', '0313'),
+            ('bConfigurationValue', '1'),
+            ('bDeviceClass', '09'),
+            ('bDeviceProtocol', '01'),
+            ('bDeviceSubClass', '00'),
+            ('bmAttributes', 'e0'),
+            ('bMaxPacketSize0', '64'),
+            ('bMaxPower', '0mA'),
+            ('bNumConfigurations', '1'),
+            ('bNumInterfaces', '1'),
+            ('busnum', '3'),
+            ('dev', '189:256'),
+            ('devnum', '1'),
+            ('devpath', '0'),
+            ('idProduct', '0002'),
+            ('idVendor', '1d6b'),
+            ('ltm_capable', 'no'),
+            ('manufacturer', 'Linux 3.13.0-48-generic xhci_hcd'),
+            ('maxchild', '4'),
+            ('product', 'xHCI Host Controller'),
+            ('quirks', '0x0'),
+            ('removable', 'unknown'),
+            ('serial', '0000:00:14.0'),
+            ('speed', '480'),
+            ('uevent', 'MAJOR=189\nMINOR=256\nDEVNAME=bus/usb/003/001\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=1d6b/2/313\nTYPE=9/0/1\nBUSNUM=003\nDEVNUM=001'),
+            ('urbnum', '884'),
+            ('version', '2.00')
+        ])
+
+        self.checkOutput('[<usbid.fs.Interface [3-0:1.0] at ...>]', str(bus.interfaces))
+        interface = bus.interfaces[0]
+        self.assertEqual(get_file_attribues(interface), [
+            ('bAlternateSetting', '0'),
+            ('bInterfaceClass', '09'),
+            ('bInterfaceNumber', '00'),
+            ('bInterfaceProtocol', '00'),
+            ('bInterfaceSubClass', '00'),
+            ('bNumEndpoints', '01'),
+            ('interface', None),
+            ('modalias', 'usb:v1D6Bp0002d0313dc09dsc00dp01ic09isc00ip00in00'),
+            ('supports_autosuspend', '1'),
+            ('uevent', 'DEVTYPE=usb_interface\nDRIVER=hub\nPRODUCT=1d6b/2/313\nTYPE=9/0/1\nINTERFACE=9/0/0\nMODALIAS=usb:v1D6Bp0002d0313dc09dsc00dp01ic09isc00ip00in00')
+        ])
+
+    def test_Port(self):
+        with self.assertRaises(ValueError) as arc:
+            Port(name=None, parent=None, fs_path='inexistent')
+        self.assertEqual(str(arc.exception), 'Invalid path given')
+
+        test_data_1_dir = os.path.join(
+            self.tempdir, '1', 'sys', 'bus', 'usb', 'devices'
+        )
+        port = USB(fs_path=test_data_1_dir)['3']['2']
+
+        self.checkOutput('<usbid.fs.Port [3-2] at ...>', str(port))
+        self.checkOutput('.../1/sys/bus/usb/devices/usb3/3-2', str(port.fs_path))
+        self.assertEqual(port.fs_name, '3-2')
+
+        self.assertEqual(get_file_attribues(port), [
+            ('authorized', '1'),
+            ('avoid_reset_quirk', '0'),
+            ('bcdDevice', '0100'),
+            ('bConfigurationValue', '1'),
+            ('bDeviceClass', '09'),
+            ('bDeviceProtocol', '01'),
+            ('bDeviceSubClass', '00'),
+            ('bmAttributes', 'e0'),
+            ('bMaxPacketSize0', '64'),
+            ('bMaxPower', '100mA'),
+            ('bNumConfigurations', '1'),
+            ('bNumInterfaces', '1'),
+            ('busnum', '3'),
+            ('dev', '189:378'),
+            ('devnum', '123'),
+            ('devpath', '2'),
+            ('idProduct', '005a'),
+            ('idVendor', '0409'),
+            ('ltm_capable', 'no'),
+            ('manufacturer', None),
+            ('maxchild', '4'),
+            ('product', None),
+            ('quirks', '0x0'),
+            ('removable', 'removable'),
+            ('serial', None),
+            ('speed', '480'),
+            ('uevent', 'MAJOR=189\nMINOR=378\nDEVNAME=bus/usb/003/123\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=409/5a/100\nTYPE=9/0/1\nBUSNUM=003\nDEVNUM=123'),
+            ('urbnum', '47'),
+            ('version', '2.00')
+        ])
+
+        self.checkOutput(
+            '[<usbid.fs.Interface [3-2:1.0] at ...>]',
+            str(port.interfaces)
+        )
+        interface = port.interfaces[0]
+        self.assertEqual(get_file_attribues(interface), [
+            ('bAlternateSetting', '0'),
+            ('bInterfaceClass', '09'),
+            ('bInterfaceNumber', '00'),
+            ('bInterfaceProtocol', '00'),
+            ('bInterfaceSubClass', '00'),
+            ('bNumEndpoints', '01'),
+            ('interface', None),
+            ('modalias', 'usb:v0409p005Ad0100dc09dsc00dp01ic09isc00ip00in00'),
+            ('supports_autosuspend', '1'),
+            ('uevent', 'DEVTYPE=usb_interface\nDRIVER=hub\nPRODUCT=409/5a/100\nTYPE=9/0/1\nINTERFACE=9/0/0\nMODALIAS=usb:v0409p005Ad0100dc09dsc00dp01ic09isc00ip00in00')
+        ])
+        self.assertEqual(sorted(port.keys()), ['1', '2', '3', '4'])
+
+        with self.assertRaises(KeyError):
+            port['0']
+
+        sub_port = port['1']
+        self.checkOutput('<usbid.fs.Port [3-2.1] at ...>', str(sub_port))
+        self.checkOutput(
+            '.../1/sys/bus/usb/devices/usb3/3-2/3-2.1',
+            str(sub_port.fs_path)
+        )
+        self.assertEqual(sub_port.fs_name, '3-2.1')
+
+        self.assertEqual(get_file_attribues(sub_port), [
+            ('authorized', '1'),
+            ('avoid_reset_quirk', '0'),
+            ('bcdDevice', '0600'),
+            ('bConfigurationValue', '1'),
+            ('bDeviceClass', '00'),
+            ('bDeviceProtocol', '00'),
+            ('bDeviceSubClass', '00'),
+            ('bmAttributes', 'a0'),
+            ('bMaxPacketSize0', '8'),
+            ('bMaxPower', '90mA'),
+            ('bNumConfigurations', '1'),
+            ('bNumInterfaces', '1'),
+            ('busnum', '3'),
+            ('dev', '189:379'),
+            ('devnum', '124'),
+            ('devpath', '2.1'),
+            ('idProduct', '6001'),
+            ('idVendor', '0403'),
+            ('ltm_capable', 'no'),
+            ('manufacturer', 'FTDI'),
+            ('maxchild', '0'),
+            ('product', 'FT232R USB UART'),
+            ('quirks', '0x0'),
+            ('removable', 'unknown'),
+            ('serial', 'A7022OOQ'),
+            ('speed', '12'),
+            ('uevent', 'MAJOR=189\nMINOR=379\nDEVNAME=bus/usb/003/124\nDEVTYPE=usb_device\nDRIVER=usb\nPRODUCT=403/6001/600\nTYPE=0/0/0\nBUSNUM=003\nDEVNUM=124'),
+            ('urbnum', '15'),
+            ('version', '2.00')
+        ])
+
+        self.checkOutput(
+            '[<usbid.fs.Interface [3-2.1:1.0] at ...>]',
+            str(sub_port.interfaces)
+        )
+        interface = sub_port.interfaces[0]
+        self.assertEqual(get_file_attribues(interface), [
+            ('bAlternateSetting', '0'),
+            ('bInterfaceClass', 'ff'),
+            ('bInterfaceNumber', '00'),
+            ('bInterfaceProtocol', 'ff'),
+            ('bInterfaceSubClass', 'ff'),
+            ('bNumEndpoints', '02'),
+            ('interface', 'FT232R USB UART'),
+            ('modalias', 'usb:v0403p6001d0600dc00dsc00dp00icFFiscFFipFFin00'),
+            ('supports_autosuspend', '1'),
+            ('uevent', 'DEVTYPE=usb_interface\nDRIVER=ftdi_sio\nPRODUCT=403/6001/600\nTYPE=0/0/0\nINTERFACE=255/255/255\nMODALIAS=usb:v0403p6001d0600dc00dsc00dp00icFFiscFFipFFin00')
+        ])
+
+    def test_Interface(self):
+        with self.assertRaises(ValueError) as arc:
+            Interface(parent=None, fs_path='inexistent')
+        self.assertEqual(str(arc.exception), 'Invalid path given')
+
+        test_data_1_dir = os.path.join(
+            self.tempdir, '1', 'sys', 'bus', 'usb', 'devices'
+        )
+        usb = USB(fs_path=test_data_1_dir)
+        port = usb['3']['2']['1']
+        self.checkOutput(
+            '[<usbid.fs.Interface [3-2.1:1.0] at ...>]',
+            str(port.interfaces)
+        )
+
+        interface = port.interfaces[0]
+        self.checkOutput(
+            '<usbid.fs.Port [3-2.1] at ...>',
+            str(interface.parent)
+        )
+        self.assertEqual(interface.fs_name, '3-2.1:1.0')
+        self.assertEqual(interface.manufacturer, 'FTDI')
+        self.assertEqual(interface.product, 'FT232R USB UART')
+
+        interface = usb.get_interface(interface.fs_name)
+        self.checkOutput(
+            '<usbid.fs.Interface [3-2.1:1.0] at ...>',
+            str(interface)
+        )
+        self.checkOutput(
+            '<usbid.fs.Port [3-2.1] at ...>',
+            str(interface.parent)
+        )
+        self.assertEqual(interface.manufacturer, 'FTDI')
+        self.assertEqual(interface.product, 'FT232R USB UART')
+
+    def test_data_tree_1(self):
+        test_data_1_dir = os.path.join(
+            self.tempdir, '1', 'sys', 'bus', 'usb', 'devices'
+        )
+        usb = USB(fs_path=test_data_1_dir)
+
+        self.checkOutput("""
+        <usbid.fs.USB [/.../1/sys/bus/usb/devices] at ...>
+        __<usbid.fs.Bus [usb1] at ...>
+        ______- Linux 3.13.0-48-generic ehci_hcd
+        ______- EHCI Host Controller
+        ____<usbid.fs.Interface [1-0:1.0] at ...>
+        ____<usbid.fs.Port [1-1] at ...>
+        ______<usbid.fs.Interface [1-1:1.0] at ...>
+        ______<usbid.fs.Port [1-1.2] at ...>
+        __________- USB Optical Mouse
+        ________<usbid.fs.Interface [1-1.2:1.0] at ...>
+        ______<usbid.fs.Port [1-1.3] at ...>
+        __________- Auth
+        __________- Biometric Coprocessor
+        ________<usbid.fs.Interface [1-1.3:1.0] at ...>
+        ______<usbid.fs.Port [1-1.4] at ...>
+        __________- Broadcom Corp
+        __________- BCM20702A0
+        ________<usbid.fs.Interface [1-1.4:1.0] at ...>
+        ________<usbid.fs.Interface [1-1.4:1.1] at ...>
+        ________<usbid.fs.Interface [1-1.4:1.2] at ...>
+        ________<usbid.fs.Interface [1-1.4:1.3] at ...>
+        ______<usbid.fs.Port [1-1.6] at ...>
+        __________- SunplusIT INC.
+        __________- Integrated Camera
+        ________<usbid.fs.Interface [1-1.6:1.0] at ...>
+        ________<usbid.fs.Interface [1-1.6:1.1] at ...>
+        __<usbid.fs.Bus [usb2] at ...>
+        ______- Linux 3.13.0-48-generic ehci_hcd
+        ______- EHCI Host Controller
+        ____<usbid.fs.Interface [2-0:1.0] at ...>
+        ____<usbid.fs.Port [2-1] at ...>
+        ______<usbid.fs.Interface [2-1:1.0] at ...>
+        __<usbid.fs.Bus [usb3] at ...>
+        ______- Linux 3.13.0-48-generic xhci_hcd
+        ______- xHCI Host Controller
+        ____<usbid.fs.Interface [3-0:1.0] at ...>
+        ____<usbid.fs.Port [3-2] at ...>
+        ______<usbid.fs.Interface [3-2:1.0] at ...>
+        ______<usbid.fs.Port [3-2.1] at ...>
+        __________- FTDI
+        __________- FT232R USB UART
+        ________<usbid.fs.Interface [3-2.1:1.0] at ...>
+        __________- ttyUSB0
+        ______<usbid.fs.Port [3-2.2] at ...>
+        __________- FTDI
+        __________- FT232R USB UART
+        ________<usbid.fs.Interface [3-2.2:1.0] at ...>
+        __________- ttyUSB1
+        ______<usbid.fs.Port [3-2.3] at ...>
+        __________- FTDI
+        __________- FT232R USB UART
+        ________<usbid.fs.Interface [3-2.3:1.0] at ...>
+        __________- ttyUSB2
+        ______<usbid.fs.Port [3-2.4] at ...>
+        __________- FTDI
+        __________- FT232R USB UART
+        ________<usbid.fs.Interface [3-2.4:1.0] at ...>
+        __________- ttyUSB3
+        ____<usbid.fs.Port [3-4] at ...>
+        ________- Lenovo
+        ________- H5321 gw
+        ______<usbid.fs.Interface [3-4:1.0] at ...>
+        ______<usbid.fs.Interface [3-4:1.1] at ...>
+        ________- ttyACM0
+        ______<usbid.fs.Interface [3-4:1.2] at ...>
+        ______<usbid.fs.Interface [3-4:1.3] at ...>
+        ________- ttyACM1
+        ______<usbid.fs.Interface [3-4:1.4] at ...>
+        ______<usbid.fs.Interface [3-4:1.5] at ...>
+        ______<usbid.fs.Interface [3-4:1.6] at ...>
+        ______<usbid.fs.Interface [3-4:1.7] at ...>
+        ______<usbid.fs.Interface [3-4:1.8] at ...>
+        ______<usbid.fs.Interface [3-4:1.9] at ...>
+        ________- ttyACM2
+        __<usbid.fs.Bus [usb4] at ...>
+        ______- Linux 3.13.0-48-generic xhci_hcd
+        ______- xHCI Host Controller
+        ____<usbid.fs.Interface [4-0:1.0] at ...>
+        """, usb.treerepr(prefix='_'))
+
+        self.checkOutput("""
+        [<usbid.fs.Interface [1-0:1.0] at ...>,
+        <usbid.fs.Interface [1-1.2:1.0] at ...>,
+        <usbid.fs.Interface [1-1.3:1.0] at ...>,
+        <usbid.fs.Interface [1-1.4:1.0] at ...>,
+        <usbid.fs.Interface [1-1.4:1.1] at ...>,
+        <usbid.fs.Interface [1-1.4:1.2] at ...>,
+        <usbid.fs.Interface [1-1.4:1.3] at ...>,
+        <usbid.fs.Interface [1-1.6:1.0] at ...>,
+        <usbid.fs.Interface [1-1.6:1.1] at ...>,
+        <usbid.fs.Interface [1-1:1.0] at ...>,
+        <usbid.fs.Interface [2-0:1.0] at ...>,
+        <usbid.fs.Interface [2-1:1.0] at ...>,
+        <usbid.fs.Interface [3-0:1.0] at ...>,
+        <usbid.fs.Interface [3-2.1:1.0] at ...>,
+        <usbid.fs.Interface [3-2.2:1.0] at ...>,
+        <usbid.fs.Interface [3-2.3:1.0] at ...>,
+        <usbid.fs.Interface [3-2.4:1.0] at ...>,
+        <usbid.fs.Interface [3-2:1.0] at ...>,
+        <usbid.fs.Interface [3-4:1.0] at ...>,
+        <usbid.fs.Interface [3-4:1.1] at ...>,
+        <usbid.fs.Interface [3-4:1.2] at ...>,
+        <usbid.fs.Interface [3-4:1.3] at ...>,
+        <usbid.fs.Interface [3-4:1.4] at ...>,
+        <usbid.fs.Interface [3-4:1.5] at ...>,
+        <usbid.fs.Interface [3-4:1.6] at ...>,
+        <usbid.fs.Interface [3-4:1.7] at ...>,
+        <usbid.fs.Interface [3-4:1.8] at ...>,
+        <usbid.fs.Interface [3-4:1.9] at ...>,
+        <usbid.fs.Interface [4-0:1.0] at ...>]
+        """, str(sorted(usb.aggregated_interfaces(), key=lambda x: x.fs_path)))
+
+        tty_ifaces = sorted(
+            usb.aggregated_interfaces(tty=True),
+            key=lambda x: x.fs_path
+        )
+        self.checkOutput("""
+        ['/.../1/sys/bus/usb/devices/usb3/3-2/3-2.1/3-2.1:1.0 - ttyUSB0',
+        '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.2/3-2.2:1.0 - ttyUSB1',
+        '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.3/3-2.3:1.0 - ttyUSB2',
+        '/.../1/sys/bus/usb/devices/usb3/3-2/3-2.4/3-2.4:1.0 - ttyUSB3',
+        '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0',
+        '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1',
+        '/.../1/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
+        """, str(['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]))
+
+    def test_data_tree_2(self):
+        test_data_2_dir = os.path.join(
+            self.tempdir, '2', 'sys', 'bus', 'usb', 'devices'
+        )
+        usb = USB(fs_path=test_data_2_dir)
+
+        self.checkOutput("""
+        <usbid.fs.USB [/.../2/sys/bus/usb/devices] at ...>
+        ...
+        __<usbid.fs.Bus [usb3] at ...>
+        ______- Linux 3.13.0-48-generic xhci_hcd
+        ______- xHCI Host Controller
+        ____<usbid.fs.Interface [3-0:1.0] at ...>
+        ____<usbid.fs.Port [3-2] at ...>
+        ________- FTDI
+        ________- USB <-> Serial Cable
+        ______<usbid.fs.Interface [3-2:1.0] at ...>
+        ________- ttyUSB0
+        ______<usbid.fs.Interface [3-2:1.1] at ...>
+        ________- ttyUSB1
+        ...
+        """, usb.treerepr(prefix='_'))
+
+        tty_ifaces = sorted(
+            usb.aggregated_interfaces(tty=True),
+            key=lambda x: x.fs_path
+        )
+        self.checkOutput("""
+        ['.../2/sys/bus/usb/devices/usb3/3-2/3-2:1.0 - ttyUSB0',
+        '/.../2/sys/bus/usb/devices/usb3/3-2/3-2:1.1 - ttyUSB1',
+        '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0',
+        '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1',
+        '/.../2/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
+        """, str(['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]))
+
+    def test_data_tree_3(self):
+        test_data_3_dir = os.path.join(
+            self.tempdir, '3', 'sys', 'bus', 'usb', 'devices'
+        )
+        usb = USB(fs_path=test_data_3_dir)
+
+        self.checkOutput("""
+        <usbid.fs.USB [/.../3/sys/bus/usb/devices] at ...>
+        __<usbid.fs.Bus [usb3] at ...>
+        ______- Linux 3.13.0-48-generic xhci_hcd
+        ______- xHCI Host Controller
+        ____<usbid.fs.Interface [3-0:1.0] at ...>
+        ____<usbid.fs.Port [3-2] at ...>
+        ______<usbid.fs.Interface [3-2:1.0] at ...>
+        ______<usbid.fs.Port [3-2.2] at ...>
+        __________- DMX4ALL
+        __________- NanoDMX Interface
+        ________<usbid.fs.Interface [3-2.2:1.0] at ...>
+        __________- ttyACM3
+        ________<usbid.fs.Interface [3-2.2:1.1] at ...>
+        ______<usbid.fs.Port [3-2.4] at ...>
+        __________- Prolific Technology Inc.
+        __________- USB-Serial Controller D
+        ________<usbid.fs.Interface [3-2.4:1.0] at ...>
+        __________- ttyUSB0
+        ______<usbid.fs.Port [3-2.6] at ...>
+        ________<usbid.fs.Interface [3-2.6:1.0] at ...>
+        ________<usbid.fs.Port [3-2.6.1] at ...>
+        ____________- FTDI
+        ____________- FT232R USB UART
+        __________<usbid.fs.Interface [3-2.6.1:1.0] at ...>
+        ____________- ttyUSB3
+        ________<usbid.fs.Port [3-2.6.2] at ...>
+        ____________- FTDI
+        ____________- FT232R USB UART
+        __________<usbid.fs.Interface [3-2.6.2:1.0] at ...>
+        ____________- ttyUSB4
+        ________<usbid.fs.Port [3-2.6.3] at ...>
+        ____________- FTDI
+        ____________- FT232R USB UART
+        __________<usbid.fs.Interface [3-2.6.3:1.0] at ...>
+        ____________- ttyUSB5
+        ________<usbid.fs.Port [3-2.6.4] at ...>
+        ____________- FTDI
+        ____________- FT232R USB UART
+        __________<usbid.fs.Interface [3-2.6.4:1.0] at ...>
+        ____________- ttyUSB6
+        ______<usbid.fs.Port [3-2.7] at ...>
+        __________- FTDI
+        __________- USB <-> Serial Cable
+        ________<usbid.fs.Interface [3-2.7:1.0] at ...>
+        __________- ttyUSB1
+        ________<usbid.fs.Interface [3-2.7:1.1] at ...>
+        __________- ttyUSB2
+        ...
+        """, usb.treerepr(prefix='_'))
+
+        tty_ifaces = sorted(
+            usb.aggregated_interfaces(tty=True),
+            key=lambda x: x.fs_path
+        )
+        self.checkOutput("""
+        ['/.../3/sys/bus/usb/devices/usb3/3-2/3-2.2/3-2.2:1.0 - ttyACM3',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.4/3-2.4:1.0 - ttyUSB0',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.1/3-2.6.1:1.0 - ttyUSB3',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.2/3-2.6.2:1.0 - ttyUSB4',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.3/3-2.6.3:1.0 - ttyUSB5',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.6/3-2.6.4/3-2.6.4:1.0 - ttyUSB6',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.7/3-2.7:1.0 - ttyUSB1',
+        '/.../3/sys/bus/usb/devices/usb3/3-2/3-2.7/3-2.7:1.1 - ttyUSB2',
+        '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.1 - ttyACM0',
+        '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.3 - ttyACM1',
+        '/.../3/sys/bus/usb/devices/usb3/3-4/3-4:1.9 - ttyACM2']
+        """, str(['{0} - {1}'.format(iface.fs_path, iface.tty) for iface in tty_ifaces]))
+
+
+if __name__ == '__main__':
+    from usbid import tests
+
+    suite = unittest.TestSuite()
+    suite.addTest(unittest.findTestCases(tests))
+    runner = unittest.TextTestRunner(failfast=True)
+    result = runner.run(suite)
+    sys.exit(not result.wasSuccessful())
```

### Comparing `usbid-2.1/src/usbid/fs.py` & `usbid-2.2/src/usbid/fs.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 IS_BUS = re.compile("^usb\d$")
 IS_BUS_PORT = re.compile("^\d-\d$")
 IS_SUB_PORT = re.compile("^\d-\d(\.\d)*$")
 IS_INTERFACE = re.compile("^\d-\d(\.\d)*:\d.\d$")
 
 
 class Container(object):
-    """Mixin for container objects.
-    """
+    """Mixin for container objects."""
     name = None
     parent = None
 
     def keys(self):
         return list(self.__iter__())
 
     def values(self):
@@ -35,16 +34,15 @@
         raise NotImplementedError()
 
     def __getitem__(self, key):
         raise NotImplementedError()
 
 
 class FSLocation(object):
-    """Mixin for objects with a file system location.
-    """
+    """Mixin for objects with a file system location."""
     fs_path = None
 
     @property
     def fs_name(self):
         if self.fs_path.find(os.path.sep) > -1:
             return self.fs_path[self.fs_path.rfind(os.path.sep) + 1:]
 
@@ -68,60 +66,61 @@
                     return file.read().strip('\n').strip()
             except IOError:
                 return None
         return object.__getattribute__(self, name)
 
 
 class ReprMixin(object):
-    """Mixin for objects inside the USB filesystem tree for debugging.
-    """
+    """Mixin for objects inside the USB filesystem tree for debugging."""
 
     def __repr__(self):
         return '<{0}.{1} [{2}] at {3}>'.format(
             self.__module__,
             self.__class__.__name__,
             self.fs_name,
             id(self)
         )
 
-    def printtree(self, indent=0):
-        print('{0}{1}'.format(indent * ' ', repr(self)))
+    def treerepr(self, indent=0, prefix=' '):
+        res = '{0}{1}\n'.format(indent * prefix, repr(self))
         manufacturer = getattr(self, 'manufacturer', None)
         if manufacturer is not None:
-            print('{0}- {1}'.format((indent + 4) * ' ', manufacturer))
+            res += '{0}- {1}\n'.format((indent + 4) * prefix, manufacturer)
         product = getattr(self, 'product', None)
         if product is not None:
-            print('{0}- {1}'.format((indent + 4) * ' ', product))
+            res += '{0}- {1}\n'.format((indent + 4) * prefix, product)
         if isinstance(self, InterfaceProvider):
             for iface in sorted(self.interfaces, key=lambda x: x.fs_name):
-                print('{0}{1}'.format((indent + 2) * ' ', repr(iface)))
+                res += '{0}{1}\n'.format((indent + 2) * prefix, repr(iface))
                 tty = iface.tty
                 if tty:
-                    print('{0}- {1}'.format((indent + 4) * ' ', tty))
+                    res += '{0}- {1}\n'.format((indent + 4) * prefix, tty)
         for node in sorted(self.values(), key=lambda x: x.fs_name):
-            node.printtree(indent + 2)
+            res += node.treerepr(indent + 2, prefix)
+        return res
+
+    def printtree(self):  # pragma: no cover
+        print(self.treerepr())
 
 
 class InterfaceProvider(Container, FSLocation):
-    """Mixin for objects providing USB interfaces.
-    """
+    """Mixin for objects providing USB interfaces."""
 
     @property
     def interfaces(self):
         ifaces = []
         for child in os.listdir(self.fs_path):
             if IS_INTERFACE.match(child):
                 iface_path = os.path.join(self.fs_path, child)
                 ifaces.append(Interface(parent=self, fs_path=iface_path))
         return ifaces
 
 
 class InterfaceAggregator(object):
-    """Mixin for objects providing USB interface aggregation.
-    """
+    """Mixin for objects providing USB interface aggregation."""
 
     def aggregated_interfaces(self, tty=False):
         def aggregate(node, ifaces):
             for child in node.values():
                 if isinstance(child, InterfaceProvider):
                     for iface in child.interfaces:
                         if tty and iface.tty is None:
@@ -130,16 +129,15 @@
                 aggregate(child, ifaces)
         ifaces = []
         aggregate(self, ifaces)
         return ifaces
 
 
 class USB(Container, FSLocation, InterfaceAggregator, ReprMixin):
-    """Object representing USB filsystem root.
-    """
+    """Object representing USB filsystem root."""
 
     def __init__(self, fs_path=USB_FS_ROOT):
         self.fs_path = fs_path
 
     def __iter__(self):
         for child in os.listdir(self.fs_path):
             if IS_BUS.match(child):
@@ -168,16 +166,15 @@
             node = node[port_path.pop()]
         for iface in node.interfaces:
             if iface.fs_name == fs_name:
                 return iface
 
 
 class Bus(FileAttributes, InterfaceProvider, ReprMixin):
-    """Object representing a USB bus.
-    """
+    """Object representing a USB bus."""
     __file_attributes__ = [
         'authorized',
         'authorized_default',
         'avoid_reset_quirk',
         'bcdDevice',
         'bConfigurationValue',
         'bDeviceClass',
@@ -226,16 +223,15 @@
         )
         if not os.path.isdir(port_path):
             raise KeyError(key)
         return Port(name=key, parent=self, fs_path=port_path)
 
 
 class Port(FileAttributes, InterfaceProvider, ReprMixin):
-    """Object representing a USB port.
-    """
+    """Object representing a USB port."""
     __file_attributes__ = [
         'authorized',
         'avoid_reset_quirk',
         'bcdDevice',
         'bConfigurationValue',
         'bDeviceClass',
         'bDeviceProtocol',
@@ -283,16 +279,15 @@
         )
         if not os.path.isdir(port_path):
             raise KeyError(key)
         return Port(name=key, parent=self, fs_path=port_path)
 
 
 class Interface(FileAttributes, ReprMixin):
-    """Object representing a USB interface.
-    """
+    """Object representing a USB interface."""
     __file_attributes__ = [
         'bAlternateSetting',
         'bInterfaceClass',
         'bInterfaceNumber',
         'bInterfaceProtocol',
         'bInterfaceSubClass',
         'bNumEndpoints',
```

### Comparing `usbid-2.1/src/usbid/testing/1.tgz` & `usbid-2.2/src/usbid/testing/1.tgz`

 * *Files identical despite different names*

### Comparing `usbid-2.1/src/usbid/testing/3.tgz` & `usbid-2.2/src/usbid/testing/3.tgz`

 * *Files identical despite different names*

### Comparing `usbid-2.1/src/usbid/testing/2.tgz` & `usbid-2.2/src/usbid/testing/2.tgz`

 * *Files identical despite different names*

### Comparing `usbid-2.1/README.rst` & `usbid-2.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -59,92 +59,81 @@
 
 Usage
 =====
 
 The API consists of a USB root object, from which all children can be accessed
 like python container types.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> from usbid import USB
     >>> usb = USB()
     >>> usb
     <usbid.fs.USB [/sys/bus/usb/devices] at ...>
 
     >>> usb.keys()
     ['1', '2']
 
 Get a specific bus.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> bus = usb['1']
     >>> bus
     <usbid.fs.Bus [usb1] at ...>
 
 Get port from bus.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> port = bus['1']
     >>> port
     <usbid.fs.Port [1-1] at ...>
 
 Get interface from port.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> port.interfaces
     [<usbid.fs.Interface [1-1:1.0] at ...>]
 
 Interfaces might have tty associated.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> port.interfaces[0].tty
     'ttyUSB0'
 
 It's not a good idea to refer to a USB interface by its tty mount name. But
 it's a good idea to remember the file system name for unique identification,
 lookup interface by this name and then connect to corresponding tty.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> interface = usb.get_interface('1-1:1.0')
     >>> interface.tty
     'ttyUSB0'
 
 For debugging you can print the USB structure.
 
-.. code-block:: python
+.. code-block:: pycon
 
     >>> usb.printtree()
     <usbid.fs.USB [/sys/bus/usb/devices] at ...>
       <usbid.fs.Bus [usb1] at ...>
           - Linux 3.13.0-48-generic xhci_hcd
           - xHCI Host Controller
         <usbid.fs.Interface [1-0:1.0] at ...>
         <usbid.fs.Port [1-1] at ...>
             - FTDI
             - FT232R USB UART
           <usbid.fs.Interface [1-1:1.0] at ...>
             - ttyUSB0
 
 
-Coverage report
-===============
-
-::
-
-    lines   cov%   module
-        4   100%   usbid.__init__
-      248   100%   usbid.fs
-       29   100%   usbid.tests
-
-
 Source Code
 ===========
 
 The sources are in a GIT DVCS with its main branches at
 `github <http://github.com/bluedynamics/usbid>`_.
```

