# Comparing `tmp/pyinfra-2.6.2.tar.gz` & `tmp/pyinfra-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinfra-2.6.2.tar", last modified: Sun Jan 29 21:11:01 2023, max compression
+gzip compressed data, was "pyinfra-2.7.tar", last modified: Mon May 15 21:06:21 2023, max compression
```

## Comparing `pyinfra-2.6.2.tar` & `pyinfra-2.7.tar`

### file list

```diff
@@ -1,193 +1,199 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.283026 pyinfra-2.6.2/
--rw-r--r--   0 nick       (501) staff       (20)    10002 2023-01-29 21:02:28.000000 pyinfra-2.6.2/CHANGELOG.md
--rw-r--r--   0 nick       (501) staff       (20)     1076 2021-01-18 10:52:39.000000 pyinfra-2.6.2/LICENSE.md
--rw-r--r--   0 nick       (501) staff       (20)       42 2022-09-25 11:45:43.000000 pyinfra-2.6.2/MANIFEST.in
--rw-r--r--   0 nick       (501) staff       (20)     5810 2023-01-29 21:11:01.283141 pyinfra-2.6.2/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     4540 2022-11-03 15:24:51.000000 pyinfra-2.6.2/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.259648 pyinfra-2.6.2/pyinfra/
--rw-r--r--   0 nick       (501) staff       (20)      535 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)       47 2020-01-22 18:18:30.000000 pyinfra-2.6.2/pyinfra/__main__.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.262675 pyinfra-2.6.2/pyinfra/api/
--rw-r--r--   0 nick       (501) staff       (20)      888 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/api/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)    10238 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/api/arguments.py
--rw-r--r--   0 nick       (501) staff       (20)     6561 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/api/command.py
--rw-r--r--   0 nick       (501) staff       (20)     3824 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/api/config.py
--rw-r--r--   0 nick       (501) staff       (20)     1417 2022-10-24 14:29:25.000000 pyinfra-2.6.2/pyinfra/api/connect.py
--rw-r--r--   0 nick       (501) staff       (20)     1016 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/api/connectors.py
--rw-r--r--   0 nick       (501) staff       (20)     3909 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/api/deploy.py
--rw-r--r--   0 nick       (501) staff       (20)     1185 2022-11-08 19:59:49.000000 pyinfra-2.6.2/pyinfra/api/exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)    10981 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/api/facts.py
--rw-r--r--   0 nick       (501) staff       (20)    11473 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/api/host.py
--rw-r--r--   0 nick       (501) staff       (20)     7785 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/api/inventory.py
--rw-r--r--   0 nick       (501) staff       (20)    12571 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/api/operation.py
--rw-r--r--   0 nick       (501) staff       (20)    12146 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/api/operations.py
--rw-r--r--   0 nick       (501) staff       (20)    11272 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/api/state.py
--rw-r--r--   0 nick       (501) staff       (20)    11690 2022-12-19 07:42:13.000000 pyinfra-2.6.2/pyinfra/api/util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.264334 pyinfra-2.6.2/pyinfra/connectors/
--rw-r--r--   0 nick       (501) staff       (20)        0 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/connectors/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5638 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/connectors/ansible.py
--rw-r--r--   0 nick       (501) staff       (20)     5367 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/chroot.py
--rw-r--r--   0 nick       (501) staff       (20)     8549 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/docker.py
--rw-r--r--   0 nick       (501) staff       (20)     8504 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/connectors/dockerssh.py
--rw-r--r--   0 nick       (501) staff       (20)     6381 2023-01-15 17:15:24.000000 pyinfra-2.6.2/pyinfra/connectors/local.py
--rw-r--r--   0 nick       (501) staff       (20)     4454 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/mech.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.264493 pyinfra-2.6.2/pyinfra/connectors/pyinfrawinrmsession/
--rw-r--r--   0 nick       (501) staff       (20)     1113 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/connectors/pyinfrawinrmsession/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)    20901 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/connectors/ssh.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.264890 pyinfra-2.6.2/pyinfra/connectors/sshuserclient/
--rw-r--r--   0 nick       (501) staff       (20)       44 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/connectors/sshuserclient/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     9606 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/sshuserclient/client.py
--rw-r--r--   0 nick       (501) staff       (20)     2721 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/connectors/sshuserclient/config.py
--rw-r--r--   0 nick       (501) staff       (20)     3014 2023-01-15 18:23:12.000000 pyinfra-2.6.2/pyinfra/connectors/terraform.py
--rw-r--r--   0 nick       (501) staff       (20)     9157 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/util.py
--rw-r--r--   0 nick       (501) staff       (20)     4376 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/vagrant.py
--rw-r--r--   0 nick       (501) staff       (20)    10047 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/connectors/winrm.py
--rw-r--r--   0 nick       (501) staff       (20)     3351 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/context.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.270134 pyinfra-2.6.2/pyinfra/facts/
--rw-r--r--   0 nick       (501) staff       (20)      347 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      482 2023-01-15 17:15:24.000000 pyinfra-2.6.2/pyinfra/facts/apk.py
--rw-r--r--   0 nick       (501) staff       (20)     1999 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/apt.py
--rw-r--r--   0 nick       (501) staff       (20)     2266 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/facts/brew.py
--rw-r--r--   0 nick       (501) staff       (20)      490 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/bsdinit.py
--rw-r--r--   0 nick       (501) staff       (20)      716 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/choco.py
--rw-r--r--   0 nick       (501) staff       (20)     1662 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/deb.py
--rw-r--r--   0 nick       (501) staff       (20)      862 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/dnf.py
--rw-r--r--   0 nick       (501) staff       (20)     1657 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/docker.py
--rw-r--r--   0 nick       (501) staff       (20)    11071 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/facts/files.py
--rw-r--r--   0 nick       (501) staff       (20)      473 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/gem.py
--rw-r--r--   0 nick       (501) staff       (20)     1215 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/git.py
--rw-r--r--   0 nick       (501) staff       (20)     3688 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/gpg.py
--rw-r--r--   0 nick       (501) staff       (20)     9125 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/facts/hardware.py
--rw-r--r--   0 nick       (501) staff       (20)     3313 2022-10-24 14:29:25.000000 pyinfra-2.6.2/pyinfra/facts/iptables.py
--rw-r--r--   0 nick       (501) staff       (20)      668 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/launchd.py
--rw-r--r--   0 nick       (501) staff       (20)      337 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/lxd.py
--rw-r--r--   0 nick       (501) staff       (20)     5873 2023-01-15 17:15:24.000000 pyinfra-2.6.2/pyinfra/facts/mysql.py
--rw-r--r--   0 nick       (501) staff       (20)      674 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/facts/npm.py
--rw-r--r--   0 nick       (501) staff       (20)     1350 2023-01-15 17:15:24.000000 pyinfra-2.6.2/pyinfra/facts/openrc.py
--rw-r--r--   0 nick       (501) staff       (20)     1001 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/pacman.py
--rw-r--r--   0 nick       (501) staff       (20)      702 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/pip.py
--rw-r--r--   0 nick       (501) staff       (20)      452 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/pkg.py
--rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/pkgin.py
--rw-r--r--   0 nick       (501) staff       (20)     4035 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/postgresql.py
--rw-r--r--   0 nick       (501) staff       (20)     1973 2022-10-24 10:12:32.000000 pyinfra-2.6.2/pyinfra/facts/rpm.py
--rw-r--r--   0 nick       (501) staff       (20)     4219 2022-10-24 10:12:32.000000 pyinfra-2.6.2/pyinfra/facts/selinux.py
--rw-r--r--   0 nick       (501) staff       (20)    15566 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/facts/server.py
--rw-r--r--   0 nick       (501) staff       (20)     1910 2022-10-24 10:12:32.000000 pyinfra-2.6.2/pyinfra/facts/snap.py
--rw-r--r--   0 nick       (501) staff       (20)     3290 2022-10-24 14:29:25.000000 pyinfra-2.6.2/pyinfra/facts/systemd.py
--rw-r--r--   0 nick       (501) staff       (20)     1414 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/sysvinit.py
--rw-r--r--   0 nick       (501) staff       (20)      543 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/upstart.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.270701 pyinfra-2.6.2/pyinfra/facts/util/
--rw-r--r--   0 nick       (501) staff       (20)      521 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/util/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      730 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/util/databases.py
--rw-r--r--   0 nick       (501) staff       (20)     1017 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/util/packaging.py
--rw-r--r--   0 nick       (501) staff       (20)     2561 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/util/win_files.py
--rw-r--r--   0 nick       (501) staff       (20)      591 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/vzctl.py
--rw-r--r--   0 nick       (501) staff       (20)     8664 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra/facts/windows.py
--rw-r--r--   0 nick       (501) staff       (20)     2101 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/windows_files.py
--rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/xbps.py
--rw-r--r--   0 nick       (501) staff       (20)      827 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/yum.py
--rw-r--r--   0 nick       (501) staff       (20)      766 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/facts/zypper.py
--rw-r--r--   0 nick       (501) staff       (20)     2827 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/local.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.275964 pyinfra-2.6.2/pyinfra/operations/
--rw-r--r--   0 nick       (501) staff       (20)      357 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2033 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/apk.py
--rw-r--r--   0 nick       (501) staff       (20)    14106 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/operations/apt.py
--rw-r--r--   0 nick       (501) staff       (20)     4316 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/brew.py
--rw-r--r--   0 nick       (501) staff       (20)     1559 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/bsdinit.py
--rw-r--r--   0 nick       (501) staff       (20)     1451 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/choco.py
--rw-r--r--   0 nick       (501) staff       (20)     5537 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/dnf.py
--rw-r--r--   0 nick       (501) staff       (20)    57380 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/operations/files.py
--rw-r--r--   0 nick       (501) staff       (20)     1068 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/gem.py
--rw-r--r--   0 nick       (501) staff       (20)    12145 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/git.py
--rw-r--r--   0 nick       (501) staff       (20)     9098 2023-01-15 17:24:22.000000 pyinfra-2.6.2/pyinfra/operations/iptables.py
--rw-r--r--   0 nick       (501) staff       (20)     1162 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/launchd.py
--rw-r--r--   0 nick       (501) staff       (20)     1845 2022-10-22 20:51:32.000000 pyinfra-2.6.2/pyinfra/operations/lxd.py
--rw-r--r--   0 nick       (501) staff       (20)    19964 2023-01-15 17:15:24.000000 pyinfra-2.6.2/pyinfra/operations/mysql.py
--rw-r--r--   0 nick       (501) staff       (20)     1402 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/npm.py
--rw-r--r--   0 nick       (501) staff       (20)     1508 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/openrc.py
--rw-r--r--   0 nick       (501) staff       (20)     1656 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/pacman.py
--rw-r--r--   0 nick       (501) staff       (20)     5515 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/pip.py
--rw-r--r--   0 nick       (501) staff       (20)     2220 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/pkg.py
--rw-r--r--   0 nick       (501) staff       (20)     1914 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/pkgin.py
--rw-r--r--   0 nick       (501) staff       (20)    10500 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/operations/postgresql.py
--rw-r--r--   0 nick       (501) staff       (20)      797 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/puppet.py
--rw-r--r--   0 nick       (501) staff       (20)     2398 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/operations/python.py
--rw-r--r--   0 nick       (501) staff       (20)     6149 2022-10-24 10:12:32.000000 pyinfra-2.6.2/pyinfra/operations/selinux.py
--rw-r--r--   0 nick       (501) staff       (20)    31428 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/operations/server.py
--rw-r--r--   0 nick       (501) staff       (20)     3077 2023-01-15 18:23:12.000000 pyinfra-2.6.2/pyinfra/operations/snap.py
--rw-r--r--   0 nick       (501) staff       (20)     5933 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/operations/ssh.py
--rw-r--r--   0 nick       (501) staff       (20)     3521 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/systemd.py
--rw-r--r--   0 nick       (501) staff       (20)     4326 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/sysvinit.py
--rw-r--r--   0 nick       (501) staff       (20)     1887 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/upstart.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.276510 pyinfra-2.6.2/pyinfra/operations/util/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-06-11 10:13:46.000000 pyinfra-2.6.2/pyinfra/operations/util/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     3287 2022-10-24 10:12:32.000000 pyinfra-2.6.2/pyinfra/operations/util/files.py
--rw-r--r--   0 nick       (501) staff       (20)     9004 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra/operations/util/packaging.py
--rw-r--r--   0 nick       (501) staff       (20)     1990 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/util/service.py
--rw-r--r--   0 nick       (501) staff       (20)     2996 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/vzctl.py
--rw-r--r--   0 nick       (501) staff       (20)     1660 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/windows.py
--rw-r--r--   0 nick       (501) staff       (20)    16125 2023-01-29 20:56:26.000000 pyinfra-2.6.2/pyinfra/operations/windows_files.py
--rw-r--r--   0 nick       (501) staff       (20)     1430 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/xbps.py
--rw-r--r--   0 nick       (501) staff       (20)     5530 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/yum.py
--rw-r--r--   0 nick       (501) staff       (20)     5481 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/operations/zypper.py
--rw-r--r--   0 nick       (501) staff       (20)     4193 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/progress.py
--rw-r--r--   0 nick       (501) staff       (20)      153 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra/version.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.260563 pyinfra-2.6.2/pyinfra.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     5810 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     4792 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)      439 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)     1133 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       26 2023-01-29 21:11:01.000000 pyinfra-2.6.2/pyinfra.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.277797 pyinfra-2.6.2/pyinfra_cli/
--rw-r--r--   0 nick       (501) staff       (20)      284 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra_cli/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      859 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyinfra_cli/__main__.py
--rw-r--r--   0 nick       (501) staff       (20)     3704 2022-11-09 17:50:39.000000 pyinfra-2.6.2/pyinfra_cli/exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)     6168 2022-10-24 14:29:25.000000 pyinfra-2.6.2/pyinfra_cli/inventory.py
--rw-r--r--   0 nick       (501) staff       (20)     1714 2022-11-03 15:24:51.000000 pyinfra-2.6.2/pyinfra_cli/log.py
--rw-r--r--   0 nick       (501) staff       (20)    18297 2023-01-15 17:24:22.000000 pyinfra-2.6.2/pyinfra_cli/main.py
--rw-r--r--   0 nick       (501) staff       (20)    10426 2023-01-15 17:18:57.000000 pyinfra-2.6.2/pyinfra_cli/prints.py
--rw-r--r--   0 nick       (501) staff       (20)     7230 2023-01-15 17:24:22.000000 pyinfra-2.6.2/pyinfra_cli/util.py
--rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:43.000000 pyinfra-2.6.2/pyinfra_cli/virtualenv.py
--rw-r--r--   0 nick       (501) staff       (20)      534 2023-01-15 18:23:08.000000 pyinfra-2.6.2/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      663 2023-01-29 21:11:01.283503 pyinfra-2.6.2/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     5090 2023-01-15 17:24:22.000000 pyinfra-2.6.2/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.278377 pyinfra-2.6.2/tests/
--rw-r--r--   0 nick       (501) staff       (20)      343 2022-09-25 11:45:43.000000 pyinfra-2.6.2/tests/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2254 2022-11-03 15:24:51.000000 pyinfra-2.6.2/tests/paramiko_util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.279987 pyinfra-2.6.2/tests/test_api/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.6.2/tests/test_api/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2295 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api.py
--rw-r--r--   0 nick       (501) staff       (20)     2043 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_arguments.py
--rw-r--r--   0 nick       (501) staff       (20)     3204 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_command.py
--rw-r--r--   0 nick       (501) staff       (20)      708 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_config.py
--rw-r--r--   0 nick       (501) staff       (20)     4194 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_deploys.py
--rw-r--r--   0 nick       (501) staff       (20)    11745 2022-11-09 18:15:49.000000 pyinfra-2.6.2/tests/test_api/test_api_facts.py
--rw-r--r--   0 nick       (501) staff       (20)     1119 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_host.py
--rw-r--r--   0 nick       (501) staff       (20)     2013 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_inventory.py
--rw-r--r--   0 nick       (501) staff       (20)    23145 2023-01-15 17:15:24.000000 pyinfra-2.6.2/tests/test_api/test_api_operations.py
--rw-r--r--   0 nick       (501) staff       (20)      684 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_api/test_api_util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.280954 pyinfra-2.6.2/tests/test_cli/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.6.2/tests/test_cli/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     6928 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_cli/test_cli.py
--rw-r--r--   0 nick       (501) staff       (20)     5794 2022-10-24 10:12:32.000000 pyinfra-2.6.2/tests/test_cli/test_cli_deploy.py
--rw-r--r--   0 nick       (501) staff       (20)     1526 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_cli/test_cli_exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)     2458 2023-01-15 17:24:22.000000 pyinfra-2.6.2/tests/test_cli/test_cli_util.py
--rw-r--r--   0 nick       (501) staff       (20)     2130 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_cli/test_context_objects.py
--rw-r--r--   0 nick       (501) staff       (20)      315 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_cli/util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-01-29 21:11:01.282885 pyinfra-2.6.2/tests/test_connectors/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.6.2/tests/test_connectors/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2009 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_connectors/test_ansible.py
--rw-r--r--   0 nick       (501) staff       (20)     5904 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_connectors/test_chroot.py
--rw-r--r--   0 nick       (501) staff       (20)     6563 2022-11-03 15:24:51.000000 pyinfra-2.6.2/tests/test_connectors/test_docker.py
--rw-r--r--   0 nick       (501) staff       (20)     9438 2023-01-15 18:23:08.000000 pyinfra-2.6.2/tests/test_connectors/test_dockerssh.py
--rw-r--r--   0 nick       (501) staff       (20)     7494 2023-01-15 17:15:24.000000 pyinfra-2.6.2/tests/test_connectors/test_local.py
--rw-r--r--   0 nick       (501) staff       (20)     4307 2022-11-03 15:24:51.000000 pyinfra-2.6.2/tests/test_connectors/test_mech.py
--rw-r--r--   0 nick       (501) staff       (20)    35114 2023-01-15 18:23:08.000000 pyinfra-2.6.2/tests/test_connectors/test_ssh.py
--rw-r--r--   0 nick       (501) staff       (20)     5681 2022-11-05 16:57:27.000000 pyinfra-2.6.2/tests/test_connectors/test_sshuserclient.py
--rw-r--r--   0 nick       (501) staff       (20)     3569 2023-01-15 18:23:12.000000 pyinfra-2.6.2/tests/test_connectors/test_terraform.py
--rw-r--r--   0 nick       (501) staff       (20)     5195 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_connectors/test_util.py
--rw-r--r--   0 nick       (501) staff       (20)     3542 2022-11-03 15:24:51.000000 pyinfra-2.6.2/tests/test_connectors/test_vagrant.py
--rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_connectors/test_winrm.py
--rw-r--r--   0 nick       (501) staff       (20)     3308 2022-09-25 11:45:44.000000 pyinfra-2.6.2/tests/test_facts.py
--rw-r--r--   0 nick       (501) staff       (20)    12505 2023-01-15 18:23:08.000000 pyinfra-2.6.2/tests/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.877574 pyinfra-2.7/
+-rw-r--r--   0 nick       (501) staff       (20)    10819 2023-05-15 20:45:14.000000 pyinfra-2.7/CHANGELOG.md
+-rw-r--r--   0 nick       (501) staff       (20)     1076 2021-01-18 10:52:39.000000 pyinfra-2.7/LICENSE.md
+-rw-r--r--   0 nick       (501) staff       (20)       42 2022-09-25 11:45:43.000000 pyinfra-2.7/MANIFEST.in
+-rw-r--r--   0 nick       (501) staff       (20)     5808 2023-05-15 21:06:21.877656 pyinfra-2.7/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     4540 2022-11-03 15:24:51.000000 pyinfra-2.7/README.md
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.845993 pyinfra-2.7/pyinfra/
+-rw-r--r--   0 nick       (501) staff       (20)      535 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)       47 2020-01-22 18:18:30.000000 pyinfra-2.7/pyinfra/__main__.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.849485 pyinfra-2.7/pyinfra/api/
+-rw-r--r--   0 nick       (501) staff       (20)      888 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)    10238 2023-05-11 16:47:41.000000 pyinfra-2.7/pyinfra/api/arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     6561 2023-03-21 14:27:34.000000 pyinfra-2.7/pyinfra/api/command.py
+-rw-r--r--   0 nick       (501) staff       (20)     3824 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/api/config.py
+-rw-r--r--   0 nick       (501) staff       (20)     1417 2022-10-24 14:29:25.000000 pyinfra-2.7/pyinfra/api/connect.py
+-rw-r--r--   0 nick       (501) staff       (20)     1016 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/api/connectors.py
+-rw-r--r--   0 nick       (501) staff       (20)     3909 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/api/deploy.py
+-rw-r--r--   0 nick       (501) staff       (20)     1185 2022-11-08 19:59:49.000000 pyinfra-2.7/pyinfra/api/exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)    11227 2023-05-15 20:15:24.000000 pyinfra-2.7/pyinfra/api/facts.py
+-rw-r--r--   0 nick       (501) staff       (20)    11473 2023-03-04 08:33:27.000000 pyinfra-2.7/pyinfra/api/host.py
+-rw-r--r--   0 nick       (501) staff       (20)     7785 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/api/inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)    12571 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/api/operation.py
+-rw-r--r--   0 nick       (501) staff       (20)    12146 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/api/operations.py
+-rw-r--r--   0 nick       (501) staff       (20)    11272 2023-03-07 14:45:07.000000 pyinfra-2.7/pyinfra/api/state.py
+-rw-r--r--   0 nick       (501) staff       (20)    11690 2022-12-19 07:42:13.000000 pyinfra-2.7/pyinfra/api/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.852160 pyinfra-2.7/pyinfra/connectors/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/connectors/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5638 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/connectors/ansible.py
+-rw-r--r--   0 nick       (501) staff       (20)     5367 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/chroot.py
+-rw-r--r--   0 nick       (501) staff       (20)     8549 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/docker.py
+-rw-r--r--   0 nick       (501) staff       (20)     8504 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/connectors/dockerssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     6381 2023-01-15 17:15:24.000000 pyinfra-2.7/pyinfra/connectors/local.py
+-rw-r--r--   0 nick       (501) staff       (20)     4454 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/mech.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.852390 pyinfra-2.7/pyinfra/connectors/pyinfrawinrmsession/
+-rw-r--r--   0 nick       (501) staff       (20)     1113 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/connectors/pyinfrawinrmsession/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)    21254 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/connectors/ssh.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.853003 pyinfra-2.7/pyinfra/connectors/sshuserclient/
+-rw-r--r--   0 nick       (501) staff       (20)       44 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/connectors/sshuserclient/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     9606 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/sshuserclient/client.py
+-rw-r--r--   0 nick       (501) staff       (20)     2721 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/connectors/sshuserclient/config.py
+-rw-r--r--   0 nick       (501) staff       (20)     3014 2023-01-15 18:23:12.000000 pyinfra-2.7/pyinfra/connectors/terraform.py
+-rw-r--r--   0 nick       (501) staff       (20)     9157 2023-05-11 16:47:41.000000 pyinfra-2.7/pyinfra/connectors/util.py
+-rw-r--r--   0 nick       (501) staff       (20)     4376 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/vagrant.py
+-rw-r--r--   0 nick       (501) staff       (20)    10047 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/connectors/winrm.py
+-rw-r--r--   0 nick       (501) staff       (20)     3351 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/context.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.859390 pyinfra-2.7/pyinfra/facts/
+-rw-r--r--   0 nick       (501) staff       (20)      347 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      482 2023-01-15 17:15:24.000000 pyinfra-2.7/pyinfra/facts/apk.py
+-rw-r--r--   0 nick       (501) staff       (20)     1999 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/apt.py
+-rw-r--r--   0 nick       (501) staff       (20)     2266 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/facts/brew.py
+-rw-r--r--   0 nick       (501) staff       (20)      490 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/bsdinit.py
+-rw-r--r--   0 nick       (501) staff       (20)      531 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/facts/cargo.py
+-rw-r--r--   0 nick       (501) staff       (20)      716 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/choco.py
+-rw-r--r--   0 nick       (501) staff       (20)     1662 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/deb.py
+-rw-r--r--   0 nick       (501) staff       (20)      862 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/dnf.py
+-rw-r--r--   0 nick       (501) staff       (20)     1657 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/docker.py
+-rw-r--r--   0 nick       (501) staff       (20)    11071 2023-05-15 20:15:16.000000 pyinfra-2.7/pyinfra/facts/files.py
+-rw-r--r--   0 nick       (501) staff       (20)      473 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/gem.py
+-rw-r--r--   0 nick       (501) staff       (20)     1236 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/facts/git.py
+-rw-r--r--   0 nick       (501) staff       (20)     3688 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/gpg.py
+-rw-r--r--   0 nick       (501) staff       (20)     9125 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/facts/hardware.py
+-rw-r--r--   0 nick       (501) staff       (20)     3313 2022-10-24 14:29:25.000000 pyinfra-2.7/pyinfra/facts/iptables.py
+-rw-r--r--   0 nick       (501) staff       (20)      668 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/launchd.py
+-rw-r--r--   0 nick       (501) staff       (20)      337 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/lxd.py
+-rw-r--r--   0 nick       (501) staff       (20)     5873 2023-01-15 17:15:24.000000 pyinfra-2.7/pyinfra/facts/mysql.py
+-rw-r--r--   0 nick       (501) staff       (20)      674 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/facts/npm.py
+-rw-r--r--   0 nick       (501) staff       (20)     1350 2023-01-15 17:15:24.000000 pyinfra-2.7/pyinfra/facts/openrc.py
+-rw-r--r--   0 nick       (501) staff       (20)     1001 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/pacman.py
+-rw-r--r--   0 nick       (501) staff       (20)      702 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/pip.py
+-rw-r--r--   0 nick       (501) staff       (20)      452 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/pkg.py
+-rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/pkgin.py
+-rw-r--r--   0 nick       (501) staff       (20)     4035 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/postgresql.py
+-rw-r--r--   0 nick       (501) staff       (20)     1973 2022-10-24 10:12:32.000000 pyinfra-2.7/pyinfra/facts/rpm.py
+-rw-r--r--   0 nick       (501) staff       (20)     4219 2022-10-24 10:12:32.000000 pyinfra-2.7/pyinfra/facts/selinux.py
+-rw-r--r--   0 nick       (501) staff       (20)    16004 2023-05-13 17:41:03.000000 pyinfra-2.7/pyinfra/facts/server.py
+-rw-r--r--   0 nick       (501) staff       (20)     1910 2022-10-24 10:12:32.000000 pyinfra-2.7/pyinfra/facts/snap.py
+-rw-r--r--   0 nick       (501) staff       (20)     3290 2022-10-24 14:29:25.000000 pyinfra-2.7/pyinfra/facts/systemd.py
+-rw-r--r--   0 nick       (501) staff       (20)     1414 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/sysvinit.py
+-rw-r--r--   0 nick       (501) staff       (20)      543 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/upstart.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.860414 pyinfra-2.7/pyinfra/facts/util/
+-rw-r--r--   0 nick       (501) staff       (20)      521 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/util/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      730 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/util/databases.py
+-rw-r--r--   0 nick       (501) staff       (20)     1017 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/util/packaging.py
+-rw-r--r--   0 nick       (501) staff       (20)     2561 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/util/win_files.py
+-rw-r--r--   0 nick       (501) staff       (20)      591 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/vzctl.py
+-rw-r--r--   0 nick       (501) staff       (20)     8664 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra/facts/windows.py
+-rw-r--r--   0 nick       (501) staff       (20)     2101 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/windows_files.py
+-rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/xbps.py
+-rw-r--r--   0 nick       (501) staff       (20)      827 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/yum.py
+-rw-r--r--   0 nick       (501) staff       (20)      766 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/facts/zypper.py
+-rw-r--r--   0 nick       (501) staff       (20)     2827 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/local.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.867558 pyinfra-2.7/pyinfra/operations/
+-rw-r--r--   0 nick       (501) staff       (20)      357 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2033 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/apk.py
+-rw-r--r--   0 nick       (501) staff       (20)    14106 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/operations/apt.py
+-rw-r--r--   0 nick       (501) staff       (20)     4316 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/brew.py
+-rw-r--r--   0 nick       (501) staff       (20)     1559 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/bsdinit.py
+-rw-r--r--   0 nick       (501) staff       (20)     1040 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/operations/cargo.py
+-rw-r--r--   0 nick       (501) staff       (20)     1451 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/choco.py
+-rw-r--r--   0 nick       (501) staff       (20)     5537 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/dnf.py
+-rw-r--r--   0 nick       (501) staff       (20)    57962 2023-02-21 20:49:23.000000 pyinfra-2.7/pyinfra/operations/files.py
+-rw-r--r--   0 nick       (501) staff       (20)     1068 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/gem.py
+-rw-r--r--   0 nick       (501) staff       (20)    12493 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/operations/git.py
+-rw-r--r--   0 nick       (501) staff       (20)     9098 2023-01-15 17:24:22.000000 pyinfra-2.7/pyinfra/operations/iptables.py
+-rw-r--r--   0 nick       (501) staff       (20)     1162 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/launchd.py
+-rw-r--r--   0 nick       (501) staff       (20)     1845 2022-10-22 20:51:32.000000 pyinfra-2.7/pyinfra/operations/lxd.py
+-rw-r--r--   0 nick       (501) staff       (20)    19964 2023-05-13 07:59:51.000000 pyinfra-2.7/pyinfra/operations/mysql.py
+-rw-r--r--   0 nick       (501) staff       (20)     1402 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/npm.py
+-rw-r--r--   0 nick       (501) staff       (20)     1508 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/openrc.py
+-rw-r--r--   0 nick       (501) staff       (20)     1656 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/pacman.py
+-rw-r--r--   0 nick       (501) staff       (20)     5515 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/pip.py
+-rw-r--r--   0 nick       (501) staff       (20)     2220 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/pkg.py
+-rw-r--r--   0 nick       (501) staff       (20)     1914 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/pkgin.py
+-rw-r--r--   0 nick       (501) staff       (20)    10500 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/operations/postgresql.py
+-rw-r--r--   0 nick       (501) staff       (20)      797 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/puppet.py
+-rw-r--r--   0 nick       (501) staff       (20)     2398 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/operations/python.py
+-rw-r--r--   0 nick       (501) staff       (20)     6149 2022-10-24 10:12:32.000000 pyinfra-2.7/pyinfra/operations/selinux.py
+-rw-r--r--   0 nick       (501) staff       (20)    33520 2023-05-13 17:41:03.000000 pyinfra-2.7/pyinfra/operations/server.py
+-rw-r--r--   0 nick       (501) staff       (20)     3077 2023-01-15 18:23:12.000000 pyinfra-2.7/pyinfra/operations/snap.py
+-rw-r--r--   0 nick       (501) staff       (20)     5933 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/operations/ssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     3521 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/systemd.py
+-rw-r--r--   0 nick       (501) staff       (20)     4326 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/sysvinit.py
+-rw-r--r--   0 nick       (501) staff       (20)     1887 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/upstart.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.868280 pyinfra-2.7/pyinfra/operations/util/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-06-11 10:13:46.000000 pyinfra-2.7/pyinfra/operations/util/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     3329 2023-05-13 08:24:28.000000 pyinfra-2.7/pyinfra/operations/util/files.py
+-rw-r--r--   0 nick       (501) staff       (20)     9004 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra/operations/util/packaging.py
+-rw-r--r--   0 nick       (501) staff       (20)     1990 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/util/service.py
+-rw-r--r--   0 nick       (501) staff       (20)     2996 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/vzctl.py
+-rw-r--r--   0 nick       (501) staff       (20)     1660 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/windows.py
+-rw-r--r--   0 nick       (501) staff       (20)    16125 2023-01-29 20:56:26.000000 pyinfra-2.7/pyinfra/operations/windows_files.py
+-rw-r--r--   0 nick       (501) staff       (20)     1430 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/xbps.py
+-rw-r--r--   0 nick       (501) staff       (20)     5530 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/yum.py
+-rw-r--r--   0 nick       (501) staff       (20)     5481 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/operations/zypper.py
+-rw-r--r--   0 nick       (501) staff       (20)     4193 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/progress.py
+-rw-r--r--   0 nick       (501) staff       (20)      153 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra/version.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.846667 pyinfra-2.7/pyinfra.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     5808 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     4954 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)      439 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/entry_points.txt
+-rw-r--r--   0 nick       (501) staff       (20)     1101 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)       26 2023-05-15 21:06:21.000000 pyinfra-2.7/pyinfra.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.870511 pyinfra-2.7/pyinfra_cli/
+-rw-r--r--   0 nick       (501) staff       (20)      284 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra_cli/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      859 2023-01-15 18:23:08.000000 pyinfra-2.7/pyinfra_cli/__main__.py
+-rw-r--r--   0 nick       (501) staff       (20)     1669 2023-05-13 08:20:28.000000 pyinfra-2.7/pyinfra_cli/commands.py
+-rw-r--r--   0 nick       (501) staff       (20)     3704 2022-11-09 17:50:39.000000 pyinfra-2.7/pyinfra_cli/exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)     8733 2023-05-13 08:20:28.000000 pyinfra-2.7/pyinfra_cli/inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)     1714 2022-11-03 15:24:51.000000 pyinfra-2.7/pyinfra_cli/log.py
+-rw-r--r--   0 nick       (501) staff       (20)    18272 2023-05-13 08:20:28.000000 pyinfra-2.7/pyinfra_cli/main.py
+-rw-r--r--   0 nick       (501) staff       (20)    10426 2023-01-15 17:18:57.000000 pyinfra-2.7/pyinfra_cli/prints.py
+-rw-r--r--   0 nick       (501) staff       (20)     5374 2023-05-13 08:20:28.000000 pyinfra-2.7/pyinfra_cli/util.py
+-rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:43.000000 pyinfra-2.7/pyinfra_cli/virtualenv.py
+-rw-r--r--   0 nick       (501) staff       (20)      534 2023-01-15 18:23:08.000000 pyinfra-2.7/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      663 2023-05-15 21:06:21.877938 pyinfra-2.7/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)     5067 2023-05-13 08:24:28.000000 pyinfra-2.7/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.871736 pyinfra-2.7/tests/
+-rw-r--r--   0 nick       (501) staff       (20)      343 2022-09-25 11:45:43.000000 pyinfra-2.7/tests/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2254 2022-11-03 15:24:51.000000 pyinfra-2.7/tests/paramiko_util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.873633 pyinfra-2.7/tests/test_api/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.7/tests/test_api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2295 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api.py
+-rw-r--r--   0 nick       (501) staff       (20)     2043 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     3204 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_command.py
+-rw-r--r--   0 nick       (501) staff       (20)      708 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_config.py
+-rw-r--r--   0 nick       (501) staff       (20)     4194 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_deploys.py
+-rw-r--r--   0 nick       (501) staff       (20)    11745 2022-11-09 18:15:49.000000 pyinfra-2.7/tests/test_api/test_api_facts.py
+-rw-r--r--   0 nick       (501) staff       (20)     1119 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_host.py
+-rw-r--r--   0 nick       (501) staff       (20)     2013 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)    23145 2023-01-15 17:15:24.000000 pyinfra-2.7/tests/test_api/test_api_operations.py
+-rw-r--r--   0 nick       (501) staff       (20)      684 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_api/test_api_util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.874675 pyinfra-2.7/tests/test_cli/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.7/tests/test_cli/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     6967 2023-05-13 08:20:28.000000 pyinfra-2.7/tests/test_cli/test_cli.py
+-rw-r--r--   0 nick       (501) staff       (20)     5794 2022-10-24 10:12:32.000000 pyinfra-2.7/tests/test_cli/test_cli_deploy.py
+-rw-r--r--   0 nick       (501) staff       (20)     1565 2023-05-13 08:20:28.000000 pyinfra-2.7/tests/test_cli/test_cli_exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)     2562 2023-05-13 08:20:28.000000 pyinfra-2.7/tests/test_cli/test_cli_util.py
+-rw-r--r--   0 nick       (501) staff       (20)     2130 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_cli/test_context_objects.py
+-rw-r--r--   0 nick       (501) staff       (20)      315 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_cli/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-05-15 21:06:21.877439 pyinfra-2.7/tests/test_connectors/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-2.7/tests/test_connectors/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2009 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_connectors/test_ansible.py
+-rw-r--r--   0 nick       (501) staff       (20)     5904 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_connectors/test_chroot.py
+-rw-r--r--   0 nick       (501) staff       (20)     6563 2022-11-03 15:24:51.000000 pyinfra-2.7/tests/test_connectors/test_docker.py
+-rw-r--r--   0 nick       (501) staff       (20)     9438 2023-01-15 18:23:08.000000 pyinfra-2.7/tests/test_connectors/test_dockerssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     7494 2023-01-15 17:15:24.000000 pyinfra-2.7/tests/test_connectors/test_local.py
+-rw-r--r--   0 nick       (501) staff       (20)     4307 2022-11-03 15:24:51.000000 pyinfra-2.7/tests/test_connectors/test_mech.py
+-rw-r--r--   0 nick       (501) staff       (20)    37584 2023-05-13 08:24:28.000000 pyinfra-2.7/tests/test_connectors/test_ssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     5681 2022-11-05 16:57:27.000000 pyinfra-2.7/tests/test_connectors/test_sshuserclient.py
+-rw-r--r--   0 nick       (501) staff       (20)     3569 2023-01-15 18:23:12.000000 pyinfra-2.7/tests/test_connectors/test_terraform.py
+-rw-r--r--   0 nick       (501) staff       (20)     5195 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_connectors/test_util.py
+-rw-r--r--   0 nick       (501) staff       (20)     3542 2022-11-03 15:24:51.000000 pyinfra-2.7/tests/test_connectors/test_vagrant.py
+-rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_connectors/test_winrm.py
+-rw-r--r--   0 nick       (501) staff       (20)     3308 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_facts.py
+-rw-r--r--   0 nick       (501) staff       (20)     1688 2022-11-05 16:24:27.000000 pyinfra-2.7/tests/test_global_arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     8187 2022-10-24 10:12:32.000000 pyinfra-2.7/tests/test_operations.py
+-rw-r--r--   0 nick       (501) staff       (20)      557 2022-09-25 11:45:44.000000 pyinfra-2.7/tests/test_operations_utils.py
+-rw-r--r--   0 nick       (501) staff       (20)    12505 2023-01-15 18:23:08.000000 pyinfra-2.7/tests/util.py
```

### Comparing `pyinfra-2.6.2/CHANGELOG.md` & `pyinfra-2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# v2.7
+
+Been a while since a release, so there's a bunch of great stuff in thise one!
+
+Added:
+
++ Add experimental support for importing inventories from Python modules
++ Add `caro.packages` operation (@wowi42)
++ Add `server.locale` operation and `server.Locales` fact (@maisim)
++ Add `ensure_newline` keyword argument to `files.line` (@yunzheng)
++ Add `args` argument to `server.script` operation
++ Add make `put_file` work with `doas` (@minusf)
++ Handle adding git config key-values with multiple lines (@gchazot)
+
+Fixed:
+
++ Add Ubuntu latest (22.04) to CI tests (@gchazot)
++ Fix codecov workflow (@ioO)
++ Escape & character during sed replacement during `line.replace` (@sysadmin75)
++ Fix last login time in `server.users` operation (@minusf)
++ Fix fact hash for short facts where the backing fact takes arguments
+
 # v2.6.2
 
 + Add support for classic confinment in `snap.packages` operation (@pabloxio)
 + Support dictionaries for Terraform connector inventory
 + Upgrade to `distro>1.6` and remove patch hack
 + Fix `files.Md5File` fact for BSD style output (@ScottKevill)
 + Fix handling of `protocol` in `iptables.rule` operation (@sysadmin75)
