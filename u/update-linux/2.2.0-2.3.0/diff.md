# Comparing `tmp/update-linux-2.2.0.tar.gz` & `tmp/update-linux-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-2.2.0.tar", last modified: Sat Apr 29 15:50:51 2023, max compression
+gzip compressed data, was "update-linux-2.3.0.tar", last modified: Mon May 15 09:27:41 2023, max compression
```

## Comparing `update-linux-2.2.0.tar` & `update-linux-2.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-29 15:50:51.417044 update-linux-2.2.0/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-29 15:50:51.000000 update-linux-2.2.0/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-29 15:50:51.417044 update-linux-2.2.0/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.2.0/setup_update_linux.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    18153 2023-04-29 12:17:06.000000 update-linux-2.2.0/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.2.0/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5714 2023-05-15 09:27:41.671724 update-linux-2.3.0/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     5160 2023-05-15 09:27:41.000000 update-linux-2.3.0/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-05-15 09:27:41.671724 update-linux-2.3.0/setup.cfg
+-rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.3.0/setup_update_linux.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    23940 2023-05-14 11:36:13.000000 update-linux-2.3.0/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.3.0/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-05-15 09:27:41.671724 update-linux-2.3.0/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5714 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-05-15 09:27:41.000000 update-linux-2.3.0/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-2.2.0/PKG-INFO` & `update-linux-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.2.0
+Version: 2.3.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,21 @@
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # update-linux command
 
-Command to automate the routine updating of packages and system upgrading for Fedora systems.
+Command to automate the routine updating of packages and system upgrading for Unix systems.
+
+Supports Fedora like and Debian Like OS.
+
+Fedora like includes Fedora, RHEL, Centos, Rocky etc that use DNF.
+
+Debian like includes Dedian, Ubuntu etc that use apt.
 
 update-linux uses ssh to run commands on the hosts being worked.
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
@@ -35,15 +41,17 @@
 $ update-linux host
 ```
 
 For an update the following steps are performed:
 
 1. Update packages  - if there is nothing to update stop here
 
-    `dnf -vy update --refresh`
+    Fedora: `dnf -vy update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-yes`
 
 1. Wait until all systemd jobs have finished
 
     `systemctl list-jobs`
 
     For example akmod building nvidia drivers for a new kernel
 
@@ -59,31 +67,33 @@
 
 ```
 $ update-linux host --check
 ```
 
 With the `--check` options these steps are performed:
 
-1. Check is there are packages to update
+1. Check if there are packages to update
 
-    `dnf check-update --refresh`
+    Fedora: `dnf check-update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-no`
 
 1. Report on state of any failed services
 
     `systemctl --failed`
 
 ## update-linux system-upgrade process
 
 ```
-$ update-linux --system-upgrade=37 host
+$ update-linux --system-upgrade=38 host
 ```
 
 For a system-upgrade update-linux will update one release at a time.
 
-This means that a host running Fedora 35 that is being upgraded to Fedora 37 will first be upgraded to Fedora 36.
+This means that a host running Fedora 36 that is being upgraded to Fedora 38 will first be upgraded to Fedora 37.
 
 This is done as it is the safer then attempting skip over releases that can have required side-effects.
 
 Run the `update-linux --system-upgrade` once for each release that is be upgraded.
 
 For a system-upgrade these steps are used:
 
@@ -180,18 +190,18 @@
 
 Install updates:
 
 ```
 $ update-linux host1 host2
 ```
 
-Apply a system upgrade to Fedota 37:
+Apply a system upgrade to Fedora 38:
 
 ```
-$ update-linux --system-upgrade=37 host3
+$ update-linux --system-upgrade=38 host3
 ```
 
 ## update-linux configuration
 
 The configuration for update-linux is stored in a JSON file.
 
 On linux this is in ~/.config/org.barrys-emacs.update-linux.json and
@@ -203,16 +213,15 @@
 {
     "logdir":   "~/tmpdir",
     "group":
         {
             "all": [
                 "router",
                 "player",
-                "armf36",
-                "armf37"
+                "vm"
                 ],
             "vm": [
                 "armf36",
                 "armf37"
                 ]
         }
 }
```

