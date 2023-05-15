# Comparing `tmp/enos-8.0.0a3.tar.gz` & `tmp/enos-8.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enos-8.0.0a3.tar", max compression
+gzip compressed data, was "enos-8.0.0a4.tar", max compression
```

## Comparing `enos-8.0.0a3.tar` & `enos-8.0.0a4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    35148 2022-10-20 13:50:57.843485 enos-8.0.0a3/LICENSE
--rw-r--r--   0        0        0     3270 2023-04-25 13:33:13.806401 enos-8.0.0a3/README.rst
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/__init__.py
--rw-r--r--   0        0        0      529 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/enos.yml
--rw-r--r--   0        0        0      372 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/group_vars/all.yml
--rw-r--r--   0        0        0      378 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/init_os.yml
--rw-r--r--   0        0        0     4979 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/plugins/callback/influxdb_events.py
--rw-r--r--   0        0        0       44 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/defaults/main.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/bench.yml
--rw-r--r--   0        0        0     1417 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/deploy.yml
--rw-r--r--   0        0        0      311 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/main.yml
--rw-r--r--   0        0        0      116 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/pull.yml
--rw-r--r--   0        0        0      280 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/defaults/main.yml
--rw-r--r--   0        0        0    23358 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/files/collectd.conf
--rw-r--r--   0        0        0       25 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/contextswitch.conf
--rw-r--r--   0        0        0      359 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/haproxy.conf
--rw-r--r--   0        0        0     9676 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/files/haproxy.py
--rw-r--r--   0        0        0      156 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/protocols.conf
--rw-r--r--   0        0        0      119 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-compute.conf
--rw-r--r--   0        0        0      353 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
--rw-r--r--   0        0        0      249 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
--rw-r--r--   0        0        0       69 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
--rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
--rw-r--r--   0        0        0      211 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-network.conf
--rw-r--r--   0        0        0      216 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-nova.conf
--rw-r--r--   0        0        0      128 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/bench.yml
--rw-r--r--   0        0        0     1881 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/deploy.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/main.yml
--rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/tasks/pull.yml
--rw-r--r--   0        0        0      114 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/templates/influx.conf.j2
--rw-r--r--   0        0        0      386 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/templates/memcached.conf.j2
--rw-r--r--   0        0        0      455 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/templates/mysql.conf.j2
--rw-r--r--   0        0        0     1081 2022-11-07 08:45:07.825216 enos-8.0.0a3/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       42 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/defaults/main.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/bench.yml
--rw-r--r--   0        0        0     1646 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/deploy.yml
--rw-r--r--   0        0        0      120 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/main.yml
--rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/grafana/tasks/pull.yml
--rw-r--r--   0        0        0       36 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/defaults/main.yml
--rw-r--r--   0        0        0    10241 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/files/config.toml
--rw-r--r--   0        0        0     9721 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/files/types.db
--rw-r--r--   0        0        0      357 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/bench.yml
--rw-r--r--   0        0        0     1582 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/deploy.yml
--rw-r--r--   0        0        0      207 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/main.yml
--rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/influx/tasks/pull.yml
--rw-r--r--   0        0        0     1112 2023-04-25 13:33:13.806401 enos-8.0.0a3/enos/ansible/roles/init_os/tasks/deploy.yml
--rw-r--r--   0        0        0       40 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/init_os/tasks/main.yml
--rw-r--r--   0        0        0      493 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/ansible/roles/init_os/tasks/pull.yml
--rw-r--r--   0        0        0     3434 2023-04-25 13:33:13.806401 enos-8.0.0a3/enos/ansible/roles/init_os/templates/init.sh.j2
--rwxr-xr-x   0        0        0    25920 2023-05-09 14:37:44.792871 enos-8.0.0a3/enos/cli.py
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/__init__.py
--rw-r--r--   0        0        0     1815 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/chameleonbaremetal.py
--rw-r--r--   0        0        0     1293 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/chameleonkvm.py
--rw-r--r--   0        0        0     2417 2023-04-25 13:33:13.806401 enos-8.0.0a3/enos/provider/enos_vagrant.py
--rw-r--r--   0        0        0     5813 2023-04-25 13:33:13.806401 enos-8.0.0a3/enos/provider/g5k.py
--rw-r--r--   0        0        0      818 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/host.py
--rw-r--r--   0        0        0     2963 2023-04-25 13:33:13.806401 enos-8.0.0a3/enos/provider/openstack.py
--rw-r--r--   0        0        0     1636 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/provider.py
--rw-r--r--   0        0        0     2786 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/provider/static.py
--rw-r--r--   0        0        0     2757 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/provider/vmong5k.py
--rw-r--r--   0        0        0     9471 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/resources/inventory.sample
--rw-r--r--   0        0        0     9666 2022-11-08 12:27:03.004104 enos-8.0.0a3/enos/resources/multinode
--rw-r--r--   0        0        0    21559 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/resources/passwords.yml
--rw-r--r--   0        0        0      513 2022-11-07 08:45:34.949389 enos-8.0.0a3/enos/resources/workload/create-and-update-image.yaml
--rw-r--r--   0        0        0     1069 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/resources/workload/nova-boot-list-cc.yml
--rw-r--r--   0        0        0      715 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/resources/workload/run.yml
--rw-r--r--   0        0        0      189 2022-11-07 08:45:07.829217 enos-8.0.0a3/enos/services/__init__.py
--rw-r--r--   0        0        0    14973 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/services/kolla.py
--rw-r--r--   0        0        0     8376 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/services/rally.py
--rw-r--r--   0        0        0     3720 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/services/shaker.py
--rwxr-xr-x   0        0        0    11791 2022-11-07 10:41:09.316608 enos-8.0.0a3/enos/tasks/__init__.py
--rw-r--r--   0        0        0     5701 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/tasks/new.py
--rw-r--r--   0        0        0    12116 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/tasks/up.py
--rw-r--r--   0        0        0      911 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/templates/Vagrantfile.j2
--rw-r--r--   0        0        0    10240 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/templates/grafana_dashboard.json
--rw-r--r--   0        0        0     2049 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/templates/reservation.yaml.j2
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/utils/__init__.py
--rw-r--r--   0        0        0     3229 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/utils/build.py
--rw-r--r--   0        0        0     3285 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/utils/cli.py
--rw-r--r--   0        0        0     1932 2023-05-09 15:17:28.775653 enos-8.0.0a3/enos/utils/constants.py
--rw-r--r--   0        0        0     1009 2022-11-07 08:45:07.833218 enos-8.0.0a3/enos/utils/errors.py
--rw-r--r--   0        0        0     6257 2023-04-25 13:33:13.810401 enos-8.0.0a3/enos/utils/extra.py
--rw-r--r--   0        0        0     1907 2023-05-09 15:17:25.815786 enos-8.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 enos-8.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-10-20 13:50:57.843485 enos-8.0.0a4/LICENSE
+-rw-r--r--   0        0        0     3270 2023-04-25 13:33:13.806401 enos-8.0.0a4/README.rst
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/__init__.py
+-rw-r--r--   0        0        0      529 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/enos.yml
+-rw-r--r--   0        0        0      372 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/group_vars/all.yml
+-rw-r--r--   0        0        0      378 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/init_os.yml
+-rw-r--r--   0        0        0     4979 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/plugins/callback/influxdb_events.py
+-rw-r--r--   0        0        0       44 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/bench.yml
+-rw-r--r--   0        0        0     1417 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/deploy.yml
+-rw-r--r--   0        0        0      311 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/main.yml
+-rw-r--r--   0        0        0      116 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/pull.yml
+-rw-r--r--   0        0        0      280 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/defaults/main.yml
+-rw-r--r--   0        0        0    23358 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/collectd.conf
+-rw-r--r--   0        0        0       25 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/contextswitch.conf
+-rw-r--r--   0        0        0      359 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.conf
+-rw-r--r--   0        0        0     9676 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.py
+-rw-r--r--   0        0        0      156 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/protocols.conf
+-rw-r--r--   0        0        0      119 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-compute.conf
+-rw-r--r--   0        0        0      353 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
+-rw-r--r--   0        0        0      249 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
+-rw-r--r--   0        0        0       69 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
+-rw-r--r--   0        0        0      211 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-network.conf
+-rw-r--r--   0        0        0      216 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-nova.conf
+-rw-r--r--   0        0        0      128 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/bench.yml
+-rw-r--r--   0        0        0     1881 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/deploy.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/main.yml
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/pull.yml
+-rw-r--r--   0        0        0      114 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/influx.conf.j2
+-rw-r--r--   0        0        0      386 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/memcached.conf.j2
+-rw-r--r--   0        0        0      455 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/mysql.conf.j2
+-rw-r--r--   0        0        0     1081 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0       42 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/bench.yml
+-rw-r--r--   0        0        0     1646 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/deploy.yml
+-rw-r--r--   0        0        0      120 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/pull.yml
+-rw-r--r--   0        0        0       36 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/defaults/main.yml
+-rw-r--r--   0        0        0    10241 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/files/config.toml
+-rw-r--r--   0        0        0     9721 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/files/types.db
+-rw-r--r--   0        0        0      357 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/bench.yml
+-rw-r--r--   0        0        0     1582 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/deploy.yml
+-rw-r--r--   0        0        0      207 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/pull.yml
+-rw-r--r--   0        0        0     1112 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/deploy.yml
+-rw-r--r--   0        0        0       40 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/main.yml
+-rw-r--r--   0        0        0      493 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/pull.yml
+-rw-r--r--   0        0        0     3391 2023-05-15 13:45:52.493838 enos-8.0.0a4/enos/ansible/roles/init_os/templates/init.sh.j2
+-rwxr-xr-x   0        0        0    25920 2023-05-09 14:37:44.792871 enos-8.0.0a4/enos/cli.py
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/__init__.py
+-rw-r--r--   0        0        0     1815 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/chameleonbaremetal.py
+-rw-r--r--   0        0        0     1293 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/chameleonkvm.py
+-rw-r--r--   0        0        0     2417 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/enos_vagrant.py
+-rw-r--r--   0        0        0     5813 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/g5k.py
+-rw-r--r--   0        0        0      818 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/host.py
+-rw-r--r--   0        0        0     2963 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/openstack.py
+-rw-r--r--   0        0        0     1636 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/provider.py
+-rw-r--r--   0        0        0     2786 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/provider/static.py
+-rw-r--r--   0        0        0     2757 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/vmong5k.py
+-rw-r--r--   0        0        0     9471 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/resources/inventory.sample
+-rw-r--r--   0        0        0     9666 2022-11-08 12:27:03.004104 enos-8.0.0a4/enos/resources/multinode
+-rw-r--r--   0        0        0    21559 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/resources/passwords.yml
+-rw-r--r--   0        0        0      513 2022-11-07 08:45:34.949389 enos-8.0.0a4/enos/resources/workload/create-and-update-image.yaml
+-rw-r--r--   0        0        0     1069 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/resources/workload/nova-boot-list-cc.yml
+-rw-r--r--   0        0        0      715 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/resources/workload/run.yml
+-rw-r--r--   0        0        0      189 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/services/__init__.py
+-rw-r--r--   0        0        0    15121 2023-05-15 13:29:39.549786 enos-8.0.0a4/enos/services/kolla.py
+-rw-r--r--   0        0        0     8376 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/services/rally.py
+-rw-r--r--   0        0        0     3720 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/services/shaker.py
+-rwxr-xr-x   0        0        0    11791 2022-11-07 10:41:09.316608 enos-8.0.0a4/enos/tasks/__init__.py
+-rw-r--r--   0        0        0     5701 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/tasks/new.py
+-rw-r--r--   0        0        0    12229 2023-05-15 13:29:39.549786 enos-8.0.0a4/enos/tasks/up.py
+-rw-r--r--   0        0        0      911 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/templates/Vagrantfile.j2
+-rw-r--r--   0        0        0    10240 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/templates/grafana_dashboard.json
+-rw-r--r--   0        0        0     2049 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/templates/reservation.yaml.j2
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/__init__.py
+-rw-r--r--   0        0        0     3229 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/utils/build.py
+-rw-r--r--   0        0        0     3285 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/cli.py
+-rw-r--r--   0        0        0     1932 2023-05-15 13:59:51.434142 enos-8.0.0a4/enos/utils/constants.py
+-rw-r--r--   0        0        0     1009 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/errors.py
+-rw-r--r--   0        0        0     6257 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/utils/extra.py
+-rw-r--r--   0        0        0     1907 2023-05-15 14:00:01.978094 enos-8.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 enos-8.0.0a4/PKG-INFO
```

### Comparing `enos-8.0.0a3/LICENSE` & `enos-8.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/README.rst` & `enos-8.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/enos.yml` & `enos-8.0.0a4/enos/ansible/enos.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/plugins/callback/influxdb_events.py` & `enos-8.0.0a4/enos/ansible/plugins/callback/influxdb_events.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/cadvisor/tasks/deploy.yml` & `enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/collectd/files/collectd.conf` & `enos-8.0.0a4/enos/ansible/roles/collectd/files/collectd.conf`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/collectd/files/haproxy.py` & `enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/collectd/tasks/deploy.yml` & `enos-8.0.0a4/enos/ansible/roles/collectd/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2` & `enos-8.0.0a4/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/grafana/tasks/deploy.yml` & `enos-8.0.0a4/enos/ansible/roles/grafana/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/influx/files/config.toml` & `enos-8.0.0a4/enos/ansible/roles/influx/files/config.toml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/influx/files/types.db` & `enos-8.0.0a4/enos/ansible/roles/influx/files/types.db`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/influx/tasks/deploy.yml` & `enos-8.0.0a4/enos/ansible/roles/influx/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/init_os/tasks/deploy.yml` & `enos-8.0.0a4/enos/ansible/roles/init_os/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/ansible/roles/init_os/templates/init.sh.j2` & `enos-8.0.0a4/enos/ansible/roles/init_os/templates/init.sh.j2`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env bash
 
 set -x
+set -e
 
 DNS_NAMESERVER={{ provider_net.dns|default("9.9.9.9", true) }}
 SUBNET_RANGE={{ provider_net.network }}
 GATEWAY={{ provider_net.gateway }}
 
 ## Images
 openstack image show debian-10 || openstack image create --disk-format=qcow2 --container-format=bare --property architecture=x86_64 --public --file /srv/init_os/debian-10.qcow2 debian-10
 openstack image show cirros.uec || openstack image create --disk-format=qcow2 --container-format=bare --property architecture=x86_64 --public --file /srv/init_os/cirros.uec.qcow2 cirros.uec
 
 
 ## Flavors
-openstack flavor show m1.tiny || openstack flavor create m1.tiny --id auto --ram 512 --disk 1 --vcpus 1 --public
-openstack flavor show m1.small || openstack flavor create m1.small --id auto --ram 2014 --disk 20 --vcpus 1 --public
-openstack flavor show m1.medium || openstack flavor create m1.medium --id auto --ram 4096 --disk 40 --vcpus 2 --public
-openstack flavor show m1.large || openstack flavor create m1.large --id auto --ram 8192 --disk 80 --vcpus 4 --public
-openstack flavor show m1.xlarge || openstack flavor create m1.xlarge --id auto --ram 16384 --disk 160 --vcpus 8 --public
+openstack flavor show m1.tiny || openstack flavor create m1.tiny --ram 512 --disk 1 --vcpus 1 --public
+openstack flavor show m1.small || openstack flavor create m1.small --ram 2014 --disk 20 --vcpus 1 --public
+openstack flavor show m1.medium || openstack flavor create m1.medium --ram 4096 --disk 40 --vcpus 2 --public
+openstack flavor show m1.large || openstack flavor create m1.large --ram 8192 --disk 80 --vcpus 4 --public
+openstack flavor show m1.xlarge || openstack flavor create m1.xlarge --ram 16384 --disk 160 --vcpus 8 --public
 
 
 ## Networks
 ## private
 openstack network show private || openstack network create private --provider-network-type vxlan
 
 ### private-subnet
```