```

### Comparing `pyinfra-2.6.2/LICENSE.md` & `pyinfra-2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/PKG-INFO` & `pyinfra-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra
-Version: 2.6.2
+Version: 2.7
 Summary: pyinfra automates/provisions/manages/deploys infrastructure.
 Home-page: https://pyinfra.com
 Author: Nick / Fizzadar
 Author-email: pointlessrambler@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/Fizzadar/pyinfra
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra Version: 2.6.2 Summary: pyinfra automates/
+Metadata-Version: 2.1 Name: pyinfra Version: 2.7 Summary: pyinfra automates/
 provisions/manages/deploys infrastructure. Home-page: https://pyinfra.com
 Author: Nick / Fizzadar Author-email: pointlessrambler@gmail.com License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com Project-URL: GitHub,
 https://github.com/Fizzadar/pyinfra Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology Classifier: License ::
```

### Comparing `pyinfra-2.6.2/README.md` & `pyinfra-2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/__init__.py` & `pyinfra-2.7/pyinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/__init__.py` & `pyinfra-2.7/pyinfra/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/arguments.py` & `pyinfra-2.7/pyinfra/api/arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/command.py` & `pyinfra-2.7/pyinfra/api/command.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/config.py` & `pyinfra-2.7/pyinfra/api/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/connect.py` & `pyinfra-2.7/pyinfra/api/connect.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/connectors.py` & `pyinfra-2.7/pyinfra/api/connectors.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/deploy.py` & `pyinfra-2.7/pyinfra/api/deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/exceptions.py` & `pyinfra-2.7/pyinfra/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/facts.py` & `pyinfra-2.7/pyinfra/api/facts.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,18 @@
     def process_pipeline(self, args, output):
         return {arg: self.process([output[i]]) for i, arg in enumerate(args)}
 
 
 class ShortFactBase(metaclass=FactNameMeta):
     fact: Type[FactBase]
 
