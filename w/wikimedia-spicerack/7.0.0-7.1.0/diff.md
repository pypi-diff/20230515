# Comparing `tmp/wikimedia-spicerack-7.0.0.tar.gz` & `tmp/wikimedia-spicerack-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimedia-spicerack-7.0.0.tar", last modified: Mon May  8 16:46:43 2023, max compression
+gzip compressed data, was "wikimedia-spicerack-7.1.0.tar", last modified: Mon May 15 08:08:23 2023, max compression
```

## Comparing `wikimedia-spicerack-7.0.0.tar` & `wikimedia-spicerack-7.1.0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.688488 wikimedia-spicerack-7.0.0/
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/.git-blame-ignore-revs
--rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/.mailmap
--rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)   105356 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-08 16:46:43.688860 wikimedia-spicerack-7.0.0/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.880379 wikimedia-spicerack-7.0.0/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.881397 wikimedia-spicerack-7.0.0/doc/examples/
--rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/examples/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.899994 wikimedia-spicerack-7.0.0/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.906083 wikimedia-spicerack-7.0.0/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/_static/theme_overrides.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.070043 wikimedia-spicerack-7.0.0/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.administrative.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.alerting.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.alertmanager.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.apt.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.confctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.debmonitor.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.dhcp.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.dnsdisc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.elasticsearch_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.ganeti.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.icinga.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.ipmi.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.k8s.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.kafka.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mediawiki.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mysql.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mysql_legacy.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.netbox.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.peeringdb.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.puppet.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.redfish.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.redis_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.remote.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.reposync.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.service.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.toolforge.etcdctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.toolforge.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.typing.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/configuration.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/development.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/docutils.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     9572 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/pyproject.toml
--rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-05-08 16:46:43.697942 wikimedia-spicerack-7.0.0/setup.cfg
--rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/setup.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.272551 wikimedia-spicerack-7.0.0/spicerack/
--rw-r--r--   0 riccardo   (501) staff       (20)    27623 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/_log.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_menu.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_module_api.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3949 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10442 2023-05-04 08:02:07.000000 wikimedia-spicerack-7.0.0/spicerack/dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13883 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.0.0/spicerack/redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27921 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.298973 wikimedia-spicerack-7.0.0/spicerack/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.313471 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.317026 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/
--rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/schema.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.318224 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config/valid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.812885 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.337922 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.367670 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
--rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
--rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
--rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.377674 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
--rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.384063 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.406166 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
--rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.444137 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
--rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.445600 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.448918 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
--rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
--rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
--rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
--rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
--rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
--rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
--rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.452151 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.454216 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/debmonitor/
--rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/debmonitor/config.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.455480 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/discovery/
--rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/discovery/authdns.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.461750 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/elasticsearch/
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/elasticsearch/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.819426 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.474676 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
--rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.477553 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.482027 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/
--rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.484877 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
--rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.508703 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/404.json
--rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/bogus.json
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/info.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/instance.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.525046 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/
--rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_downtimed.json
--rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_invalid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_missing.json
--rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_valid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.526160 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/kafka/
--rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/kafka/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.527086 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/netbox/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/netbox/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.529189 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/
--rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/asn.json
--rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/ixlan.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.530154 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/phabricator/valid.conf
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.531094 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/redis_cluster/
--rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.533049 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/config_installer.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.534033 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/reposync/
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/reposync/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.534964 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/
--rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/service.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.639110 wikimedia-spicerack-7.0.0/spicerack/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__log.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5648 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18840 2023-05-04 08:02:07.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15575 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14445 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_init.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    22477 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.651438 wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/test_etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.661640 wikimedia-spicerack-7.0.0/spicerack/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/toolforge/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/toolforge/etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/typing.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.675764 wikimedia-spicerack-7.0.0/utils/
--rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/utils/check-style.sh
--rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/utils/format-code.sh
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.687783 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/entry_points.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.860638 wikimedia-spicerack-7.1.0/
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/.git-blame-ignore-revs
+-rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/.mailmap
+-rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)   105768 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-15 08:08:23.860933 wikimedia-spicerack-7.1.0/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.239626 wikimedia-spicerack-7.1.0/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.242171 wikimedia-spicerack-7.1.0/doc/examples/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/examples/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.270993 wikimedia-spicerack-7.1.0/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.272147 wikimedia-spicerack-7.1.0/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/_static/theme_overrides.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.373407 wikimedia-spicerack-7.1.0/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.administrative.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.alerting.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.alertmanager.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.apt.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.confctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.debmonitor.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.dhcp.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.dnsdisc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.elasticsearch_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.ganeti.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.icinga.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.ipmi.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.k8s.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.kafka.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mediawiki.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mysql.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mysql_legacy.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.netbox.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.peeringdb.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.puppet.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.redfish.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.redis_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.remote.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.reposync.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.service.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.toolforge.etcdctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.toolforge.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.typing.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/configuration.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/development.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/docutils.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     9572 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/pyproject.toml
+-rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-05-15 08:08:23.861830 wikimedia-spicerack-7.1.0/setup.cfg
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/setup.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.516429 wikimedia-spicerack-7.1.0/spicerack/
+-rw-r--r--   0 riccardo   (501) staff       (20)    27623 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-05-11 12:43:06.000000 wikimedia-spicerack-7.1.0/spicerack/_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/_log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/_menu.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/_module_api.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3949 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10644 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13883 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.1.0/spicerack/ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-05-15 07:26:54.000000 wikimedia-spicerack-7.1.0/spicerack/netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.1.0/spicerack/redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28496 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.520395 wikimedia-spicerack-7.1.0/spicerack/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.548266 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.551058 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/
+-rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/schema.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.552149 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config/valid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.182740 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.576471 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.615072 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.617489 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.620562 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.628337 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.665094 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.667574 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.669919 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.672013 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.673184 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/debmonitor/
+-rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/debmonitor/config.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.674479 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/discovery/
+-rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/discovery/authdns.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.678339 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/elasticsearch/
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/elasticsearch/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.190389 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.689467 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
+-rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.695569 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.699332 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/
+-rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.701750 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.707693 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/404.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/bogus.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/info.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/instance.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.738736 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/
+-rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_downtimed.json
+-rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_invalid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_missing.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_valid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.740094 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/kafka/
+-rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/kafka/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.741229 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/netbox/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/netbox/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.749287 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/
+-rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/asn.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/ixlan.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.754520 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/phabricator/valid.conf
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.759949 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/redis_cluster/
+-rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.767741 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/config_installer.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.768781 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/reposync/
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/reposync/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.772713 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/service.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.844514 wikimedia-spicerack-7.1.0/spicerack/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5648 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    19551 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15575 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14445 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_init.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-05-12 17:35:57.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23896 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.845851 wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/test_etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.849739 wikimedia-spicerack-7.1.0/spicerack/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/toolforge/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/toolforge/etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/typing.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.1.0/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.852698 wikimedia-spicerack-7.1.0/utils/
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/utils/check-style.sh
+-rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/utils/format-code.sh
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.859628 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-05-15 08:08:23.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/entry_points.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/top_level.txt
```

### Comparing `wikimedia-spicerack-7.0.0/.mailmap` & `wikimedia-spicerack-7.1.0/.mailmap`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/CHANGELOG.rst` & `wikimedia-spicerack-7.1.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Spicerack Changelog
 -------------------
 
+`v7.1.0`_ (2023-05-15)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+* dhcp: expand support for hostname based match using the manufacturer to adapt to different settings.
+* remote: improve usability of ``RemoteHosts.wait_reboot_since()`` clarifying the message and making it more DRY-RUN
+  friendly.
+
 `v7.0.0`_ (2023-05-08)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 API breaking changes
 """"""""""""""""""""
 
 * spicerack: refactor IRC logging:
@@ -2586,7 +2596,8 @@
 .. _`v6.2.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.2
 .. _`v6.3.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.3.0
 .. _`v6.4.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.0
 .. _`v6.4.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.1
 .. _`v6.4.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.2
 .. _`v6.4.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.3
 .. _`v7.0.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.0.0