### Comparing `enos-8.0.0a3/enos/cli.py` & `enos-8.0.0a4/enos/cli.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/chameleonbaremetal.py` & `enos-8.0.0a4/enos/provider/chameleonbaremetal.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/chameleonkvm.py` & `enos-8.0.0a4/enos/provider/chameleonkvm.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/enos_vagrant.py` & `enos-8.0.0a4/enos/provider/enos_vagrant.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/g5k.py` & `enos-8.0.0a4/enos/provider/g5k.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/host.py` & `enos-8.0.0a4/enos/provider/host.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/openstack.py` & `enos-8.0.0a4/enos/provider/openstack.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/provider.py` & `enos-8.0.0a4/enos/provider/provider.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/static.py` & `enos-8.0.0a4/enos/provider/static.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/provider/vmong5k.py` & `enos-8.0.0a4/enos/provider/vmong5k.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/inventory.sample` & `enos-8.0.0a4/enos/resources/inventory.sample`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/multinode` & `enos-8.0.0a4/enos/resources/multinode`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/passwords.yml` & `enos-8.0.0a4/enos/resources/passwords.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/workload/create-and-update-image.yaml` & `enos-8.0.0a4/enos/resources/workload/create-and-update-image.yaml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/workload/nova-boot-list-cc.yml` & `enos-8.0.0a4/enos/resources/workload/nova-boot-list-cc.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/resources/workload/run.yml` & `enos-8.0.0a4/enos/resources/workload/run.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/services/kolla.py` & `enos-8.0.0a4/enos/services/kolla.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,15 +342,17 @@
         with elib.play_on(roles={}, pattern_hosts="localhost") as yaml:
             yaml.local_action(
                 **title(f'Install {pip_package} in {venv}'),
                 module="pip",
                 # Pin Jinja2 version to fix the renaming of `contextfilter`
                 # into `pass_context.evalcontextfilter`.
                 # See https://github.com/BeyondTheClouds/enos/pull/346#issuecomment-1080851796  # noqa
-                name=[ANSIBLE_PKG, 'influxdb', 'Jinja2==3.0.3', pip_package],
+                # requests/urllib3 bug: https://github.com/docker/docker-py/issues/3113  # noqa
+                name=[ANSIBLE_PKG, 'Jinja2==3.0.3', 'requests<2.29', 'urllib3<2',
+                      'influxdb', pip_package],
                 virtualenv=str(venv),
                 virtualenv_python=PY_VERSION)
 
         return venv
 
 
 def title(title: str) -> Dict[str, str]:
```

### Comparing `enos-8.0.0a3/enos/services/rally.py` & `enos-8.0.0a4/enos/services/rally.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/services/shaker.py` & `enos-8.0.0a4/enos/services/shaker.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/tasks/__init__.py` & `enos-8.0.0a4/enos/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/tasks/new.py` & `enos-8.0.0a4/enos/tasks/new.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/tasks/up.py` & `enos-8.0.0a4/enos/tasks/up.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,17 +201,18 @@
 
         # sudo required by `kolla-ansible destroy`.  See
         # https://github.com/openstack/kolla-ansible/blob/stable/ussuri/tools/validate-docker-execute.sh#L7
         yml.apt(
             **title('Install the bare necessities (apt)'),
             name=['sudo', 'git', 'qemu-kvm'],
             update_cache=True)
+        # requests/urllib3 bug: https://github.com/docker/docker-py/issues/3113
         yml.pip(
             **title('Install the bare necessities (pip)'),
-            name=['docker', 'influxdb'],
+            name=['docker', 'requests==2.28.2', 'urllib3<2', 'influxdb'],
             executable='pip3')
 
         # nscd prevents kolla-toolbox to start. See,
         # https://bugs.launchpad.net/kolla-ansible/+bug/1680139
         yml.systemd(
             **title('Stop nscd to prevent kolla-toolbox error'),
             name='nscd', state='stopped', ignore_errors=True)