+    @staticmethod
+    def process_data(data):
+        return data
+
 
 def get_short_facts(state: "State", host: "Host", short_fact, **kwargs):
     fact_data = get_fact(state, host, short_fact.fact, **kwargs)
     return short_fact().process_data(fact_data)
 
 
 def _make_command(command_attribute, host_args):
@@ -189,14 +193,17 @@
         return get_short_facts(
             state,
             host,
             cls,
             args=args,
             kwargs=kwargs,
             ensure_hosts=ensure_hosts,
+            apply_failed_hosts=apply_failed_hosts,
+            fact_hash=fact_hash,
+            use_cache=use_cache,
         )
 
     with host.facts_lock:
         if use_cache and fact_hash and fact_hash in host.facts:
             return host.facts[fact_hash]
 
         return _get_fact(
@@ -328,14 +335,16 @@
 
     if fact_hash:
         host.facts[fact_hash] = data
     return data
 
 
 def _get_fact_hash(state: "State", host: "Host", cls, args, kwargs):
+    if issubclass(cls, ShortFactBase):
+        cls = cls.fact
     fact_kwargs, executor_kwargs = _handle_fact_kwargs(state, host, cls, args, kwargs)
     return make_hash((cls, fact_kwargs, executor_kwargs))
 
 
 def get_host_fact(
     state: "State",
     host: "Host",
```

### Comparing `pyinfra-2.6.2/pyinfra/api/host.py` & `pyinfra-2.7/pyinfra/api/host.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/inventory.py` & `pyinfra-2.7/pyinfra/api/inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/operation.py` & `pyinfra-2.7/pyinfra/api/operation.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/operations.py` & `pyinfra-2.7/pyinfra/api/operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/state.py` & `pyinfra-2.7/pyinfra/api/state.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/api/util.py` & `pyinfra-2.7/pyinfra/api/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/ansible.py` & `pyinfra-2.7/pyinfra/connectors/ansible.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/chroot.py` & `pyinfra-2.7/pyinfra/connectors/chroot.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/docker.py` & `pyinfra-2.7/pyinfra/connectors/docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/dockerssh.py` & `pyinfra-2.7/pyinfra/connectors/dockerssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/local.py` & `pyinfra-2.7/pyinfra/connectors/local.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/mech.py` & `pyinfra-2.7/pyinfra/connectors/mech.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/pyinfrawinrmsession/__init__.py` & `pyinfra-2.7/pyinfra/connectors/pyinfrawinrmsession/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/ssh.py` & `pyinfra-2.7/pyinfra/connectors/ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -466,18 +466,20 @@
             err=True,
         )
 
     return True
 
 
 def _put_file(host: "Host", filename_or_io, remote_location):
-    attempts = 1
+    logger.debug("Attempting upload of %s to %s", filename_or_io, remote_location)
+
+    attempts = 0
     last_e = None
 
-    while attempts < 4:
+    while attempts < 3:
         try:
             with get_file_io(filename_or_io) as file_io:
                 sftp = _get_sftp_connection(host)
                 sftp.putfo(file_io, remote_location)
             return
         except OSError as e:
             logger.warning(f"Failed to upload file, retrying: {e}")
@@ -492,37 +494,42 @@
     state: "State",
     host: "Host",
     filename_or_io,
     remote_filename,
     remote_temp_filename=None,
     sudo: bool = False,
     sudo_user=None,
+    doas: bool = False,
+    doas_user=None,
     su_user=None,
     print_output: bool = False,
     print_input: bool = False,
     **command_kwargs,
 ):
     """
     Upload file-ios to the specified host using SFTP. Supports uploading files
     with sudo by uploading to a temporary directory then moving & chowning.
     """
 
     # sudo/su are a little more complicated, as you can only sftp with the SSH
     # user connected, so upload to tmp and copy/chown w/sudo and/or su_user