### Comparing `update-linux-2.2.0/README.md` & `update-linux-2.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # update-linux command
 
-Command to automate the routine updating of packages and system upgrading for Fedora systems.
+Command to automate the routine updating of packages and system upgrading for Unix systems.
+
+Supports Fedora like and Debian Like OS.
+
+Fedora like includes Fedora, RHEL, Centos, Rocky etc that use DNF.
+
+Debian like includes Dedian, Ubuntu etc that use apt.
 
 update-linux uses ssh to run commands on the hosts being worked.
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
@@ -18,15 +24,17 @@
 $ update-linux host
 ```
 
 For an update the following steps are performed:
 
 1. Update packages  - if there is nothing to update stop here
 
-    `dnf -vy update --refresh`
+    Fedora: `dnf -vy update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-yes`
 
 1. Wait until all systemd jobs have finished
 
     `systemctl list-jobs`
 
     For example akmod building nvidia drivers for a new kernel
 
@@ -42,31 +50,33 @@
 
 ```
 $ update-linux host --check
 ```
 
 With the `--check` options these steps are performed:
 
-1. Check is there are packages to update
+1. Check if there are packages to update
 
-    `dnf check-update --refresh`
+    Fedora: `dnf check-update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-no`
 
 1. Report on state of any failed services
 
     `systemctl --failed`
 
 ## update-linux system-upgrade process
 
 ```
-$ update-linux --system-upgrade=37 host
+$ update-linux --system-upgrade=38 host
 ```
 
 For a system-upgrade update-linux will update one release at a time.
 
-This means that a host running Fedora 35 that is being upgraded to Fedora 37 will first be upgraded to Fedora 36.
+This means that a host running Fedora 36 that is being upgraded to Fedora 38 will first be upgraded to Fedora 37.
 
 This is done as it is the safer then attempting skip over releases that can have required side-effects.
 
 Run the `update-linux --system-upgrade` once for each release that is be upgraded.
 
 For a system-upgrade these steps are used:
 
@@ -163,18 +173,18 @@
 
 Install updates:
 
 ```
 $ update-linux host1 host2
 ```
 
-Apply a system upgrade to Fedota 37:
+Apply a system upgrade to Fedora 38:
 
 ```
-$ update-linux --system-upgrade=37 host3
+$ update-linux --system-upgrade=38 host3
 ```
 
 ## update-linux configuration
 
 The configuration for update-linux is stored in a JSON file.
 
 On linux this is in ~/.config/org.barrys-emacs.update-linux.json and
@@ -186,16 +196,15 @@
 {
     "logdir":   "~/tmpdir",
     "group":
         {
             "all": [
                 "router",
                 "player",
-                "armf36",
-                "armf37"
+                "vm"
                 ],
             "vm": [
                 "armf36",
                 "armf37"
                 ]
         }
 }
```

### Comparing `update-linux-2.2.0/setup_update_linux.py` & `update-linux-2.3.0/setup_update_linux.py`

 * *Files identical despite different names*

### Comparing `update-linux-2.2.0/update_linux/__init__.py` & `update-linux-2.3.0/update_linux/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath  # type: ignore
 
-VERSION = '2.2.0'
+VERSION = '2.3.0'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
 
-
 from pathlib import Path
 
 from colour_text import ColourText
 from ssh_wait import ssh_wait
 
 class OptionError(Exception):
     pass
@@ -219,41 +218,65 @@
             t = datetime.datetime.now()
             self.header( 'Update summary %s' % (t.strftime( '%Y-%m-%d %H:%M:%S' ),) )
 
             for host in self.all_hosts:
                 if host in all_to_exclude:
                     continue
 
+                os_plugin_type, os_id = self.detectOperatingSystem( host )
+                if os_plugin_type is None:
+                    if os_id is not None:
+                        self.warn( host, 'Unsupported OS type %s' % (os_id,) )
+                    continue
+
+                self.info( host, 'OS is %s. Using OS plugin %s' % (os_id, os_plugin_type) )
+
+                plugin = os_id_to_plugin[ os_plugin_type ]( self )
+
                 self.flushDns()
                 if self.opt_check:
-                    self.check( host )
+                    plugin.check( host,
+                        check_log_name=self.logdir / ('check-update-%s-%s.log' % (host, self.ts)) )
 
                 elif self.opt_install_package() is not None:
-                    self.installPackage( host, self.opt_install_package )
+                    self.installPackage( host, self.opt_install_package,
+                        update_log_name=self.logdir / ('install-%s-%s.log' % (host, self.ts)) )
 
                 else:
                     if self.isThisHost( host ):
                         self.warn( host, 'Refusing to update this host' )
 
                     elif self.opt_system_upgrade:
-                        self.systemUpgrade( host, self.opt_system_upgrade )
+                        plugin.systemUpgrade( host, self.opt_system_upgrade,
+                            upgrade_log_name=self.logdir / ('upgrade-%s-%s.log' % (host, self.ts)) )
 
                     else:
-                        self.update( host )
+                        plugin.update( host,
+                            update_log_name=self.logdir / ('update-%s-%s.log' % (host, self.ts)),
+                            status_log_name=self.logdir / ('status-%s-%s.log' % (host, self.ts)) )
 
         print( '-' * 60 )
         for line in self.all_summary_lines:
             print( line )
 
         return 0
 
-    def hostIter( self, groups_or_hosts ):
-        for group_or_host in groups_or_hosts:
+    def hostIter( self, all_groups_or_hosts, _handled=None ):
+        if _handled is None:
+            _handled = set()
+
+        for group_or_host in all_groups_or_hosts:
+            # deal with recursive groups and duplicate host
+            # by ignoring them
+            if group_or_host in _handled:
+                continue
+
+            _handled.add( group_or_host )
             if group_or_host in self.all_groups:
-                yield from self.hostIter( self.all_groups[ group_or_host ] )
+                yield from self.hostIter( self.all_groups[ group_or_host ], _handled )
 
             else:
                 yield group_or_host
 
     def isThisHost( self, other_host ):
         this_host = socket.gethostname()
         this_info = socket.getaddrinfo( this_host, 'ssh', proto=socket.IPPROTO_TCP )
@@ -314,111 +337,45 @@
             return
 
         # mac often needs its DNS cache flushing as it will
         # not notice newly booted hosts
         cmd = ['sudo', 'killall', '-HUP', 'mDNSResponder']
         self.runAndLog( None, cmd, log=False )
 
-    def check( self, host ):
+    def detectOperatingSystem( self, host ):
         rc = ssh_wait( host, wait=False, log_fn=None )
         if rc != 0:
             self.warn( host, 'Is not reachable' )
-            return
-
-        check_log_name = self.logdir / ('check-update-%s-%s.log' % (host, self.ts))
-
-        self.info( host, 'Starting Check for Updates' )
-        cmd = ['dnf', 'check-update', '--refresh']
-        rc, stdout = self.runAndLog( host, cmd, log=False )
-        self.writeLines( check_log_name, stdout )
-
-        if rc == 0:
-            self.info( host, 'Already up to date' )
-
-        elif rc == 100:
-            self.warn( host, 'Updates available' )
-
-        else:
-            self.error( host, 'check-update failed' )
-
-        self.checkServices( host, check_log_name )
+            return None, None
 
-        release = self.releaseInfo( host )
-        self.info( host, 'Running on Fedora release %s' % (release,) )
+        os_release = {}
 
-    def releaseInfo( self, host ):
-        cmd = ['cat', '/etc/system-release-cpe']
+        cmd = ['cat', '/etc/os-release']
         rc, stdout = self.runAndLog( host, cmd, log=False )