+.. _`v7.1.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.1.0
```

### Comparing `wikimedia-spicerack-7.0.0/LICENSE` & `wikimedia-spicerack-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/PKG-INFO` & `wikimedia-spicerack-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 7.0.0
+Version: 7.1.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-7.0.0/doc/Makefile` & `wikimedia-spicerack-7.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/examples/config.yaml` & `wikimedia-spicerack-7.1.0/doc/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/api/index.rst` & `wikimedia-spicerack-7.1.0/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/conf.py` & `wikimedia-spicerack-7.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/configuration.rst` & `wikimedia-spicerack-7.1.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/development.rst` & `wikimedia-spicerack-7.1.0/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/installation.rst` & `wikimedia-spicerack-7.1.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/doc/source/introduction.rst` & `wikimedia-spicerack-7.1.0/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/prospector.yaml` & `wikimedia-spicerack-7.1.0/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/setup.cfg` & `wikimedia-spicerack-7.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/setup.py` & `wikimedia-spicerack-7.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/__init__.py` & `wikimedia-spicerack-7.1.0/spicerack/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/_cookbook.py` & `wikimedia-spicerack-7.1.0/spicerack/_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/_log.py` & `wikimedia-spicerack-7.1.0/spicerack/_log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/_menu.py` & `wikimedia-spicerack-7.1.0/spicerack/_menu.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/_module_api.py` & `wikimedia-spicerack-7.1.0/spicerack/_module_api.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/administrative.py` & `wikimedia-spicerack-7.1.0/spicerack/administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/alerting.py` & `wikimedia-spicerack-7.1.0/spicerack/alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/alertmanager.py` & `wikimedia-spicerack-7.1.0/spicerack/alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/apt.py` & `wikimedia-spicerack-7.1.0/spicerack/apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/confctl.py` & `wikimedia-spicerack-7.1.0/spicerack/confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/cookbook.py` & `wikimedia-spicerack-7.1.0/spicerack/cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/debmonitor.py` & `wikimedia-spicerack-7.1.0/spicerack/debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/decorators.py` & `wikimedia-spicerack-7.1.0/spicerack/decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/dhcp.py` & `wikimedia-spicerack-7.1.0/spicerack/dhcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,29 @@
 @dataclass(frozen=True)
 class DHCPConfMgmt(DHCPConfiguration):
     """A configuration for management network DHCP entries.
 
     Arguments:
         datacenter: the name of the Datacenter the host is.
         serial: the vendor serial of the host.
+        manufacturer: the name of the manufacturer.
         fqdn: the management console FQDN to use for this host.
         ipv4: the IP address to give the management interface.
 
     """
 
     datacenter: str
     serial: str