-    if sudo or su_user:
+    if sudo or doas or su_user:
         # Get temp file location
         temp_file = remote_temp_filename or state.get_temp_filename(remote_filename)
         _put_file(host, filename_or_io, temp_file)
 
         # Make sure our sudo/su user can access the file
         if su_user:
             command = StringCommand("setfacl", "-m", "u:{0}:r".format(su_user), temp_file)
         elif sudo_user:
-            command = StringCommand("setfacl -m u:{0}:r".format(sudo_user), temp_file)
-        if su_user or sudo_user:
+            command = StringCommand("setfacl", "-m", "u:{0}:r".format(sudo_user), temp_file)
+        elif doas_user:
+            command = StringCommand("setfacl", "-m", "u:{0}:r".format(doas_user), temp_file)
+
+        if su_user or sudo_user or doas_user:
             status, _, stderr = run_shell_command(
                 state,
                 host,
                 command,
                 sudo=False,
                 print_output=print_output,
                 print_input=print_input,
@@ -538,14 +545,16 @@
 
         status, _, stderr = run_shell_command(
             state,
             host,
             command,
             sudo=sudo,
             sudo_user=sudo_user,
+            doas=doas,
+            doas_user=doas_user,
             su_user=su_user,
             print_output=print_output,
             print_input=print_input,
             **command_kwargs,
         )
 
         if status is False:
@@ -556,14 +565,15 @@
         command = StringCommand("rm", "-f", temp_file)
 
         status, _, stderr = run_shell_command(
             state,
             host,
             command,
             sudo=False,
+            doas=False,
             print_output=print_output,
             print_input=print_input,
             **command_kwargs,
         )
 
         if status is False:
             logger.error("Unable to remove temporary file: {0}".format("\n".join(stderr)))
```

### Comparing `pyinfra-2.6.2/pyinfra/connectors/sshuserclient/client.py` & `pyinfra-2.7/pyinfra/connectors/sshuserclient/client.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/sshuserclient/config.py` & `pyinfra-2.7/pyinfra/connectors/sshuserclient/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/terraform.py` & `pyinfra-2.7/pyinfra/connectors/terraform.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/util.py` & `pyinfra-2.7/pyinfra/connectors/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/vagrant.py` & `pyinfra-2.7/pyinfra/connectors/vagrant.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/connectors/winrm.py` & `pyinfra-2.7/pyinfra/connectors/winrm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/context.py` & `pyinfra-2.7/pyinfra/context.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/apt.py` & `pyinfra-2.7/pyinfra/facts/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/brew.py` & `pyinfra-2.7/pyinfra/facts/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/choco.py` & `pyinfra-2.7/pyinfra/facts/choco.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/deb.py` & `pyinfra-2.7/pyinfra/facts/deb.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/dnf.py` & `pyinfra-2.7/pyinfra/facts/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/docker.py` & `pyinfra-2.7/pyinfra/facts/docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/files.py` & `pyinfra-2.7/pyinfra/facts/files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/git.py` & `pyinfra-2.7/pyinfra/facts/git.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     @staticmethod
     def process(output):
         items = {}
 
         for line in output:
             key, value = line.split("=", 1)
-            items[key] = value
+            items.setdefault(key, []).append(value)
 
         return items
 
 
 class GitTrackingBranch(FactBase):
     requires_command = "git"
```

### Comparing `pyinfra-2.6.2/pyinfra/facts/gpg.py` & `pyinfra-2.7/pyinfra/facts/gpg.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/hardware.py` & `pyinfra-2.7/pyinfra/facts/hardware.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/iptables.py` & `pyinfra-2.7/pyinfra/facts/iptables.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/launchd.py` & `pyinfra-2.7/pyinfra/facts/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/mysql.py` & `pyinfra-2.7/pyinfra/facts/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/npm.py` & `pyinfra-2.7/pyinfra/facts/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/openrc.py` & `pyinfra-2.7/pyinfra/facts/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/pacman.py` & `pyinfra-2.7/pyinfra/facts/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/pip.py` & `pyinfra-2.7/pyinfra/facts/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/postgresql.py` & `pyinfra-2.7/pyinfra/facts/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/rpm.py` & `pyinfra-2.7/pyinfra/facts/rpm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/selinux.py` & `pyinfra-2.7/pyinfra/facts/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/server.py` & `pyinfra-2.7/pyinfra/facts/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,15 +420,15 @@
             },
         }
     """
 
     command = """
         for i in `cat /etc/passwd | cut -d: -f1`; do
             ENTRY=`grep ^$i: /etc/passwd`;