-        cpe_parts = stdout[0].strip().split( ':' )
-        if len(cpe_parts) >= 4 and cpe_parts[3] == 'fedora':
-            return int( cpe_parts[4] )
-
-        self.error( host, 'Host is not running Fedora - %r' % (cpe_parts,) )
-        return 0
-
-    def installPackage( self, host, package ):
-        rc = ssh_wait( host, wait=False, log_fn=None )
-        if rc != 0:
-            self.warn( host, 'Is not reachable' )
-            return
-
-        install_log_name = self.logdir / ('install-%s-%s.log' % (host, self.ts))
-
-        cmd = ['dnf', '-y', 'install', '--refresh', package]
-        rc, stdout = self.runAndLog( host, cmd )
-
-        self.writeLines( install_log_name, stdout )
-
-        if rc != 0:
-            self.error( host, 'Install failed' )
-            return
-
-    def update( self, host ):
-        rc = ssh_wait( host, wait=False, log_fn=None )
-        if rc != 0:
-            self.warn( host, 'Is not reachable' )
-            return
-
-        self.info( host, 'Starting Update' )
-
-        update_log_name = self.logdir / ('update-%s-%s.log' % (host, self.ts))
-        status_log_name = self.logdir / ('status-%s-%s.log' % (host, self.ts))
-
-        cmd = ['dnf', '-vy', 'update', '--refresh']
-        rc, stdout = self.runAndLog( host, cmd )
-
-        self.writeLines( update_log_name, stdout )
-
-        if rc != 0:
-            self.error( host, 'Update failed' )
-            return
-
-        if 'Nothing to do.\n' in stdout:
-            self.info( host, 'Already up to date' )
-            if not self.opt_force_reboot:
-                return
-
-        self.info( host, 'Check all systemd jobs finished' )
-        while True:
-            cmd = ['systemctl', 'list-jobs']
-            rc, stdout = self.runAndLog( host, cmd )
-            self.writeLines( update_log_name, stdout )
-            if rc != 0:
-                self.error( host, 'cannot list jobs' )
-                return
-
-            if 'No jobs running.\n' in stdout:
-                self.info( host, 'All systemd jobs finished' )
-                break
-
-            time.sleep( 10 )
+        for line in stdout:
+            line = line.strip()
+            if line == '' or '=' not in line:
+                continue
+
+            key, value = line.split( '=', 1 )
+            if value.startswith('"') and value.endswith('"'):
+                value = value[1:-1]
+            os_release[key] = value
+
+        os_main_id = os_release.get('ID', None)
+        os_id_set = set([os_main_id])
+        if 'ID_LIKE' in os_release:
+            for ID in os_release['ID_LIKE'].split():
+                os_id_set.add( ID )
+
+        for os_id in os_id_set:
+            if os_id in os_id_to_plugin:
+                return os_id, os_main_id
 
-        self.info( host, 'Rebooting' )
-        if self.reboot( host, ['reboot'] ):
-            self.checkServices( host, status_log_name )
+        return None, os_main_id
 
     def reboot( self, host, cmd, wait_limit=600 ):
         while True:
             rc, stdout = self.runAndLog( host, cmd )
             if len(stdout) == 0:
                 # no messages assume ok
                 break
@@ -444,51 +401,39 @@
 
     def checkServices( self, host, log_name=None ):
         cmd = ['systemctl', '--failed']
         rc, stdout = self.runAndLog( host, cmd, log=False )
         if log_name is not None:
             self.writeLines( log_name, stdout )
 
-        if '0 loaded units listed.\n' not in stdout:
+        if len(stdout) < 1 and not stdout[0].startswith( '0 loaded units listed.' ):
             for line in stdout:
                 print( self.ct( '<>proc %s<>: %s' % (host, line.rstrip()) ) )
 
             self.error( host, 'Some services failed' )
             return False
 
         self.info( host, 'All services running' )
         return True
 
-    def systemUpgrade( self, host, target_release ):
-        current_release = self.releaseInfo( host )
-        if current_release == target_release:
-            self.info( host, 'Already running Fedora release %d' % (target_release,) )
-            return
-
-        upgrade_log_name = self.logdir / ('update-%s-%s.log' % (host, self.ts))
-
-        self.info( host, 'Currently Fedora release %d' % (current_release,) )
-
-        # only update by one release at a time
-        next_release = current_release + 1
-
-        cmd = ['dnf', 'system-upgrade', 'download', '--releasever=%d' % (next_release,), '--assumeyes']
-        rc, stdout = self.runAndLog( host, cmd )
-        self.writeLines( upgrade_log_name, stdout )
-
-        if rc != 0:
-            self.error( host, 'Failure to download release %d' % (next_release,) )
-            return
+    def waitAllSystemdJobsFinished( self, host, log_name=None ):
+        self.info( host, 'Check all systemd jobs finished' )
+        while True:
+            cmd = ['systemctl', 'list-jobs']
+            rc, stdout = self.runAndLog( host, cmd )
+            self.writeLines( log_name, stdout )
+            if rc != 0:
+                self.error( host, 'cannot list jobs' )
+                return
 