+    manufacturer: str
     fqdn: str
     ipv4: IPv4Address
 
     _template: str = """
     class "{s.fqdn}" {{
-        match if (lcase(option host-name) = "idrac-{s.lserial}");
+        match if (lcase(option host-name) = "{s.hostname}");
     }}
     pool {{
         allow members of "{s.fqdn}";
         range {s.ipv4} {s.ipv4};
     }}
     """
 
@@ -175,17 +177,21 @@
 
     @property
     def filename(self) -> str:
         """Return the filename that corresponds to this configuration."""
         return f"""mgmt-{self.datacenter}/{self.fqdn}.conf"""
 
     @property
-    def lserial(self) -> str:
-        """Return the serial as lowercase."""
-        return self.serial.lower()
+    def hostname(self) -> str:
+        """Return the hostname based on manufacturer and serial."""
+        serial = self.serial.lower()
+        if self.manufacturer.lower() == "dell":
+            return f"idrac-{serial}"
+
+        return serial
 
 
 class DHCP:
     """A class which provides tools for manipulating DHCP configuration snippets by data center."""
 
     def __init__(self, hosts: RemoteHosts, *, dry_run: bool = True):
         """Create a DHCP instance.
```

### Comparing `wikimedia-spicerack-7.0.0/spicerack/dnsdisc.py` & `wikimedia-spicerack-7.1.0/spicerack/dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/elasticsearch_cluster.py` & `wikimedia-spicerack-7.1.0/spicerack/elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/exceptions.py` & `wikimedia-spicerack-7.1.0/spicerack/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/ganeti.py` & `wikimedia-spicerack-7.1.0/spicerack/ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/icinga.py` & `wikimedia-spicerack-7.1.0/spicerack/icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/interactive.py` & `wikimedia-spicerack-7.1.0/spicerack/interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/ipmi.py` & `wikimedia-spicerack-7.1.0/spicerack/ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/k8s.py` & `wikimedia-spicerack-7.1.0/spicerack/k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/kafka.py` & `wikimedia-spicerack-7.1.0/spicerack/kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/mediawiki.py` & `wikimedia-spicerack-7.1.0/spicerack/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/mysql.py` & `wikimedia-spicerack-7.1.0/spicerack/mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/mysql_legacy.py` & `wikimedia-spicerack-7.1.0/spicerack/mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/netbox.py` & `wikimedia-spicerack-7.1.0/spicerack/netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/peeringdb.py` & `wikimedia-spicerack-7.1.0/spicerack/peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/puppet.py` & `wikimedia-spicerack-7.1.0/spicerack/puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/redfish.py` & `wikimedia-spicerack-7.1.0/spicerack/redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/redis_cluster.py` & `wikimedia-spicerack-7.1.0/spicerack/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/remote.py` & `wikimedia-spicerack-7.1.0/spicerack/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -540,29 +540,39 @@
 
         Arguments:
             since: the time after which the host should have booted.
             print_progress_bars: whether to print Cumin's progress bars to stderr.
 
         Raises:
             spicerack.remote.RemoteCheckError: if unable to connect to the host or the uptime is higher than expected.
+                When in DRY-RUN mode, it will raise only if unable to connect.
 
         """
         delta = (datetime.utcnow() - since).total_seconds()
         try:
             uptimes = self.uptime(print_progress_bars=print_progress_bars)
         except (RemoteExecutionError, RemoteError) as e:
-            raise RemoteCheckError(f"Unable to get uptime for {self._hosts}") from e
+            if self._dry_run:
+                raise RemoteCheckError(f"Reboot for {self._hosts} not found: unable to get uptime") from e
+            raise RemoteCheckError(
+                f"Reboot for {self._hosts} not found yet, keep polling for it: unable to get uptime"
+            ) from e
 
         for nodeset, uptime in uptimes:
             if uptime >= delta:
-                raise RemoteCheckError(
-                    f"Uptime for {nodeset} higher than threshold: {round(uptime, 2)} > {round(delta, 2)}"
-                )
+                msg = f"uptime {round(uptime, 2)} > threshold {round(delta, 2)}"
+                if self._dry_run:
+                    logger.info(
+                        "Reboot for %s not found - expected in dry run mode, host not rebooted: %s", nodeset, msg
+                    )
+                else:
+                    raise RemoteCheckError(f"Reboot for {nodeset} not found yet, keep polling for it: {msg}")
 
-        logger.info("Found reboot since %s for hosts %s", since, self._hosts)
+        if not self._dry_run:
+            logger.info("Found reboot since %s for hosts %s", since, self._hosts)
 
     def uptime(self, print_progress_bars: bool = True) -> list[tuple[NodeSet, float]]:
         """Get current uptime.
 
         Arguments:
             print_progress_bars: whether to print Cumin's progress bars to stderr.
```

### Comparing `wikimedia-spicerack-7.0.0/spicerack/reposync.py` & `wikimedia-spicerack-7.1.0/spicerack/reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/service.py` & `wikimedia-spicerack-7.1.0/spicerack/service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/__init__.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/schema.yaml` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/schema.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/info.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/info.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/instance.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/instance.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/asn.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/asn.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/ixlan.json` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/ixlan.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/service.yaml` & `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/service.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/sphinx_checker.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__cookbook.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__log.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_administrative.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alerting.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alertmanager.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_apt.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_confctl.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_debmonitor.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_decorators.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dhcp.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dhcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,33 +165,52 @@
             "    fixed-address 10.0.0.1;\n"
             '    option pxelinux.pathprefix "http://apt.wikimedia.org/tftpboot/bullseye-installer/";\n'
             "}\n"
         ),
         "ttyS1-115200/testhost0.conf",
     ),
     # dhcpconfmgmt tests
-    # - basic check of functionality
-    (
+    (  # Dell host
         dhcp.DHCPConfMgmt,
         {
             "datacenter": "eqiad",
             "serial": "TEST",
+            "manufacturer": "Dell",
             "fqdn": "test1001.mgmt.eqiad.wmnet",
             "ipv4": IPv4Address("10.0.0.1"),
         },
         (
             '\nclass "test1001.mgmt.eqiad.wmnet" {\n'
             '    match if (lcase(option host-name) = "idrac-test");\n'
             "}\npool {\n"
             '    allow members of "test1001.mgmt.eqiad.wmnet";\n'
             "    range 10.0.0.1 10.0.0.1;\n"
             "}\n"
         ),
         "mgmt-eqiad/test1001.mgmt.eqiad.wmnet.conf",
     ),
+    (  # Juniper device
+        dhcp.DHCPConfMgmt,
+        {
+            "datacenter": "eqiad",
+            "serial": "TESTSERIAL",
+            "manufacturer": "Juniper",
+            "fqdn": "test-switch1001.mgmt.eqiad.wmnet",
+            "ipv4": IPv4Address("10.0.0.1"),
+        },
+        (
+            '\nclass "test-switch1001.mgmt.eqiad.wmnet" {\n'
+            '    match if (lcase(option host-name) = "testserial");\n'
+            "}\npool {\n"
+            '    allow members of "test-switch1001.mgmt.eqiad.wmnet";\n'
+            "    range 10.0.0.1 10.0.0.1;\n"
+            "}\n"
+        ),
+        "mgmt-eqiad/test-switch1001.mgmt.eqiad.wmnet.conf",
+    ),
 )
 """`tuple[class, tuple[dict[str, str], str]]`: Parameters for test_configuration_generator."""
 
 
 @pytest.mark.parametrize("generator,kw_arguments,expected,expected_filename", configuration_generator_data)
 def test_configuration_generator(generator, kw_arguments, expected, expected_filename):
     """Test configuration generators producing expected outputs with various parameters."""
@@ -241,19 +260,19 @@
         dhcp.DHCPConfMac(hostname="testhost0", ipv4=IPv4Address("10.0.0.1"), mac=mac, ttys=1, distro="bullseye")
 
 
 def test_dhcp_mgmt_fail():
     """A DHCPConfMgmt object should fail to create if invalid parameters are passed to its init."""
     with pytest.raises(dhcp.DHCPError):
         # data center must be a value in ALL_DATACENTERS
-        dhcp.DHCPConfMgmt(datacenter="not-a-real-datacenter", serial="", fqdn="", ipv4=None)
+        dhcp.DHCPConfMgmt(datacenter="not-a-real-datacenter", serial="", manufacturer="", fqdn="", ipv4=None)
 
     with pytest.raises(dhcp.DHCPError):
         # hostname must be in the correct format
-        dhcp.DHCPConfMgmt(datacenter="eqiad", serial="", fqdn="not-a-real-hostname", ipv4=None)
+        dhcp.DHCPConfMgmt(datacenter="eqiad", serial="", manufacturer="", fqdn="not-a-real-hostname", ipv4=None)
 
 
 def test_create_dhcp_fail():
     """Test fail (hosts parameter has no hosts) DHCP instance creation."""
     hosts_mock = get_mock_hosts()
     hosts_mock.__len__.return_value = 0
     with pytest.raises(dhcp.DHCPError):
```

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dnsdisc.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_elasticsearch_cluster.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ganeti.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_icinga.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_init.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_interactive.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ipmi.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_k8s.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_kafka.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mediawiki.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql_legacy.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_netbox.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_peeringdb.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_puppet.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redfish.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redis_cluster.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_remote.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -377,15 +377,15 @@
     @mock.patch("spicerack.remote.RemoteHosts.uptime")
     def test_wait_reboot_since_uptime_fails(self, mocked_uptime, mocked_sleep, side_effect):
         """It should raise RemoteCheckError if unable to check the uptime on any host."""
         since = datetime.utcnow()
         mocked_uptime.side_effect = side_effect
         with pytest.raises(
             remote.RemoteCheckError,
-            match=r"Unable to get uptime for host\[1-9\]",
+            match=r"Reboot for host\[1-9\] not found yet, keep polling for it: unable to get uptime",
         ):
             self.remote_hosts.wait_reboot_since(since)
 
         # wait_reboot_since() sets tries to 240 and dry_run is False.
         assert mocked_uptime.call_count == 240
         assert mocked_sleep.called
 
@@ -393,21 +393,50 @@
     @mock.patch("spicerack.remote.RemoteHosts.uptime")
     def test_wait_reboot_since_uptime_too_big(self, mocked_uptime, mocked_sleep):
         """It should raise RemoteCheckError if any host doesn't have a small-enough uptime."""
         since = datetime.utcnow()
         mocked_uptime.return_value = [(nodeset("host[1-9]"), 30.0)]
         with pytest.raises(
             remote.RemoteCheckError,
-            match=r"Uptime for host\[1-9\] higher than threshold",
+            match=r"Reboot for host\[1-9\] not found yet, keep polling for it: uptime .* > threshold",
         ):
             self.remote_hosts.wait_reboot_since(since)
 
         mocked_uptime.assert_called_with(print_progress_bars=True)
         assert mocked_sleep.called
 