-            LASTLOG=`lastlog -u $i | grep ^$i` | tr -s ' ';
+            LASTLOG=`lastlog -u $i | grep ^$i | tr -s ' '`;
             echo "$ENTRY|`id -gn $i`|`id -Gn $i`|$LASTLOG";
         done
     """.strip()
 
     default = dict
 
     def process(self, output):
@@ -653,7 +653,26 @@
     """
 
     fact = LinuxGui
 
     @staticmethod
     def process_data(data):
         return len(data) > 0
+
+
+class Locales(FactBase):
+    """
+    Returns installed locales on the target host.
+
+    .. code:: python
+
+        ["C.UTF-8", "en_US.UTF-8"]
+    """
+
+    command = "locale -a"
+    requires_command = "locale"
+    default = list
+
+    def process(self, output):
+        # replace utf8 with UTF-8 to match names in /etc/locale.gen
+        # return a list of enabled locales
+        return [line.replace("utf8", "UTF-8") for line in output]
```

### Comparing `pyinfra-2.6.2/pyinfra/facts/snap.py` & `pyinfra-2.7/pyinfra/facts/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/systemd.py` & `pyinfra-2.7/pyinfra/facts/systemd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/sysvinit.py` & `pyinfra-2.7/pyinfra/facts/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/upstart.py` & `pyinfra-2.7/pyinfra/facts/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/util/__init__.py` & `pyinfra-2.7/pyinfra/facts/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/util/databases.py` & `pyinfra-2.7/pyinfra/facts/util/databases.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/util/packaging.py` & `pyinfra-2.7/pyinfra/facts/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/util/win_files.py` & `pyinfra-2.7/pyinfra/facts/util/win_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/vzctl.py` & `pyinfra-2.7/pyinfra/facts/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/windows.py` & `pyinfra-2.7/pyinfra/facts/windows.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/windows_files.py` & `pyinfra-2.7/pyinfra/facts/windows_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/yum.py` & `pyinfra-2.7/pyinfra/facts/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/facts/zypper.py` & `pyinfra-2.7/pyinfra/facts/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/local.py` & `pyinfra-2.7/pyinfra/local.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/apk.py` & `pyinfra-2.7/pyinfra/operations/apk.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/apt.py` & `pyinfra-2.7/pyinfra/operations/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/brew.py` & `pyinfra-2.7/pyinfra/operations/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/bsdinit.py` & `pyinfra-2.7/pyinfra/operations/bsdinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/choco.py` & `pyinfra-2.7/pyinfra/operations/choco.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/dnf.py` & `pyinfra-2.7/pyinfra/operations/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/files.py` & `pyinfra-2.7/pyinfra/operations/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,27 +241,29 @@
     present=True,
     replace=None,
     flags=None,
     backup=False,
     interpolate_variables=False,
     escape_regex_characters=False,
     assume_present=False,
+    ensure_newline=False,
 ):
     """
     Ensure lines in files using grep to locate and sed to replace.
 
     + path: target remote file to edit
     + line: string or regex matching the target line
     + present: whether the line should be in the file
     + replace: text to replace entire matching lines when ``present=True``
     + flags: list of flags to pass to sed when replacing/deleting
     + backup: whether to backup the file (see below)
     + interpolate_variables: whether to interpolate variables in ``replace``
     + assume_present: whether to assume a matching line already exists in the file
     + escape_regex_characters: whether to escape regex characters from the matching line
+    + ensure_newline: ensures that the appended line is on a new line
 
     Regex line matching:
         Unless line matches a line (starts with ^, ends $), pyinfra will wrap it such that
         it does, like: ``^.*LINE.*$``. This means we don't swap parts of lines out. To
         change bits of lines, see ``files.replace``.
 
     Regex line escaping:
@@ -273,14 +275,19 @@
         date (taken from the machine running ``pyinfra``) appended as the extension. If
         you pass a string value this will be used as the extension of the backed up file.
 
     Append:
         If ``line`` is not in the file but we want it (``present`` set to ``True``), then
         it will be append to the end of the file.
 
+    Ensure new line:
+        This will ensure that the ``line`` being appended is always on a seperate new
+        line in case the file doesn't end with a newline character.
+
+
     **Examples:**
 
     .. code:: python
 
         # prepare to do some maintenance
         maintenance_line = "SYSTEM IS DOWN FOR MAINTENANCE"
         files.line(
@@ -351,19 +358,26 @@
     if replace:
         line = replace
     # We must provide some kind of replace to sed_replace_command below
     else:
         replace = ""
 
     # Save commands for re-use in dynamic script when file not present at fact stage
-    echo_command = make_formatted_string_command(
-        "echo {0} >> {1}",
-        '"{0}"'.format(line) if interpolate_variables else QuoteString(line),
-        QuoteString(path),
-    )
+    if ensure_newline:
+        echo_command = make_formatted_string_command(
+            "( [ $(tail -c1 {1} | wc -l) -eq 0 ] && echo ; echo {0} ) >> {1}",
+            '"{0}"'.format(line) if interpolate_variables else QuoteString(line),
+            QuoteString(path),
+        )
+    else:
+        echo_command = make_formatted_string_command(
+            "echo {0} >> {1}",
+            '"{0}"'.format(line) if interpolate_variables else QuoteString(line),
+            QuoteString(path),
+        )
 
     if backup:
         backup_filename = "{0}.{1}".format(path, get_timestamp())
         echo_command = StringCommand(
             make_formatted_string_command(
                 "cp {0} {1} && ",
                 QuoteString(path),
```

### Comparing `pyinfra-2.6.2/pyinfra/operations/gem.py` & `pyinfra-2.7/pyinfra/operations/gem.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/git.py` & `pyinfra-2.7/pyinfra/operations/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 from . import files, ssh
 from .util.files import chown, unix_path_join
 
 
 @operation(
     pipeline_facts={"git_config": "repo"},
 )
-def config(key, value, repo=None):
+def config(key, value, multi_value=False, repo=None):
     """
     Manage git config for a repository or globally.
 
     + key: the key of the config to ensure
     + value: the value this key should have