-        self.info( host, 'Rebooting to install system-upgrade' )
-        # upgrades of lots of packages can be slow - wait for 45 minutes
-        if self.reboot( host, ['dnf', 'system-upgrade', 'reboot'], wait_limit=45*60 ):
-            self.checkServices( host, upgrade_log_name )
+            if 'No jobs running.\n' in stdout:
+                self.info( host, 'All systemd jobs finished' )
+                break
 
-        self.info( host, 'Now running Fedora release %d' % (self.releaseInfo( host ),) )
+            time.sleep( 10 )
 
     def runAndLog( self, host, cmd, log=True ):
         if host is not None:
             cmd = ['ssh', 'root@%s' % (host,)] + cmd
 
         self.debug( 'runAndLog( %s )' % (' '.join( cmd ),) )
         stdout = []
@@ -535,7 +480,215 @@
         log_line = self.ct( fmt % {'HOST': host
                                   ,'TIME': t.strftime( '%H:%M:%S' )
                                   ,'MSG': msg} )
         print( log_line, flush=True )
         if self.summary_log is not None:
             print( log_line, file=self.summary_log, flush=True )
             self.all_summary_lines.append( log_line )
+
+class UpdatePluginFedora:
+    def __init__( self, app ):
+        self.app = app
+
+    def check( self, host, check_log_name ):
+        rc = ssh_wait( host, wait=False, log_fn=None )
+        if rc != 0:
+            self.app.warn( host, 'Is not reachable' )
+            return
+
+        self.app.info( host, 'Starting Check for Updates' )
+        cmd = ['dnf', 'check-update', '--refresh']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        self.app.writeLines( check_log_name, stdout )
+
+        if rc == 0:
+            self.app.info( host, 'Already up to date' )
+
+        elif rc == 100:
+            self.app.warn( host, 'Updates available' )
+
+        else:
+            self.app.error( host, 'check-update failed' )
+
+        self.app.checkServices( host, check_log_name )
+
+        release = self.releaseInfo( host )
+        self.app.info( host, 'Running on release %s' % (release,) )
+
+    def installPackage( self, host, package, install_log_name ):
+        rc = ssh_wait( host, wait=False, log_fn=None )
+        if rc != 0:
+            self.app.warn( host, 'Is not reachable' )
+            return
+
+        cmd = ['dnf', '-y', 'install', '--refresh', package]
+        rc, stdout = self.app.runAndLog( host, cmd )
+
+        self.app.writeLines( install_log_name, stdout )
+
+        if rc != 0:
+            self.app.error( host, 'Install failed' )
+            return
+
+    def update( self, host, update_log_name, status_log_name ):
+        rc = ssh_wait( host, wait=False, log_fn=None )
+        if rc != 0:
+            self.app.warn( host, 'Is not reachable' )
+            return
+
+        self.app.info( host, 'Starting Update' )
+
+        cmd = ['dnf', '-vy', 'update', '--refresh']
+        rc, stdout = self.app.runAndLog( host, cmd )
+
+        self.app.writeLines( update_log_name, stdout )
+
+        if rc != 0:
+            self.app.error( host, 'Update failed' )
+            return
+
+        if 'Nothing to do.\n' in stdout:
+            self.app.info( host, 'Already up to date' )
+            if not self.app.opt_force_reboot:
+                return
+
+        self.app.waitAllSystemdJobsFinished( host, update_log_name )
+
+        self.app.info( host, 'Rebooting' )
+        if self.app.reboot( host, ['reboot'] ):
+            self.app.checkServices( host, status_log_name )
+
+    def systemUpgrade( self, host, target_release, upgrade_log_name ):
+        current_release = self.app.releaseInfo( host )
+        if current_release == target_release:
+            self.app.info( host, 'Already running release %d' % (target_release,) )
+            return
+
+        self.app.info( host, 'Currently release %d' % (current_release,) )
+
+        # only update by one release at a time
+        next_release = current_release + 1
+
+        cmd = ['dnf', 'system-upgrade', 'download', '--releasever=%d' % (next_release,), '--assumeyes']
+        rc, stdout = self.app.runAndLog( host, cmd )
+        self.app.writeLines( upgrade_log_name, stdout )
+
+        if rc != 0:
+            self.app.error( host, 'Failure to download release %d' % (next_release,) )
+            return
+
+        self.app.info( host, 'Rebooting to install system-upgrade' )
+        # upgrades of lots of packages can be slow - wait for 45 minutes
+        if self.app.reboot( host, ['dnf', 'system-upgrade', 'reboot'], wait_limit=45*60 ):
+            self.app.checkServices( host, upgrade_log_name )
+
+        self.app.info( host, 'Now running release %d' % (self.app.releaseInfo( host ),) )
+
+    def releaseInfo( self, host ):
+        cmd = ['cat', '/etc/system-release-cpe']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        cpe_parts = stdout[0].strip().split( ':' )
+        if len(cpe_parts) >= 4:
+            return int( cpe_parts[4] )
+
+        self.app.error( host, 'Not enough fields in /etc/system-release-cpe - %r' % (cpe_parts,) )
+        return 0
+
+
+class UpdatePluginDebian:
+    def __init__( self, app ):
+        self.app = app
+
+    def check( self, host, check_log_name ):
+        rc = ssh_wait( host, wait=False, log_fn=None )
+        if rc != 0:
+            self.app.warn( host, 'Is not reachable' )
+            return
+
+        self.app.info( host, 'Starting Check for Updates' )
+        cmd = ['apt-get', 'update', '--assume-yes']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        self.app.writeLines( check_log_name, stdout )
+        if rc != 0:
+            self.app.error( host, 'apt-get update failed' )
+            return
+
+        cmd = ['apt-get', 'upgrade', '--assume-no']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        self.app.debug( 'check_log_name %s' % (check_log_name,) )
+        self.app.writeLines( check_log_name, stdout )
+
+        for line in stdout:
+            words = line.split()
+            self.app.debug( 'apt-get-upgrade: %r' % (words,) )
+            if len(words) >= 2 and words[1] == 'upgraded,':
+                if words[0] == '0':
+                    self.app.info( host, 'Already up to date' )
+
+                else:
+                    self.app.warn( host, 'Updates available: %s' % (line,) )
+
+                self.app.checkServices( host, check_log_name )
+                return
+
+        self.app.error( host, 'apt-get upgrade failed' )
+
+    def installPackage( self, host, package, install_log_name ):
+        pass
+
+    def update( self, host, update_log_name, status_log_name ):
+        rc = ssh_wait( host, wait=False, log_fn=None )
+        if rc != 0:
+            self.app.warn( host, 'Is not reachable' )
+            return
+
+        self.app.info( host, 'Starting Update' )
+        cmd = ['apt-get', 'update', '--assume-yes']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        self.app.writeLines( update_log_name, stdout )
+        if rc != 0:
+            self.app.error( host, 'apt-get update failed' )
+            return
+
+        cmd = ['apt-get', 'upgrade', '--assume-yes']
+        rc, stdout = self.app.runAndLog( host, cmd )
+
+        self.app.writeLines( update_log_name, stdout )
+
+        for line in stdout:
+            words = line.split()
+            self.app.debug( 'apt-get-upgrade: %r' % (words,) )
+            if len(words) >= 2 and words[1] == 'upgraded,':
+                if words[0] == '0':
+                    self.app.info( host, 'Already up to date' )
+                    if not self.app.opt_force_reboot:
+                        return
+
+                else:
+                    self.app.info( host, 'Updated: %s' % (line,) )
+                break
+
+        self.updateAptFileDatabase( host, update_log_name )
+
+        self.app.waitAllSystemdJobsFinished( host, update_log_name )
+
+        self.app.info( host, 'Rebooting' )
+        if self.app.reboot( host, ['reboot'] ):
+            self.app.checkServices( host, status_log_name )
+
+    def updateAptFileDatabase( self, host, update_log_name ):
+        cmd = ['/usr/bin/test', '-x', '/usr/bin/apt-file']
+        rc, stdout = self.app.runAndLog( host, cmd, log=False )
+        if rc == 0:
+            self.app.info( host, 'Updating apt-file database' )
+            cmd = ['/usr/bin/apt-file', 'update']
+            rc, stdout = self.app.runAndLog( host, cmd, log=True )
+            self.app.writeLines( update_log_name, stdout )
+
+    def systemUpgrade( self, host, target_release, upgrade_log_name ):
+        pass
+
+
+os_id_to_plugin = {
+    'fedora':   UpdatePluginFedora,
+    'debian':   UpdatePluginDebian,
+    }
```

### Comparing `update-linux-2.2.0/update_linux.egg-info/PKG-INFO` & `update-linux-2.3.0/update_linux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.2.0
+Version: 2.3.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,21 @@
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # update-linux command
 