+    @pytest.mark.parametrize(
+        "side_effect",
+        (
+            remote.RemoteExecutionError(message="unable to connect", retcode=1, results=iter(())),
+            remote.RemoteError("Unable to extract data"),
+        ),
+    )
+    @mock.patch("spicerack.remote.RemoteHosts.uptime")
+    def test_wait_reboot_since_uptime_fails_dry_run(self, mocked_uptime, side_effect):
+        """It should raise RemoteCheckError if unable to check the uptime on any host."""
+        since = datetime.utcnow()
+        mocked_uptime.side_effect = side_effect
+        with pytest.raises(
+            remote.RemoteCheckError,
+            match=r"Reboot for host\[1-9\] not found: unable to get uptime",
+        ):
+            self.remote_hosts_dry_run.wait_reboot_since(since)
+
+        # tries reduced to 1 when dry_run is True.
+        mocked_uptime.assert_called_once_with(print_progress_bars=True)
+
+    @mock.patch("spicerack.remote.RemoteHosts.uptime")
+    def test_wait_reboot_since_uptime_too_big_dry_run(self, mocked_uptime):
+        """It should succeed in dry-run mode, even when the uptime is too high."""
+        since = datetime.utcnow()
+        mocked_uptime.return_value = [(nodeset("host[1-9]"), 30.0)]
+        self.remote_hosts_dry_run.wait_reboot_since(since)
+        mocked_uptime.assert_called_once_with(print_progress_bars=True)
+
     def test_uptime_ok(self):
         """It should gather the current uptime from the target hosts."""
         nodes_a = "host1"
         nodes_b = "host[2-9]"
         mock_cumin(
             self.mocked_transports,
             0,
```

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_reposync.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_service.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/test_etcdctl.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/test_etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/tests/vulture_whitelist.py` & `wikimedia-spicerack-7.1.0/spicerack/tests/vulture_whitelist.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/spicerack/toolforge/etcdctl.py` & `wikimedia-spicerack-7.1.0/spicerack/toolforge/etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/tox.ini` & `wikimedia-spicerack-7.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/utils/check-style.sh` & `wikimedia-spicerack-7.1.0/utils/check-style.sh`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/PKG-INFO` & `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 7.0.0
+Version: 7.1.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/SOURCES.txt` & `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/requires.txt` & `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/requires.txt`

 * *Files identical despite different names*