```

### Comparing `enos-8.0.0a3/enos/templates/Vagrantfile.j2` & `enos-8.0.0a4/enos/templates/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/templates/grafana_dashboard.json` & `enos-8.0.0a4/enos/templates/grafana_dashboard.json`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/templates/reservation.yaml.j2` & `enos-8.0.0a4/enos/templates/reservation.yaml.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/utils/build.py` & `enos-8.0.0a4/enos/utils/build.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/utils/cli.py` & `enos-8.0.0a4/enos/utils/cli.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/utils/constants.py` & `enos-8.0.0a4/enos/utils/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 # fake interface a give it the neutron_external_interface role
 NEUTRON_EXTERNAL_INTERFACE = 'neutron_external_interface'
 
 # In case we need to create a fake interface, this will be the nic name.
 FAKE_NEUTRON_EXTERNAL_INTERFACE = 'nei'
 
 # ENOS Setup
-VERSION = '8.0.0a3'
+VERSION = '8.0.0a4'
```

### Comparing `enos-8.0.0a3/enos/utils/errors.py` & `enos-8.0.0a4/enos/utils/errors.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/enos/utils/extra.py` & `enos-8.0.0a4/enos/utils/extra.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a3/pyproject.toml` & `enos-8.0.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enos"
-version = "8.0.0a3"
+version = "8.0.0a4"
 description = "Experimental eNvironment for OpenStack"
 authors = ["Didier Iscovery <discovery-dev@inria.fr>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/BeyondTheClouds/enos"
 documentation = "https://beyondtheclouds.github.io/enos/"
 keywords = ["OpenStack", "Evaluation", "Grid'5000", "Chameleon", "Vagrant"]
```

### Comparing `enos-8.0.0a3/PKG-INFO` & `enos-8.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enos
-Version: 8.0.0a3
+Version: 8.0.0a4
 Summary: Experimental eNvironment for OpenStack
 Home-page: https://github.com/BeyondTheClouds/enos
 License: GPL-3.0-or-later
 Keywords: OpenStack,Evaluation,Grid'5000,Chameleon,Vagrant
 Author: Didier Iscovery
 Author-email: discovery-dev@inria.fr
 Requires-Python: >=3.8,<4.0
```