-Command to automate the routine updating of packages and system upgrading for Fedora systems.
+Command to automate the routine updating of packages and system upgrading for Unix systems.
+
+Supports Fedora like and Debian Like OS.
+
+Fedora like includes Fedora, RHEL, Centos, Rocky etc that use DNF.
+
+Debian like includes Dedian, Ubuntu etc that use apt.
 
 update-linux uses ssh to run commands on the hosts being worked.
 
 It assumes that it can `ssh root@<host>` without a password prompt.
 
 If running update-linux on a macOS system it is necessary to flush DNS so that freshly booted hosts can be accessed by host-name.
 
@@ -35,15 +41,17 @@
 $ update-linux host
 ```
 
 For an update the following steps are performed:
 
 1. Update packages  - if there is nothing to update stop here
 
-    `dnf -vy update --refresh`
+    Fedora: `dnf -vy update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-yes`
 
 1. Wait until all systemd jobs have finished
 
     `systemctl list-jobs`
 
     For example akmod building nvidia drivers for a new kernel
 
@@ -59,31 +67,33 @@
 
 ```
 $ update-linux host --check
 ```
 
 With the `--check` options these steps are performed:
 
-1. Check is there are packages to update
+1. Check if there are packages to update
 
-    `dnf check-update --refresh`
+    Fedora: `dnf check-update --refresh`
+
+    Debian: `apt-get update --assume-yes` then `apt-get upgrade --assume-no`
 
 1. Report on state of any failed services
 
     `systemctl --failed`
 
 ## update-linux system-upgrade process
 
 ```
