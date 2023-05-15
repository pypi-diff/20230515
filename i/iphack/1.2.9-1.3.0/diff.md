# Comparing `tmp/iphack-1.2.9.tar.gz` & `tmp/iphack-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphack-1.2.9.tar", last modified: Mon Jan 30 09:42:23 2023, max compression
+gzip compressed data, was "iphack-1.3.0.tar", last modified: Mon Jan 30 09:49:20 2023, max compression
```

## Comparing `iphack-1.2.9.tar` & `iphack-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:42:23.500546 iphack-1.2.9/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7251 2023-01-30 09:42:23.500546 iphack-1.2.9/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     5731 2023-01-30 09:40:53.000000 iphack-1.2.9/README.md
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:42:23.496546 iphack-1.2.9/iphack/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.2.9/iphack/__init__.py
--rw-------   0 u0_a314  (10314) u0_a314  (10314)    41855 2023-01-30 09:41:22.000000 iphack-1.2.9/iphack/iphack.py
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:42:23.500546 iphack-1.2.9/iphack.egg-info/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7251 2023-01-30 09:42:23.000000 iphack-1.2.9/iphack.egg-info/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-01-30 09:42:23.000000 iphack-1.2.9/iphack.egg-info/SOURCES.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-01-30 09:42:23.000000 iphack-1.2.9/iphack.egg-info/dependency_links.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       74 2023-01-30 09:42:23.000000 iphack-1.2.9/iphack.egg-info/requires.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-01-30 09:42:23.000000 iphack-1.2.9/iphack.egg-info/top_level.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-01-30 09:42:23.500546 iphack-1.2.9/setup.cfg
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     2305 2023-01-30 09:41:34.000000 iphack-1.2.9/setup.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:49:20.720546 iphack-1.3.0/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7222 2023-01-30 09:49:20.720546 iphack-1.3.0/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     5702 2023-01-30 09:48:18.000000 iphack-1.3.0/README.md
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:49:20.720546 iphack-1.3.0/iphack/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.0/iphack/__init__.py
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)    41855 2023-01-30 09:46:34.000000 iphack-1.3.0/iphack/iphack.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-01-30 09:49:20.720546 iphack-1.3.0/iphack.egg-info/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7222 2023-01-30 09:49:20.000000 iphack-1.3.0/iphack.egg-info/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-01-30 09:49:20.000000 iphack-1.3.0/iphack.egg-info/SOURCES.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-01-30 09:49:20.000000 iphack-1.3.0/iphack.egg-info/dependency_links.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       57 2023-01-30 09:49:20.000000 iphack-1.3.0/iphack.egg-info/requires.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-01-30 09:49:20.000000 iphack-1.3.0/iphack.egg-info/top_level.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-01-30 09:49:20.720546 iphack-1.3.0/setup.cfg
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     2285 2023-01-30 09:46:49.000000 iphack-1.3.0/setup.py
```

### Comparing `iphack-1.2.9/PKG-INFO` & `iphack-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.2.9
+Version: 1.3.0
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -81,15 +81,14 @@
 
 **with manual**
 ```bash
 pip install pyproxify==0.0.1
 pip install ua-headers
 pip install requests
 pip install torpy==1.1.6
-pip install eventlet==0.33.1
 wget --no-check-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh"
 bash install.sh
 ```
 
 ## Usage
 **Ip Address**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.2.9 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.0 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -36,35 +36,35 @@
 (https://github.com/mishakorzik/IpHack/blob/main/LICENSE). ---- ## New Features
 **1) New Functions** - Now you can find out in which country the person is.
 **2) New Desing** - Now a new design has been added and now it is more
 beautiful. **3) More Information** - Now you can learn more about the device
 via IP **4) Detail Information** - You can find out a lot of information about
 IP ----- ## Install **with pip** ```bash pip install iphack ``` **with manual**
 ```bash pip install pyproxify==0.0.1 pip install ua-headers pip install
-requests pip install torpy==1.1.6 pip install eventlet==0.33.1 wget --no-check-
-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/
-install.sh" bash install.sh ``` ## Usage **Ip Address** ```python # ip address
-tracking from iphack import ip ip.address("ip") # domain ip address tracking
-from iphack import ip ip.domain("google.com") # my ip address from iphack
-import ip ip.my() # get proxy from iphack import ip ip.proxy(False) # get proxy
-list for api >>> from iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882',
-'130.41.47.235:8080', '130.41.55.190:8080'] >>> ``` **Check Proxy** ```python #
-check proxy >>> from iphack import check >>> check.proxy("130.41.55.190",
-"8080") Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-
-PLATFORM City : Los Angeles Country : United States Region : California Network
-: 130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+requests pip install torpy==1.1.6 wget --no-check-certificate "https://
+raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
+``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
+ip ip.address("ip") # domain ip address tracking from iphack import ip
+ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
+proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
+iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
+'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
+iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
+#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
+Angeles Country : United States Region : California Network : 130.41.52.0/22
+Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
+iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
+iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
+anonymous request from iphack import inquiry # request from url, using tor &
+fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
+print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
+#method post put = inquiry.put("https://example.com") #method put delete =
+inquiry.delete("https://example.com") #method delete head = inquiry.head
+("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.2.9/README.md` & `iphack-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 
 **with manual**
 ```bash
 pip install pyproxify==0.0.1
 pip install ua-headers
 pip install requests
 pip install torpy==1.1.6
-pip install eventlet==0.33.1
 wget --no-check-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh"
 bash install.sh
 ```
 
 ## Usage
 **Ip Address**
```

#### html2text {}

```diff
@@ -15,35 +15,35 @@
 (https://github.com/mishakorzik/IpHack/blob/main/LICENSE). ---- ## New Features
 **1) New Functions** - Now you can find out in which country the person is.
 **2) New Desing** - Now a new design has been added and now it is more
 beautiful. **3) More Information** - Now you can learn more about the device
 via IP **4) Detail Information** - You can find out a lot of information about
 IP ----- ## Install **with pip** ```bash pip install iphack ``` **with manual**
 ```bash pip install pyproxify==0.0.1 pip install ua-headers pip install
-requests pip install torpy==1.1.6 pip install eventlet==0.33.1 wget --no-check-
-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/
-install.sh" bash install.sh ``` ## Usage **Ip Address** ```python # ip address
-tracking from iphack import ip ip.address("ip") # domain ip address tracking
-from iphack import ip ip.domain("google.com") # my ip address from iphack
-import ip ip.my() # get proxy from iphack import ip ip.proxy(False) # get proxy
-list for api >>> from iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882',
-'130.41.47.235:8080', '130.41.55.190:8080'] >>> ``` **Check Proxy** ```python #
-check proxy >>> from iphack import check >>> check.proxy("130.41.55.190",
-"8080") Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-
-PLATFORM City : Los Angeles Country : United States Region : California Network
-: 130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+requests pip install torpy==1.1.6 wget --no-check-certificate "https://
+raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
+``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
+ip ip.address("ip") # domain ip address tracking from iphack import ip
+ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
+proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
+iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
+'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
+iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
+#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
+Angeles Country : United States Region : California Network : 130.41.52.0/22
+Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
+iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
+iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
+anonymous request from iphack import inquiry # request from url, using tor &
+fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
+print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
+#method post put = inquiry.put("https://example.com") #method put delete =
+inquiry.delete("https://example.com") #method delete head = inquiry.head
+("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.2.9/iphack/iphack.py` & `iphack-1.3.0/iphack/iphack.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 red = '\033[31m'
 yellow = '\033[93m'
 lgreen = '\033[92m'
 clear = '\033[0m'
 bold = '\033[01m'
 cyan = '\033[96m'
-version = "1.2.9"
+version = "1.3.0"
 referer_list = ["https://www.google.com/", "https://www.youtube.com/", "https://www.twitter.com/", "https://www.discord.com/", "https://www.tiktok.com/", "https://www.instagram.com/", "https://check-host.net/", "https://github.com", "https://gitlab.com", "https://he1zen.rf.gd"]
 
 major = str(sys.version_info.major)
 minor = str(sys.version_info.minor)
 path = str(sys.exec_prefix+"/lib/python"+major+"."+minor+"/site-packages/iphack/")
 
 global log
```

### Comparing `iphack-1.2.9/iphack.egg-info/PKG-INFO` & `iphack-1.3.0/iphack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.2.9
+Version: 1.3.0
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
@@ -81,15 +81,14 @@
 
 **with manual**
 ```bash
 pip install pyproxify==0.0.1
 pip install ua-headers
 pip install requests
 pip install torpy==1.1.6
-pip install eventlet==0.33.1
 wget --no-check-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh"
 bash install.sh
 ```
 
 ## Usage
 **Ip Address**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.2.9 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.0 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
@@ -36,35 +36,35 @@
 (https://github.com/mishakorzik/IpHack/blob/main/LICENSE). ---- ## New Features
 **1) New Functions** - Now you can find out in which country the person is.
 **2) New Desing** - Now a new design has been added and now it is more
 beautiful. **3) More Information** - Now you can learn more about the device
 via IP **4) Detail Information** - You can find out a lot of information about
 IP ----- ## Install **with pip** ```bash pip install iphack ``` **with manual**
 ```bash pip install pyproxify==0.0.1 pip install ua-headers pip install
-requests pip install torpy==1.1.6 pip install eventlet==0.33.1 wget --no-check-
-certificate "https://raw.githubusercontent.com/mishakorzik/IpHack/main/
-install.sh" bash install.sh ``` ## Usage **Ip Address** ```python # ip address
-tracking from iphack import ip ip.address("ip") # domain ip address tracking
-from iphack import ip ip.domain("google.com") # my ip address from iphack
-import ip ip.my() # get proxy from iphack import ip ip.proxy(False) # get proxy
-list for api >>> from iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882',
-'130.41.47.235:8080', '130.41.55.190:8080'] >>> ``` **Check Proxy** ```python #
-check proxy >>> from iphack import check >>> check.proxy("130.41.55.190",
-"8080") Proxy : Online #Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-
-PLATFORM City : Los Angeles Country : United States Region : California Network
-: 130.41.52.0/22 Version : IPv4 >>> ``` **Websites** ```python # Check amazon
-subdomains from iphack import ip ip.subdomains("amazon.com") # Check amazon
-directories from iphack import ip ip.directory("amazon.com") ``` **Inquiry**
-```python # anonymous request from iphack import inquiry # request from url,
-using tor & fake user-agent >>> get = inquiry.get("https://api.ipify.org/")
-#method get >>> print(get.text) 199.249.230.102 >>> post = inquiry.post("https:
-//example.com") #method post put = inquiry.put("https://example.com") #method
-put delete = inquiry.delete("https://example.com") #method delete head =
-inquiry.head("https://example.com") #method head # inquiry logs inquiry.debug()
-#enable log inquiry.debug() #disable log # inquiry anon method (default: web)
+requests pip install torpy==1.1.6 wget --no-check-certificate "https://
+raw.githubusercontent.com/mishakorzik/IpHack/main/install.sh" bash install.sh
+``` ## Usage **Ip Address** ```python # ip address tracking from iphack import
+ip ip.address("ip") # domain ip address tracking from iphack import ip
+ip.domain("google.com") # my ip address from iphack import ip ip.my() # get
+proxy from iphack import ip ip.proxy(False) # get proxy list for api >>> from
+iphack import ip >>> ip.proxy(True) ['3.66.38.117:10882', '130.41.47.235:8080',
+'130.41.55.190:8080'] >>> ``` **Check Proxy** ```python # check proxy >>> from
+iphack import check >>> check.proxy("130.41.55.190", "8080") Proxy : Online
+#Online or Offline Asn : AS396982 Org : GOOGLE-CLOUD-PLATFORM City : Los
+Angeles Country : United States Region : California Network : 130.41.52.0/22
+Version : IPv4 >>> ``` **Websites** ```python # Check amazon subdomains from
+iphack import ip ip.subdomains("amazon.com") # Check amazon directories from
+iphack import ip ip.directory("amazon.com") ``` **Inquiry** ```python #
+anonymous request from iphack import inquiry # request from url, using tor &
+fake user-agent >>> get = inquiry.get("https://api.ipify.org/") #method get >>>
+print(get.text) 199.249.230.102 >>> post = inquiry.post("https://example.com")
+#method post put = inquiry.put("https://example.com") #method put delete =
+inquiry.delete("https://example.com") #method delete head = inquiry.head
+("https://example.com") #method head # inquiry logs inquiry.debug() #enable log
+inquiry.debug() #disable log # inquiry anon method (default: web)
 inquiry.rechange("tor") #use tor inquiry.rechange("web") #use web
 inquiry.rechange("vpn") #use vpn ``` ## Screenshot **Repository Views** !
 [Views](https://profile-counter.glitch.me/IpHack/count.svg) **Without logs**
 [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
 IMG_20220822_110928.jpg] **With logs & tor** [https://
 raw.githubusercontent.com/mishakorzik/IpHack/main/IMG_20220824_150950.jpg]
 **With logs & web** [https://raw.githubusercontent.com/mishakorzik/IpHack/main/
```

### Comparing `iphack-1.2.9/setup.py` & `iphack-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iphack',  # should match the package folder
     packages=['iphack'],  # should match the package folder
-    version='1.2.9',  # important for updates
+    version='1.3.0',  # important for updates
     python_requires=">=3.4",
     license='Apache 2.0',  # should match your chosen license
     description='the most ideal tool for finding out information about IP, etc.',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='MishaKorzhik_He1Zen',
     author_email='developer.mishakorzhik@gmail.com',
     url='https://github.com/mishakorzik/IpHack',
     project_urls={  # Optional
         "Bug Tracker": "https://github.com/mishakorzik/IpHack/issues",
         "Sponsor": "https://www.buymeacoffee.com/misakorzik"
     },
-    install_requires=['eventlet==0.33.1', 'ua-headers==0.0.3', 'requests', 'torpy==1.1.6', 'pyproxify==0.0.1'],  # list all packages that your package uses
+    install_requires=['ua-headers==0.0.3', 'requests', 'torpy==1.1.6', 'pyproxify==0.0.1'],  # list all packages that your package uses
     keywords=["ip", "address", "iphack", "ips", "pypi", "pip", "dns", "router", "ipv4", "ipv6", "public", "ip-address", "isp", "location", "lookup", "iplookup", "inquiry", "tor", "anon"],  # descriptive meta-data
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