+    + multi_value: Add the value rather than set it for settings that can have multiple values
     + repo: specify the git repo path to edit local config (defaults to global)
 
     **Example:**
 
     .. code:: python
 
         git.config(
@@ -42,21 +43,26 @@
     if not repo:
         existing_config = host.get_fact(GitConfig)
 
     # Only get the config if the repo exists at this stage
     elif host.get_fact(Directory, path=unix_path_join(repo, ".git")):
         existing_config = host.get_fact(GitConfig, repo=repo)
 
-    if existing_config.get(key) != value:
-        if repo is None:
-            yield 'git config --global {0} "{1}"'.format(key, value)
-        else:
-            yield 'cd {0} && git config --local {1} "{2}"'.format(repo, key, value)
+    if repo is None:
+        base_command = "git config --global"
+    else:
+        base_command = "cd {0} && git config --local".format(repo)
 
-        existing_config[key] = value
+    if not multi_value and existing_config.get(key) != [value]:
+        yield '{0} {1} "{2}"'.format(base_command, key, value)
+        existing_config[key] = [value]
+
+    elif multi_value and value not in existing_config.get(key, []):
+        yield '{0} --add {1} "{2}"'.format(base_command, key, value)
+        existing_config.setdefault(key, []).append(value)
 
     else:
         host.noop("git config {0} is set to {1}".format(key, value))
 
 
 @operation(
     pipeline_facts={"git_branch": "target"},
```

### Comparing `pyinfra-2.6.2/pyinfra/operations/iptables.py` & `pyinfra-2.7/pyinfra/operations/iptables.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/launchd.py` & `pyinfra-2.7/pyinfra/operations/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/lxd.py` & `pyinfra-2.7/pyinfra/operations/lxd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/mysql.py` & `pyinfra-2.7/pyinfra/operations/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/npm.py` & `pyinfra-2.7/pyinfra/operations/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/openrc.py` & `pyinfra-2.7/pyinfra/operations/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/pacman.py` & `pyinfra-2.7/pyinfra/operations/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/pip.py` & `pyinfra-2.7/pyinfra/operations/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/pkg.py` & `pyinfra-2.7/pyinfra/operations/pkg.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/pkgin.py` & `pyinfra-2.7/pyinfra/operations/pkgin.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/postgresql.py` & `pyinfra-2.7/pyinfra/operations/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/puppet.py` & `pyinfra-2.7/pyinfra/operations/puppet.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/python.py` & `pyinfra-2.7/pyinfra/operations/python.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/selinux.py` & `pyinfra-2.7/pyinfra/operations/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/server.py` & `pyinfra-2.7/pyinfra/operations/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 
 import shlex
 from io import StringIO
 from itertools import filterfalse, tee
 from os import path
 from time import sleep
 
-from pyinfra import host, state
+from pyinfra import host, logger, state
 from pyinfra.api import FunctionCommand, OperationError, StringCommand, operation
 from pyinfra.api.util import try_int
 from pyinfra.connectors.util import remove_any_sudo_askpass_file
-from pyinfra.facts.files import Directory, Link
+from pyinfra.facts.files import Directory, FindInFile, Link
 from pyinfra.facts.server import (
     Crontab,
     Groups,
     Hostname,
     KernelModules,
+    Locales,
     Mounts,
     Os,
     Sysctl,
     Users,
     Which,
 )
 
@@ -151,36 +152,44 @@
         commands = [commands]
 
     for command in commands:
         yield command
 
 
 @operation(is_idempotent=False)
-def script(src):
+def script(src, args=()):
     """
     Upload and execute a local script on the remote host.
 
     + src: local script filename to upload & execute
+    + args: iterable to pass as arguments to the script
 
     **Example:**
 
     .. code:: python
 
         # Note: This assumes there is a file in files/hello.bash locally.
         server.script(
             name="Hello",
             src="files/hello.bash",
         )
+
+        # Example passing arguments to the script
+        server.script(
+            name="Hello",
+            src="files/hello.bash",
+            args=("do-something", "with-this"),
+        )
     """
 
     temp_file = state.get_temp_filename()
     yield from files.put(src, temp_file)
 
     yield chmod(temp_file, "+x")
-    yield temp_file
+    yield StringCommand(temp_file, *args)
 
 
 @operation(is_idempotent=False)
 def script_template(src, **data):
     """
     Generate, upload and execute a local script template on the remote host.
 
@@ -895,15 +904,15 @@
             user=user,
             group=group or user,
             mode=600,
         )
 
         # And every public key is present
         for key in public_keys:
-            yield from files.line(path=authorized_key_file, line=key)
+            yield from files.line(path=authorized_key_file, line=key, ensure_newline=True)
 
 
 @operation
 def user(
     user,
     present=True,
     home=None,
@@ -1096,7 +1105,77 @@
             user,
             public_keys,
             group=group,
             delete_keys=delete_keys,
             authorized_key_directory="{0}/.ssh".format(home),
             authorized_key_filename=None,
         )
+
+
+@operation
+def locale(
+    locale,
+    present=True,
+):
+    """
+    Enable/Disable locale.
+
+    + locale: name of the locale to enable/disable
+    + present: whether this locale should be present or not
+
+    **Examples:**
+
+    .. code:: python
+
+        server.locale(
+            name="Ensure en_GB.UTF-8 locale is not present",
+            locale="en_GB.UTF-8",
+            present=False,
+        )
+
+        server.locale(
+            name="Ensure en_GB.UTF-8 locale is present",
+            locale="en_GB.UTF-8",
+        )
+
+    """
+
+    locales = host.get_fact(Locales)
+
+    logger.debug("Enabled locales: {0}".format(locales))
+
+    locales_definitions_file = "/etc/locale.gen"
+
+    # Find the matching line in /etc/locale.gen
+    matching_lines = host.get_fact(
+        FindInFile, path=locales_definitions_file, pattern=rf"^.*{locale}[[:space:]]\+.*$"
+    )
+
+    if not matching_lines:
+        raise OperationError(f"Locale {locale} not found in {locales_definitions_file}")
+
+    if len(matching_lines) > 1:
+        raise OperationError(f"Multiple locales matches for {locale} in {locales_definitions_file}")
+
+    matching_line = matching_lines[0]
+
+    # Remove locale
+    if not present and locale in locales:
+        logger.debug(f"Removing locale {locale}")
+
+        yield from files.line(
+            path=locales_definitions_file, line=f"^{matching_line}$", replace=f"# {matching_line}"
+        )
+
+        yield "locale-gen"
+
+    # Add locale
+    if present and locale not in locales:
+        logger.debug(f"Adding locale {locale}")
+
+        yield from files.replace(
+            path=locales_definitions_file,
+            text=f"^{matching_line}$",
+            replace=f"{matching_line}".replace("# ", ""),
+        )
+
+        yield "locale-gen"
```

### Comparing `pyinfra-2.6.2/pyinfra/operations/snap.py` & `pyinfra-2.7/pyinfra/operations/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/ssh.py` & `pyinfra-2.7/pyinfra/operations/ssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/systemd.py` & `pyinfra-2.7/pyinfra/operations/systemd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/sysvinit.py` & `pyinfra-2.7/pyinfra/operations/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/upstart.py` & `pyinfra-2.7/pyinfra/operations/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/util/files.py` & `pyinfra-2.7/pyinfra/operations/util/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     interpolate_variables=False,
 ):
     flags = "".join(flags) if flags else ""
 
     line = line.replace("/", r"\/")
     replace = str(replace)
     replace = replace.replace("/", r"\/")
+    replace = replace.replace("&", r"\&")
     backup_extension = get_timestamp()
 
     if interpolate_variables:
         line = line.replace('"', '\\"')
         replace = replace.replace('"', '\\"')
         sed_script_formatter = '"s/{0}/{1}/{2}"'
     else:
```

### Comparing `pyinfra-2.6.2/pyinfra/operations/util/packaging.py` & `pyinfra-2.7/pyinfra/operations/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/util/service.py` & `pyinfra-2.7/pyinfra/operations/util/service.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/vzctl.py` & `pyinfra-2.7/pyinfra/operations/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/windows.py` & `pyinfra-2.7/pyinfra/operations/windows.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/windows_files.py` & `pyinfra-2.7/pyinfra/operations/windows_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/xbps.py` & `pyinfra-2.7/pyinfra/operations/xbps.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/yum.py` & `pyinfra-2.7/pyinfra/operations/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/operations/zypper.py` & `pyinfra-2.7/pyinfra/operations/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra/progress.py` & `pyinfra-2.7/pyinfra/progress.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra.egg-info/PKG-INFO` & `pyinfra-2.7/pyinfra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra
-Version: 2.6.2
+Version: 2.7
 Summary: pyinfra automates/provisions/manages/deploys infrastructure.
 Home-page: https://pyinfra.com
 Author: Nick / Fizzadar
 Author-email: pointlessrambler@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/Fizzadar/pyinfra
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra Version: 2.6.2 Summary: pyinfra automates/
+Metadata-Version: 2.1 Name: pyinfra Version: 2.7 Summary: pyinfra automates/
 provisions/manages/deploys infrastructure. Home-page: https://pyinfra.com
 Author: Nick / Fizzadar Author-email: pointlessrambler@gmail.com License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com Project-URL: GitHub,
 https://github.com/Fizzadar/pyinfra Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology Classifier: License ::
```

### Comparing `pyinfra-2.6.2/pyinfra.egg-info/SOURCES.txt` & `pyinfra-2.7/pyinfra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 pyinfra/connectors/sshuserclient/client.py
 pyinfra/connectors/sshuserclient/config.py
 pyinfra/facts/__init__.py
 pyinfra/facts/apk.py
 pyinfra/facts/apt.py
 pyinfra/facts/brew.py
 pyinfra/facts/bsdinit.py
+pyinfra/facts/cargo.py
 pyinfra/facts/choco.py
 pyinfra/facts/deb.py
 pyinfra/facts/dnf.py
 pyinfra/facts/docker.py
 pyinfra/facts/files.py
 pyinfra/facts/gem.py
 pyinfra/facts/git.py
@@ -91,14 +92,15 @@
 pyinfra/facts/util/packaging.py
 pyinfra/facts/util/win_files.py
 pyinfra/operations/__init__.py
 pyinfra/operations/apk.py
 pyinfra/operations/apt.py
 pyinfra/operations/brew.py
 pyinfra/operations/bsdinit.py
+pyinfra/operations/cargo.py
 pyinfra/operations/choco.py
 pyinfra/operations/dnf.py
 pyinfra/operations/files.py
 pyinfra/operations/gem.py
 pyinfra/operations/git.py
 pyinfra/operations/iptables.py
 pyinfra/operations/launchd.py
@@ -128,24 +130,28 @@
 pyinfra/operations/zypper.py
 pyinfra/operations/util/__init__.py
 pyinfra/operations/util/files.py
 pyinfra/operations/util/packaging.py
 pyinfra/operations/util/service.py
 pyinfra_cli/__init__.py
 pyinfra_cli/__main__.py
+pyinfra_cli/commands.py
 pyinfra_cli/exceptions.py
 pyinfra_cli/inventory.py
 pyinfra_cli/log.py
 pyinfra_cli/main.py
 pyinfra_cli/prints.py
 pyinfra_cli/util.py
 pyinfra_cli/virtualenv.py
 tests/__init__.py
 tests/paramiko_util.py
 tests/test_facts.py
+tests/test_global_arguments.py
+tests/test_operations.py
+tests/test_operations_utils.py
 tests/util.py
 tests/test_api/__init__.py
 tests/test_api/test_api.py
 tests/test_api/test_api_arguments.py
 tests/test_api/test_api_command.py
 tests/test_api/test_api_config.py
 tests/test_api/test_api_deploys.py
```

### Comparing `pyinfra-2.6.2/pyinfra.egg-info/requires.txt` & `pyinfra-2.7/pyinfra.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 [ansible]
 pyyaml
 
 [dev]
 pyyaml
 pytest-cov==4.0.0
-codecov==2.1.12
 black==22.3.0
 isort==5.10.1
 flake8==4.0.1
 flake8-black==0.3.0
 flake8-isort==4.1.1
 mypy==0.971
 types-cryptography
@@ -55,15 +54,14 @@
 recommonmark==0.5.0
 sphinx==2.2.1
 docutils==0.17.1
 
 [test]
 pyyaml
 pytest-cov==4.0.0
-codecov==2.1.12
 black==22.3.0
 isort==5.10.1
 flake8==4.0.1
 flake8-black==0.3.0
 flake8-isort==4.1.1
 mypy==0.971
 types-cryptography
```

### Comparing `pyinfra-2.6.2/pyinfra_cli/__main__.py` & `pyinfra-2.7/pyinfra_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra_cli/exceptions.py` & `pyinfra-2.7/pyinfra_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra_cli/inventory.py` & `pyinfra-2.7/pyinfra_cli/inventory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from collections import defaultdict
 from os import listdir, path
 from types import GeneratorType
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
 from pyinfra import logger
 from pyinfra.api.inventory import Inventory
 from pyinfra.context import ctx_inventory
-from pyinfra_cli.util import exec_file
+
+from .exceptions import CliError
+from .util import exec_file, try_import_module_attribute
+
+HostType = Union[str, Tuple[str, Dict]]
 
 # Hosts in an inventory can be just the hostname or a tuple (hostname, data)
 ALLOWED_HOST_TYPES = (str, tuple)
 
 
 def _is_inventory_group(key: str, value: Any):
     """
@@ -64,15 +68,93 @@
 
 def _get_groups_from_filename(inventory_filename: str):
     attrs = exec_file(inventory_filename, return_locals=True)
 
     return {key: value for key, value in attrs.items() if _is_inventory_group(key, value)}
 
 
+T = TypeVar("T")
+
+
+def _get_any_tuple_first(item: Union[T, Tuple[T, Any]]) -> T:
+    return item[0] if isinstance(item, tuple) else item
+
+
 def make_inventory(
+    inventory: str,
+    override_data=None,
+    cwd: Optional[str] = None,
+    group_data_directories=None,
+):
+    # First, try loading the inventory as if it's a Python import function
+    try:
+        inventory_func = try_import_module_attribute(inventory)
+    except (CliError, ValueError):
+        # If not an import, load as if from the filesystem *or* comma separated list, which also
+        # loads any all.py group data files (imported functions do not load group data).
+        return make_inventory_from_files(inventory, override_data, cwd, group_data_directories)
+    else:
+        return make_inventory_from_func(inventory_func, override_data)
+
+
+def make_inventory_from_func(
+    inventory_func: Callable[[], Dict[str, List[HostType]]],
+    override_data: Optional[Dict[Any, Any]] = None,
+):
+    logger.warning("Loading inventory via import function is in alpha!")
+
+    try:
+        groups = inventory_func()
+    except Exception as e:
+        raise CliError(f"Failed to load inventory function: {inventory_func.__name__}: {e}")
+
+    if not isinstance(groups, dict):
+        raise TypeError(f"Inventory function {inventory_func.__name__} did not return a dictionary")
+
+    # TODO: this shouldn't be required to make an inventory, groups should suffice
+    combined_host_list = set()
+    groups_with_data: Dict[str, Tuple[List[HostType], Dict]] = {}
+
+    for key, hosts in groups.items():
+        data: Dict = {}
+
+        if isinstance(hosts, tuple):
+            hosts, data = hosts
+
+        if not isinstance(data, dict):
+            raise TypeError(
+                f"Inventory function {inventory_func.__name__} "
+                f"group contains non-dictionary data: {key}"
+            )
+
+        for host in hosts:
+            if not isinstance(host, ALLOWED_HOST_TYPES):
+                raise TypeError(
+                    f"Inventory function {inventory_func.__name__} invalid host: {host}"
+                )
+
+            host = _get_any_tuple_first(host)
+
+            if not isinstance(host, str):
+                raise TypeError(
+                    f"Inventory function {inventory_func.__name__} invalid host name: {host}"
+                )
+
+            combined_host_list.add(host)
+
+        groups_with_data[key] = (hosts, data)
+
+    return Inventory(
+        (list(combined_host_list), {}),
+        override_data=override_data,
+        **groups_with_data,
+    )
+
+
+def make_inventory_from_files(
     inventory_filename: str,
     override_data=None,
     cwd: Optional[str] = None,
     group_data_directories=None,
 ):
     """
     Builds a ``pyinfra.api.Inventory`` from the filesystem. If the file does not exist
@@ -104,19 +186,19 @@
             all_hosts, all_data = all_hosts
 
     # Build all out of the existing hosts if not defined
     else:
         all_hosts = []
         for hosts in groups.values():
             # Groups can be a list of hosts or tuple of (hosts, data)
-            hosts = hosts[0] if isinstance(hosts, tuple) else hosts
+            hosts = _get_any_tuple_first(hosts)
 
             for host in hosts:
                 # Hosts can be a hostname or tuple of (hostname, data)
-                hostname = host[0] if isinstance(host, tuple) else host
+                hostname = _get_any_tuple_first(host)
 
                 if hostname not in all_hosts:
                     all_hosts.append(hostname)
 
     groups["all"] = (all_hosts, all_data)
 
     # Apply the filename group if not already defined
@@ -169,11 +251,8 @@
 
     # Loop back through any leftover group data and create an empty (for now)
     # group - this is because inventory @connectors can attach arbitrary groups
     # to hosts, so we need to support that.
     for name, data in group_data.items():
         groups[name] = ([], data)
 
-    return (
-        Inventory(groups.pop("all"), override_data=override_data, **groups),
-        file_groupname and file_groupname.lower(),
-    )
+    return Inventory(groups.pop("all"), override_data=override_data, **groups)
```

### Comparing `pyinfra-2.6.2/pyinfra_cli/log.py` & `pyinfra-2.7/pyinfra_cli/log.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra_cli/main.py` & `pyinfra-2.7/pyinfra_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,34 +13,28 @@
 from pyinfra.api.exceptions import NoGroupError, PyinfraError
 from pyinfra.api.facts import get_facts
 from pyinfra.api.operations import run_ops
 from pyinfra.api.util import get_kwargs_str
 from pyinfra.context import ctx_config, ctx_inventory, ctx_state
 from pyinfra.operations import server
 
+from .commands import get_facts_and_args, get_func_and_args
 from .exceptions import CliError, UnexpectedExternalError, UnexpectedInternalError
 from .inventory import make_inventory
 from .log import setup_logging
 from .prints import (
     print_facts,
     print_inventory,
     print_meta,
     print_results,
     print_state_facts,
     print_state_operations,
     print_support_info,
 )
-from .util import (
-    exec_file,
-    get_facts_and_args,
-    get_func_and_args,
-    load_deploy_file,
-    load_func,
-    parse_cli_arg,
-)
+from .util import exec_file, load_deploy_file, load_func, parse_cli_arg
 from .virtualenv import init_virtualenv
 
 
 def _exit():
     if ctx_state.isset() and state.failed_hosts:
         sys.exit(1)
     sys.exit(0)
@@ -334,15 +328,15 @@
         winrm_port,
         winrm_transport,
     )
 
     # Load up the inventory from the filesystem
     #
     echo_msg("--> Loading inventory...", quiet)
-    inventory, inventory_group = make_inventory(
+    inventory = make_inventory(
         inventory,
         cwd=state.cwd,
         override_data=override_data,
         group_data_directories=group_data,
     )
     ctx_inventory.set(inventory)
```

### Comparing `pyinfra-2.6.2/pyinfra_cli/prints.py` & `pyinfra-2.7/pyinfra_cli/prints.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyinfra_cli/util.py` & `pyinfra-2.7/pyinfra_cli/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -129,96 +129,38 @@
         return json.loads(arg)
     except ValueError:
         pass
 
     return arg
 
 
-def get_func_and_args(commands):
-    operation_name = commands[0]
+def try_import_module_attribute(path, prefix=None):
+    mod_path, attr_name = path.rsplit(".", 1)
+    module = None
 
-    # Get the module & operation name
-    op_module, op_name = operation_name.rsplit(".", 1)
-
-    # Try to load the requested operation from the main operations package.
-    # If that fails, try to load from the user's operations package.
-    try:
-        op_module = import_module("pyinfra.operations.{0}".format(op_module))
-    except ImportError:
-        try:
-            op_module = import_module(op_module)
-        except ImportError:
-            raise CliError("No such module: {0}".format(op_module))
-
-    op = getattr(op_module, op_name, None)
-    if not op:
-        raise CliError("No such operation: {0}".format(operation_name))
-
-    # Parse the arguments
-    operation_args = commands[1:]
-
-    if len(operation_args) == 1:
-        # Check if we're JSON (in which case we expect a list of two items:
-        # a list of args and a dict of kwargs).
+    if prefix:
+        full_path = f"{prefix}.{mod_path}"
         try:
-            args, kwargs = json.loads(operation_args[0])
-            return op, (args or (), kwargs or {})
-        except ValueError:
+            module = import_module(full_path)
+        except (ModuleNotFoundError, ImportError):
             pass
+    else:
+        full_path = mod_path
 
-    args = [parse_cli_arg(arg) for arg in operation_args if "=" not in arg]
-
-    kwargs = {
-        key: parse_cli_arg(value)
-        for key, value in [arg.split("=", 1) for arg in operation_args if "=" in arg]
-    }
-
-    return op, (args, kwargs)
-
-
-def get_facts_and_args(commands):
-    facts = []
-
-    current_fact = None
-
-    for command in commands:
-        if "=" in command:
-            if not current_fact:
-                raise CliError("Invalid fact commands: `{0}`".format(commands))
-
-            key, value = command.split("=", 1)
-            current_fact[2][key] = value
-            continue
-
-        if current_fact:
-            facts.append(current_fact)
-            current_fact = None
-
-        if "." not in command:
-            raise CliError(f"Invalid fact: `{command}`, should be in the format `module.cls`")
-
-        fact_module, fact_name = command.rsplit(".", 1)
+    if module is None:
         try:
-            fact_module = import_module("pyinfra.facts.{0}".format(fact_module))
-        except ImportError:
-            try:
-                fact_module = import_module(str(fact_module))
-            except ImportError:
-                raise CliError("No such module: `{0}`".format(fact_module))
-
-        fact_cls = getattr(fact_module, fact_name, None)
-        if not fact_cls:
-            raise CliError("No such fact: `{0}`".format(command))
-
-        current_fact = (fact_cls, (), {})
-
-    if current_fact:
-        facts.append(current_fact)
+            module = import_module(mod_path)
+        except (ModuleNotFoundError, ImportError):
+            raise CliError(f"No such module: {full_path}")
+
+    attr = getattr(module, attr_name, None)
+    if attr is None:
+        raise CliError(f"No such attribute in module {full_path}: {attr_name}")
 
-    return facts
+    return attr
 
 
 def _parallel_load_hosts(state: "State", callback: Callable, name: str):
     def load_file(local_host):
         try:
             with ctx_config.use(state.config.copy()):
                 with ctx_host.use(local_host):
```

### Comparing `pyinfra-2.6.2/pyinfra_cli/virtualenv.py` & `pyinfra-2.7/pyinfra_cli/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/pyproject.toml` & `pyinfra-2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/setup.cfg` & `pyinfra-2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/setup.py` & `pyinfra-2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     # Unit testing
     # TODO: drop Python 3.6 support
     'pytest==7.0.1 ; python_version <= "3.6"',
     'coverage==6.2 ; python_version <= "3.6"',
     'pytest==7.2.0 ; python_version > "3.6"',
     'coverage==6.5 ; python_version > "3.6"',
     "pytest-cov==4.0.0",
-    "codecov==2.1.12",
     # Formatting & linting
     "black==22.3.0",
     "isort==5.10.1",
     "flake8==4.0.1",
     "flake8-black==0.3.0",
     "flake8-isort==4.1.1",
     # Typing
```

### Comparing `pyinfra-2.6.2/tests/paramiko_util.py` & `pyinfra-2.7/tests/paramiko_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api.py` & `pyinfra-2.7/tests/test_api/test_api.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_arguments.py` & `pyinfra-2.7/tests/test_api/test_api_arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_command.py` & `pyinfra-2.7/tests/test_api/test_api_command.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_config.py` & `pyinfra-2.7/tests/test_api/test_api_config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_deploys.py` & `pyinfra-2.7/tests/test_api/test_api_deploys.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_facts.py` & `pyinfra-2.7/tests/test_api/test_api_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_host.py` & `pyinfra-2.7/tests/test_api/test_api_host.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_inventory.py` & `pyinfra-2.7/tests/test_api/test_api_inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_operations.py` & `pyinfra-2.7/tests/test_api/test_api_operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_api/test_api_util.py` & `pyinfra-2.7/tests/test_api/test_api_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_cli/test_cli.py` & `pyinfra-2.7/tests/test_cli/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,24 +95,24 @@
     def test_invalid_fact_module(self):
         result = run_cli(
             path.join("tests", "deploy", "inventories", "inventory.py"),
             "fact",
             "not_a_module.NotAFact",
         )
         assert result.exit_code == 1, result.stdout
-        assert "No such module: `not_a_module`" in result.stdout
+        assert "No such module: pyinfra.facts.not_a_module" in result.stdout
 
     def test_invalid_fact_class(self):
         result = run_cli(
             path.join("tests", "deploy", "inventories", "inventory.py"),
             "fact",
             "server.NotAFact",
         )
         assert result.exit_code == 1, result.stdout
-        assert "No such fact: `server.NotAFact`" in result.stdout
+        assert "No such attribute in module pyinfra.facts.server: NotAFact" in result.stdout
 
 
 class TestExecCli(PatchSSHTestCase):
     def test_exec_command(self):
         result = run_cli(
             path.join("tests", "deploy", "inventories", "inventory.py"),
             "exec",
```

### Comparing `pyinfra-2.6.2/tests/test_cli/test_cli_deploy.py` & `pyinfra-2.7/tests/test_cli/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_cli/test_cli_exceptions.py` & `pyinfra-2.7/tests/test_cli/test_cli_exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             ["my-server.net", "fact", "thing"],
             "Invalid fact: `thing`, should be in the format `module.cls`",
         )
 
     def test_no_fact_module(self):
         self.assert_cli_exception(
             ["my-server.net", "fact", "not_a_module.SomeFact"],
-            "No such module: `not_a_module`",
+            "No such module: pyinfra.facts.not_a_module",
         )
 
     def test_no_fact_cls(self):
         self.assert_cli_exception(
             ["my-server.net", "fact", "server.NotAFact"],
-            "No such fact: `server.NotAFact`",
+            "No such attribute in module pyinfra.facts.server: NotAFact",
         )
```

### Comparing `pyinfra-2.6.2/tests/test_cli/test_cli_util.py` & `pyinfra-2.7/tests/test_cli/test_cli_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from datetime import datetime
 from io import StringIO
 from unittest import TestCase
 
 import pytest
 
 from pyinfra.operations import server
+from pyinfra_cli.commands import get_func_and_args
 from pyinfra_cli.exceptions import CliError
-from pyinfra_cli.util import get_func_and_args, json_encode
+from pyinfra_cli.util import json_encode
 
 
 class TestCliUtil(TestCase):
     def test_json_encode_function(self):
         assert json_encode(get_func_and_args) == "Function: get_func_and_args"
 
     def test_json_encode_datetime(self):
@@ -25,21 +26,23 @@
 
     def test_json_encode_set(self):
         assert json_encode({1, 2, 3}) == [1, 2, 3]
 
     def test_setup_no_module(self):
         with self.assertRaises(CliError) as context:
             get_func_and_args(("no.op",))
-        assert context.exception.message == "No such module: no"
+        assert context.exception.message == "No such module: pyinfra.operations.no"
 
     def test_setup_no_op(self):
         with self.assertRaises(CliError) as context:
             get_func_and_args(("server.no",))
 
-        assert context.exception.message == "No such operation: server.no"
+        assert (
+            context.exception.message == "No such attribute in module pyinfra.operations.server: no"
+        )
 
     def test_setup_op_and_args(self):
         commands = ("pyinfra.operations.server.user", "one", "two", "hello=world")
 
         assert get_func_and_args(commands) == (
             server.user,
             (["one", "two"], {"hello": "world"}),
```

### Comparing `pyinfra-2.6.2/tests/test_cli/test_context_objects.py` & `pyinfra-2.7/tests/test_cli/test_context_objects.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_ansible.py` & `pyinfra-2.7/tests/test_connectors/test_ansible.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_chroot.py` & `pyinfra-2.7/tests/test_connectors/test_chroot.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_docker.py` & `pyinfra-2.7/tests/test_connectors/test_docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_dockerssh.py` & `pyinfra-2.7/tests/test_connectors/test_dockerssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_local.py` & `pyinfra-2.7/tests/test_connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_mech.py` & `pyinfra-2.7/tests/test_connectors/test_mech.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_ssh.py` & `pyinfra-2.7/tests/test_connectors/test_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
     def test_connect_with_rsa_ssh_key(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
         with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
             "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
         ) as fake_key_open:
-
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             connect_all(state)
 
             # Check the key was created properly
             fake_key_open.assert_called_with(filename="testkey")
@@ -177,15 +176,14 @@
 
     def test_connect_with_rsa_ssh_key_missing_password(self):
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
         with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
             "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
         ) as fake_key_open:
-
             fake_key_open.side_effect = make_raise_exception_function(PasswordRequiredException)
 
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             with self.assertRaises(PyinfraError) as e:
                 connect_all(state)
@@ -239,15 +237,14 @@
         state = State(make_inventory(hosts=(("somehost", {"ssh_key": "testkey"}),)), Config())
 
         with patch("pyinfra.connectors.ssh.path.isfile", lambda *args, **kwargs: True), patch(
             "pyinfra.connectors.ssh.RSAKey.from_private_key_file",
         ) as fake_rsa_key_open, patch(
             "pyinfra.connectors.ssh.DSSKey.from_private_key_file",
         ) as fake_key_open:  # noqa
-
             fake_rsa_key_open.side_effect = make_raise_exception_function(SSHException)
 
             fake_key = MagicMock()
             fake_key_open.return_value = fake_key
 
             connect_all(state)
 
@@ -629,17 +626,85 @@
                 print_output=True,
                 sudo=True,
                 sudo_user="ubuntu",
             )
 
         assert status is True
 
-        fake_ssh_client().exec_command.assert_called_with(
-            ("sh -c 'rm -f " "/tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24'"),
-            get_pty=False,
+        fake_ssh_client().exec_command.assert_has_calls(
+            [
+                call(
+                    (
+                        "sh -c 'setfacl -m u:ubuntu:r "
+                        "/tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24'"
+                    ),
+                    get_pty=False,
+                ),
+                call(
+                    (
+                        "sudo -H -n -u ubuntu sh -c 'cp /tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24 '\"'\"'not another file'\"'\"''"  # noqa: E501
+                    ),
+                    get_pty=False,
+                ),
+                call(
+                    ("sh -c 'rm -f /tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24'"),
+                    get_pty=False,
+                ),
+            ],
+        )
+
+        fake_sftp_client.from_transport().putfo.assert_called_with(
+            fake_open(),
+            "/tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24",
+        )
+
+    @patch("pyinfra.connectors.ssh.SSHClient")
+    @patch("pyinfra.connectors.ssh.SFTPClient")
+    def test_put_file_doas(self, fake_sftp_client, fake_ssh_client):
+        inventory = make_inventory(hosts=("anotherhost",))
+        State(inventory, Config())
+        host = inventory.get_host("anotherhost")
+        host.connect()
+
+        stdout_mock = MagicMock()
+        stdout_mock.channel.recv_exit_status.return_value = 0
+        fake_ssh_client().exec_command.return_value = MagicMock(), stdout_mock, MagicMock()
+
+        fake_open = mock_open(read_data="test!")
+        with patch("pyinfra.api.util.open", fake_open, create=True):
+            status = host.put_file(
+                "not-a-file",
+                "not another file",
+                print_output=True,
+                doas=True,
+                doas_user="ubuntu",
+            )
+
+        assert status is True
+
+        fake_ssh_client().exec_command.assert_has_calls(
+            [
+                call(
+                    (
+                        "sh -c 'setfacl -m u:ubuntu:r "
+                        "/tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24'"
+                    ),
+                    get_pty=False,
+                ),
+                call(
+                    (
+                        "doas -n -u ubuntu sh -c 'cp /tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24 '\"'\"'not another file'\"'\"''"  # noqa: E501
+                    ),
+                    get_pty=False,
+                ),
+                call(
+                    ("sh -c 'rm -f /tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24'"),
+                    get_pty=False,
+                ),
+            ],
         )
 
         fake_sftp_client.from_transport().putfo.assert_called_with(
             fake_open(),
             "/tmp/pyinfra-de01e82cb691e8a31369da3c7c8f17341c44ac24",
         )
```

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_sshuserclient.py` & `pyinfra-2.7/tests/test_connectors/test_sshuserclient.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_terraform.py` & `pyinfra-2.7/tests/test_connectors/test_terraform.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_util.py` & `pyinfra-2.7/tests/test_connectors/test_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_vagrant.py` & `pyinfra-2.7/tests/test_connectors/test_vagrant.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_connectors/test_winrm.py` & `pyinfra-2.7/tests/test_connectors/test_winrm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/test_facts.py` & `pyinfra-2.7/tests/test_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra-2.6.2/tests/util.py` & `pyinfra-2.7/tests/util.py`

 * *Files identical despite different names*