-$ update-linux --system-upgrade=37 host
+$ update-linux --system-upgrade=38 host
 ```
 
 For a system-upgrade update-linux will update one release at a time.
 
-This means that a host running Fedora 35 that is being upgraded to Fedora 37 will first be upgraded to Fedora 36.
+This means that a host running Fedora 36 that is being upgraded to Fedora 38 will first be upgraded to Fedora 37.
 
 This is done as it is the safer then attempting skip over releases that can have required side-effects.
 
 Run the `update-linux --system-upgrade` once for each release that is be upgraded.
 
 For a system-upgrade these steps are used:
 
@@ -180,18 +190,18 @@
 
 Install updates:
 
 ```
 $ update-linux host1 host2
 ```
 
-Apply a system upgrade to Fedota 37:
+Apply a system upgrade to Fedora 38:
 
 ```
-$ update-linux --system-upgrade=37 host3
+$ update-linux --system-upgrade=38 host3
 ```
 
 ## update-linux configuration
 
 The configuration for update-linux is stored in a JSON file.
 
 On linux this is in ~/.config/org.barrys-emacs.update-linux.json and
@@ -203,16 +213,15 @@
 {
     "logdir":   "~/tmpdir",
     "group":
         {
             "all": [
                 "router",
                 "player",
-                "armf36",
-                "armf37"
+                "vm"
                 ],
             "vm": [
                 "armf36",
                 "armf37"
                 ]
         }
 }
```

