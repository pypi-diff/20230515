# Comparing `tmp/gardener-cicd-libs-1.2054.0.tar.gz` & `tmp/gardener-cicd-libs-1.2055.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2054.0.tar", last modified: Fri May 12 07:20:27 2023, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2055.0.tar", last modified: Mon May 15 06:33:41 2023, max compression
```

## Comparing `gardener-cicd-libs-1.2054.0.tar` & `gardener-cicd-libs-1.2055.0.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.584491 gardener-cicd-libs-1.2054.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-12 07:20:27.584491 gardener-cicd-libs-1.2054.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.552491 gardener-cicd-libs-1.2054.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10735 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/jira.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.552491 gardener-cicd-libs-1.2054.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)     9811 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    16096 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)     9233 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.556491 gardener-cicd-libs-1.2054.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/replicate.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)    19528 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.556491 gardener-cicd-libs-1.2054.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.556491 gardener-cicd-libs-1.2054.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14969 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.556491 gardener-cicd-libs-1.2054.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    17522 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.560491 gardener-cicd-libs-1.2054.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     2587 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5217 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    19200 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    17352 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)     9849 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27053 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.560491 gardener-cicd-libs-1.2054.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-12 07:20:21.000000 gardener-cicd-libs-1.2054.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4192 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      639 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/alter_container_images.py
--rw-r--r--   0 root         (0) root         (0)     9157 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    11982 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     3439 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8822 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     5271 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     3660 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)     4201 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    37168 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     4902 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     7028 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/scan_container_images.mako
--rw-r--r--   0 root         (0) root         (0)     8649 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    19259 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1165 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23433 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5362 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/container/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16315 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      735 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/cosign.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/platform.py
--rwxr-xr-x   0 root         (0) root         (0)    26860 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/rbsc_bom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.568491 gardener-cicd-libs-1.2054.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9639 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     5163 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-12 07:20:27.000000 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6208 2023-05-12 07:20:27.000000 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 07:20:27.000000 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      925 2023-05-12 07:20:27.000000 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      233 2023-05-12 07:20:27.000000 gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/github/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11313 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)     9092 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    34570 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/compliance/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.572491 gardener-cicd-libs-1.2054.0/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/release_notes/renderer.py
--rw-r--r--   0 root         (0) root         (0)    19222 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/release_notes/util.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    33961 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    15039 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6926 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/kube/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/kube/ctx.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/kube/helm.py
--rw-r--r--   0 root         (0) root         (0)    26693 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/kube/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/mail/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/makoutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/product/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/product/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/product/util.py
--rw-r--r--   0 root         (0) root         (0)    22448 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/product/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11164 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     4577 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/release_notes/markdown.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     7272 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/reutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/saf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/saf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/saf/client.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/saf/model.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-12 07:20:27.584491 gardener-cicd-libs-1.2054.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.576491 gardener-cicd-libs-1.2054.0/test/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/container/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/github/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6142 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/github_util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.580491 gardener-cicd-libs-1.2054.0/test/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/release_notes/default_util.py
--rw-r--r--   0 root         (0) root         (0)    18172 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/release_notes/renderer_test.py
--rw-r--r--   0 root         (0) root         (0)    21822 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/github/release_notes/util_test.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/kubeutil_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.584491 gardener-cicd-libs-1.2054.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 07:20:27.584491 gardener-cicd-libs-1.2054.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    15220 2023-05-12 07:19:09.000000 gardener-cicd-libs-1.2054.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.940026 gardener-cicd-libs-1.2055.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10735 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/jira.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.944026 gardener-cicd-libs-1.2055.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    16096 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     9233 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.944026 gardener-cicd-libs-1.2055.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/replicate.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)    19528 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.948026 gardener-cicd-libs-1.2055.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.948026 gardener-cicd-libs-1.2055.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14969 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.948026 gardener-cicd-libs-1.2055.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.952026 gardener-cicd-libs-1.2055.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    19200 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    17352 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)    10994 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27053 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.952026 gardener-cicd-libs-1.2055.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-15 06:33:36.000000 gardener-cicd-libs-1.2055.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      639 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.956026 gardener-cicd-libs-1.2055.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/alter_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    11982 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3439 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8822 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    37168 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/scan_container_images.mako
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    20482 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.956026 gardener-cicd-libs-1.2055.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23433 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.956026 gardener-cicd-libs-1.2055.0/container/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16315 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/cosign.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/platform.py
+-rwxr-xr-x   0 root         (0) root         (0)    26860 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/rbsc_bom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9639 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.960026 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-15 06:33:41.000000 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6208 2023-05-15 06:33:41.000000 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 06:33:41.000000 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      925 2023-05-15 06:33:41.000000 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2023-05-15 06:33:41.000000 gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/github/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11313 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)     9092 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    34570 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/compliance/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/release_notes/renderer.py
+-rw-r--r--   0 root         (0) root         (0)    19222 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/release_notes/util.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    33961 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    15039 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/kube/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/kube/ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/kube/helm.py
+-rw-r--r--   0 root         (0) root         (0)    26693 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/kube/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/makoutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.964026 gardener-cicd-libs-1.2055.0/product/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/product/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/product/util.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/product/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11275 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     7272 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/reutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/saf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/saf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/saf/client.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/saf/model.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7482 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.968026 gardener-cicd-libs-1.2055.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6142 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/github_util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/test/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/release_notes/default_util.py
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/release_notes/renderer_test.py
+-rw-r--r--   0 root         (0) root         (0)    21822 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/github/release_notes/util_test.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/kubeutil_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 06:33:41.972026 gardener-cicd-libs-1.2055.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-05-15 06:29:14.000000 gardener-cicd-libs-1.2055.0/version.py
```

### Comparing `gardener-cicd-libs-1.2054.0/LICENSE.md` & `gardener-cicd-libs-1.2055.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/README.md` & `gardener-cicd-libs-1.2055.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/__init__.py` & `gardener-cicd-libs-1.2055.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2055.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/aws.py` & `gardener-cicd-libs-1.2055.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/clamav.py` & `gardener-cicd-libs-1.2055.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/concourse.py` & `gardener-cicd-libs-1.2055.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/delivery.py` & `gardener-cicd-libs-1.2055.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2055.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/gcp.py` & `gardener-cicd-libs-1.2055.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/github.py` & `gardener-cicd-libs-1.2055.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2055.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/jira.py` & `gardener-cicd-libs-1.2055.0/ccc/jira.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/oci.py` & `gardener-cicd-libs-1.2055.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/protecode.py` & `gardener-cicd-libs-1.2055.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2055.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2055.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cli.py` & `gardener-cicd-libs-1.2055.0/cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/access.py` & `gardener-cicd-libs-1.2055.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/iter.py` & `gardener-cicd-libs-1.2055.0/cnudie/iter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/purge.py` & `gardener-cicd-libs-1.2055.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/replicate.py` & `gardener-cicd-libs-1.2055.0/cnudie/replicate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2055.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/util.py` & `gardener-cicd-libs-1.2055.0/cnudie/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cnudie/validate.py` & `gardener-cicd-libs-1.2055.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/client/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/client/api.py` & `gardener-cicd-libs-1.2055.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/client/model.py` & `gardener-cicd-libs-1.2055.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2055.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/client/util.py` & `gardener-cicd-libs-1.2055.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2055.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/factory.py` & `gardener-cicd-libs-1.2055.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/base.py` & `gardener-cicd-libs-1.2055.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/job.py` & `gardener-cicd-libs-1.2055.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2055.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2055.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/step.py` & `gardener-cicd-libs-1.2055.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/draft_release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/update_component_deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from concourse.model.step import (
     PipelineStep,
     PrivilegeMode,
     PullRequestNotificationPolicy,
 )
 from concourse.model.base import (
     AttributeSpec,
+    EnumValueWithDocumentation,
+    EnumWithDocumentation,
     ModelBase,
     ScriptType,
     Trait,
     TraitTransformer,
 )
 from concourse.model.job import (
     JobVariant,
@@ -51,14 +53,35 @@
 
 
 class UpstreamUpdatePolicy(enum.Enum):
     STRICTLY_FOLLOW = 'strictly_follow'
     ACCEPT_HOTFIXES = 'accept_hotfixes'
 
 
+class ReleaseNotesHandling(EnumWithDocumentation):
+    DEFAULT = EnumValueWithDocumentation(
+        value='default',
+        doc='''
+        Use default version of release note creation code. Use this if you are interested in
+        stability rather than the latest features.
+        ''',
+    )
+    PREVIEW = EnumValueWithDocumentation(
+        value='preview',
+        doc='''
+            Use preview version of release note creation code. Use this to join new features and
+            feature-rollouts.
+
+            .. note::
+                if no features are being tested/rolled-out, using this value is the same as using
+                `default`.
+        '''
+    )
+
+
 MERGE_POLICY_CONFIG_ATTRIBUTES = (
     AttributeSpec.optional(
         name='component_names',
         default=[],
         type=typing.List[str],
         doc=(
             'a sequence of regular expressions. This merge policy will be applied to matching '
@@ -160,15 +183,23 @@
         type=bool,
     ),
     AttributeSpec.optional(
         name='vars',
         default={},
         doc='env vars to pass to after_merge_callback (similar to step\'s vars)',
         type=dict,
-    )
+    ),
+    AttributeSpec.optional(
+        name='release_notes_handling',
+        default=ReleaseNotesHandling.DEFAULT.value,
+        doc='''
+        configures which iteration of the code to use when generating release notes.
+        ''',
+        type=ReleaseNotesHandling,
+    ),
 )
 
 
 class UpdateComponentDependenciesTrait(Trait):
     @classmethod
     def _attribute_specs(cls):
         return ATTRIBUTES
@@ -219,14 +250,17 @@
 
     def after_merge_callback(self):
         return self.raw.get('after_merge_callback')
 
     def ignore_prerelease_versions(self):
         return self.raw.get('ignore_prerelease_versions')
 
+    def release_notes_handling(self) -> ReleaseNotesHandling:
+        return ReleaseNotesHandling(self.raw['release_notes_handling'])
+
     def vars(self):
         return self.raw['vars']
 
     def transformer(self):
         return UpdateComponentDependenciesTraitTransformer(trait=self)
 
     def validate(self):
```

### Comparing `gardener-cicd-libs-1.2054.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2055.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/replicator.py` & `gardener-cicd-libs-1.2055.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2055.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2055.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2055.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2055.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2055.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/alter_container_images.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/alter_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-import typing
 
 import git
 import yaml
 
 import ci.util
 import cnudie.util
 import cnudie.retrieve
@@ -37,15 +36,15 @@
         data=dataclasses.asdict(component_descriptor_v2),
         Dumper=cm.EnumValueYamlDumper,
     )
 
 
 def base_component_descriptor_v2(
     component_name_v2: str,
-    component_labels: typing.Iterable[cm.Label],
+    component_labels: list[cm.Label],
     effective_version: str,
     source_labels: tuple,
     ctx_repository_base_url: str,
     commit: str,
 ):
     import datetime
     import cnudie.migrate
@@ -68,20 +67,27 @@
     if cnudie.migrate.emit_compatible_to_cnudie_v2:
         provider = 'internal'
     else:
         provider = {
             'name': 'SAP SE',
         }
 
+    component_labels = list(component_labels)
+    component_labels.append(
+        cm.Label(
+            name='cloud.gardener/ocm/creation-date',
+            value=datetime.datetime.now(tz=datetime.timezone.utc).isoformat(),
+        ),
+    )
+
     base_descriptor_v2 = cm.ComponentDescriptor(
       meta=cm.Metadata(schemaVersion=cm.SchemaVersion.V2),
       component=cm.Component(
         name=component_name_v2,
         version=effective_version,
-        creationTime=datetime.datetime.now(tz=datetime.timezone.utc).isoformat(),
         repositoryContexts=[
           cm.OciRepositoryContext(
             baseUrl=ctx_repository_base_url,
             type=cm.AccessType.OCI_REGISTRY,
           )
         ],
         provider=provider,
@@ -97,15 +103,15 @@
             ),
             version=effective_version,
             labels=source_labels,
           )
         ],
         componentReferences=[], # added later
         resources=[], # added later
-        labels=list(component_labels),
+        labels=component_labels,
       ),
     )
 
     return base_descriptor_v2
 
 
 def component_diff_since_last_release(
```

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/component_descriptor_util.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/component_descriptor_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/draft_release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/os_id.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/scan_container_images.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/scan_container_images.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/update_component_deps.mako`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 repo_branch = main_repo.branch()
 
 update_component_deps_trait = job_variant.trait('update_component_deps')
 set_dependency_version_script_path = update_component_deps_trait.set_dependency_version_script_path()
 after_merge_callback = update_component_deps_trait.after_merge_callback()
 upstream_update_policy = update_component_deps_trait.upstream_update_policy()
 ignore_prerelease_versions=update_component_deps_trait.ignore_prerelease_versions()
+release_notes_handling=update_component_deps_trait.release_notes_handling()
 component_descriptor_trait = job_variant.trait('component_descriptor')
 ctx_repo = component_descriptor_trait.ctx_repository()
 
 set_version_script_image_cfg = \
     update_component_deps_trait.set_dependency_version_script_container_image()
 if set_version_script_image_cfg:
     set_version_script_image = set_version_script_image_cfg.image_reference()
@@ -91,14 +92,17 @@
 ]
 merge_policy_and_filters = {
     p: component_ref_component_name_filter(
         include_regexes=p.component_names(),
         exclude_regexes=(),
     ) for p in merge_policy_configs
 }
+release_notes_handling = concourse.model.traits.update_component_deps.ReleaseNotesHandling(
+    '${release_notes_handling.value}'
+)
 # indicates whether or not an upstream component was defined as a reference
 upstream_component_name = os.environ.get('UPSTREAM_COMPONENT_NAME', None)
 UPGRADE_TO_UPSTREAM = bool(upstream_component_name)
 
 logger.info(f'{UPGRADE_TO_UPSTREAM=}')
 
 pull_request_util = github.util.PullRequestUtil(
@@ -189,16 +193,17 @@
         merge_method=merge_method,
 % if after_merge_callback:
         after_merge_callback='${after_merge_callback}',
 % endif
 % if set_version_script_image:
         container_image='${set_version_script_image}',
 % else:
-        container_image = None
+        container_image = None,
 % endif
+        release_notes_handling=release_notes_handling,
     )
     # add pr to the list of known upgrade pull requests, so next iteration
     # on the generator returned by determine_upgrade_prs takes it into
     # consideration
     upgrade_pull_requests.append(pull_request)
 
 for upgrade_pull_request in github.util.iter_obsolete_upgrade_pull_requests(
```

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/update_component_deps.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 
 import gci.componentmodel
 import github3.exceptions
 import github3.repos.repo
 
 import ccc.github
 import ci.util
-import cnudie.util
 import cnudie.retrieve
+import cnudie.util
 import concourse.model.traits.update_component_deps
-import concourse.steps.component_descriptor_util as cdu
 import concourse.paths
+import concourse.steps.component_descriptor_util as cdu
 import dockerutil
 import github.util
 import gitutil
 import model.container_registry as cr
 import product.v2
+import release_notes.fetch as release_notes_fetch
 import version
 from concourse.model.traits.update_component_deps import (
     MergePolicy,
     MergeMethod,
+    ReleaseNotesHandling,
 )
 from github.util import (
     GitHubRepoBranch,
 )
 from github.release_notes.util import ReleaseNotes
 
 logger = logging.getLogger('step.update_component_deps')
@@ -265,14 +267,15 @@
                 yield(greatest_component_reference, greatest_version)
 
 
 def _import_release_notes(
     component: gci.componentmodel.Component,
     to_version: str,
     pull_request_util,
+    release_notes_handling: ReleaseNotesHandling = ReleaseNotesHandling.DEFAULT,
 ):
     if not component.sources:
         logger.warning(
             f'''
             {component.name=}:{component.version=} has no sources; skipping release-notes-import
             '''
         )
@@ -285,14 +288,15 @@
 
     release_notes = create_release_notes(
         from_component=component,
         from_github_cfg=github_cfg,
         from_repo_owner=org_name,
         from_repo_name=repository_name,
         to_version=to_version,
+        release_notes_handling=release_notes_handling,
     )
 
     if not release_notes:
         release_notes = pull_request_util.retrieve_pr_template_text()
 
     return release_notes
 
@@ -308,16 +312,16 @@
     githubrepobranch: GitHubRepoBranch,
     repo_dir,
     github_cfg_name,
     merge_policy: MergePolicy,
     merge_method: MergeMethod,
     after_merge_callback=None,
     container_image:str=None,
+    release_notes_handling: ReleaseNotesHandling=ReleaseNotesHandling.DEFAULT,
 ) -> github.util.UpgradePullRequest:
-
     if container_image:
         dockerutil.launch_dockerd_if_not_running()
 
     ls_repo = pull_request_util.repository
 
     from_component_descriptor = component_descriptor_lookup()(
         component_id=gci.componentmodel.ComponentIdentity(
@@ -401,14 +405,15 @@
     )
     # branch was created. Cleanup if something fails
     try:
         release_notes = _import_release_notes(
             component=from_component,
             to_version=to_version,
             pull_request_util=pull_request_util,
+            release_notes_handling=release_notes_handling,
         )
     except Exception:
         logger.warning('failed to retrieve release-notes')
         traceback.print_exc()
         release_notes = 'failed to retrieve release-notes'
 
     if release_notes:
@@ -513,35 +518,52 @@
 
 def create_release_notes(
     from_component: gci.componentmodel.Component,
     from_github_cfg,
     from_repo_owner: str,
     from_repo_name: str,
     to_version: str,
+    release_notes_handling: ReleaseNotesHandling = ReleaseNotesHandling.DEFAULT,
 ):
     from_version = from_component.version
     try:
         with tempfile.TemporaryDirectory() as temp_dir:
             gitutil.GitHelper.clone_into(
                 target_directory=temp_dir,
                 github_cfg=from_github_cfg,
                 github_repo_path=f'{from_repo_owner}/{from_repo_name}'
             )
-            commit_range = '{from_version}..{to_version}'.format(
-                from_version=from_version,
-                to_version=to_version,
-            )
-            release_notes = ReleaseNotes(
-                component=from_component,
-                repo_dir=temp_dir,
-            )
-            release_notes.create(
-                start_ref=None, # the repo's default branch
-                commit_range=commit_range
-            )
-            release_note_blocks = release_notes.release_note_blocks()
-            if release_note_blocks:
-                return f'**Release Notes**:\n{release_note_blocks}'
+            if release_notes_handling is ReleaseNotesHandling.DEFAULT:
+                commit_range = '{from_version}..{to_version}'.format(
+                    from_version=from_version,
+                    to_version=to_version,
+                )
+                release_notes = ReleaseNotes(
+                    component=from_component,
+                    repo_dir=temp_dir,
+                )
+                release_notes.create(
+                    start_ref=None, # the repo's default branch
+                    commit_range=commit_range
+                )
+                release_note_blocks = release_notes.release_note_blocks()
+                if release_note_blocks:
+                    return f'**Release Notes**:\n{release_note_blocks}'
+
+            elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
+                release_note_blocks = release_notes_fetch.fetch_release_notes(
+                    repo_path=temp_dir,
+                    component=from_component,
+                    current_version=version.parse_to_semver(to_version),
+                    previous_version=version.parse_to_semver(from_version),
+                )
+                if release_note_blocks:
+                    n = '\n'
+                    return f'**Release Notes**:\n{n.join(r.block_str for r in release_note_blocks)}'
+
+            else:
+                raise NotImplementedError(release_notes_handling)
+
     except:
         logger.warning('an error occurred during release notes processing (ignoring)')
         import traceback
         logger.warning(traceback.format_exc())
```

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2055.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2055.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/templates/__init__.py` & `gardener-cicd-libs-1.2055.0/concourse/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2055.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/util.py` & `gardener-cicd-libs-1.2055.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/concourse/validator.py` & `gardener-cicd-libs-1.2055.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/container/__init__.py` & `gardener-cicd-libs-1.2055.0/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/container/util.py` & `gardener-cicd-libs-1.2055.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cosign/__init__.py` & `gardener-cicd-libs-1.2055.0/cosign/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/cosign/payload.py` & `gardener-cicd-libs-1.2055.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/cosign.py` & `gardener-cicd-libs-1.2055.0/ctt/cosign.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/filters.py` & `gardener-cicd-libs-1.2055.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/platform.py` & `gardener-cicd-libs-1.2055.0/ctt/platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2055.0/ctt/process_dependencies.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2055.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/processors.py` & `gardener-cicd-libs-1.2055.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2055.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2055.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2055.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2055.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2055.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2055.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2055.0/ctt/uploaders.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/ctt/util.py` & `gardener-cicd-libs-1.2055.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/delivery/client.py` & `gardener-cicd-libs-1.2055.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/delivery/model.py` & `gardener-cicd-libs-1.2055.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/delivery/util.py` & `gardener-cicd-libs-1.2055.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/dockerutil.py` & `gardener-cicd-libs-1.2055.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/dso/cvss.py` & `gardener-cicd-libs-1.2055.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/dso/labels.py` & `gardener-cicd-libs-1.2055.0/dso/labels.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/dso/model.py` & `gardener-cicd-libs-1.2055.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2055.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-gardener-cicd-base>=1.2054.0
-gardener-oci>=1.2054.0
+gardener-cicd-base>=1.2055.0
+gardener-oci>=1.2055.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.13.36
-aliyun-python-sdk-ecs==4.24.31
+aliyun-python-sdk-ecs==4.24.62
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
 bcrypt<5.0.0
 boto3
 cachecontrol<1
 cachetools
 cryptography
```

### Comparing `gardener-cicd-libs-1.2054.0/github/__init__.py` & `gardener-cicd-libs-1.2055.0/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/codeowners.py` & `gardener-cicd-libs-1.2055.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2055.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2055.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/compliance/model.py` & `gardener-cicd-libs-1.2055.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/compliance/report.py` & `gardener-cicd-libs-1.2055.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2055.0/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/release_notes/model.py` & `gardener-cicd-libs-1.2055.0/github/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/release_notes/renderer.py` & `gardener-cicd-libs-1.2055.0/github/release_notes/renderer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/release_notes/util.py` & `gardener-cicd-libs-1.2055.0/github/release_notes/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/retry.py` & `gardener-cicd-libs-1.2055.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/user.py` & `gardener-cicd-libs-1.2055.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/util.py` & `gardener-cicd-libs-1.2055.0/github/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/github/webhook.py` & `gardener-cicd-libs-1.2055.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/gitutil.py` & `gardener-cicd-libs-1.2055.0/gitutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/gziputil.py` & `gardener-cicd-libs-1.2055.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/http_requests.py` & `gardener-cicd-libs-1.2055.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/kube/__init__.py` & `gardener-cicd-libs-1.2055.0/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/kube/ctx.py` & `gardener-cicd-libs-1.2055.0/kube/ctx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/kube/helm.py` & `gardener-cicd-libs-1.2055.0/kube/helm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/kube/helper.py` & `gardener-cicd-libs-1.2055.0/kube/helper.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/mail/__init__.py` & `gardener-cicd-libs-1.2055.0/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2055.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/mailutil.py` & `gardener-cicd-libs-1.2055.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/product/__init__.py` & `gardener-cicd-libs-1.2055.0/product/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/product/util.py` & `gardener-cicd-libs-1.2055.0/product/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/product/v2.py` & `gardener-cicd-libs-1.2055.0/product/v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2055.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2055.0/release_notes/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     ), tuple()
 
 
 def fetch_release_notes(
         component: gci.componentmodel.Component,
         repo_path: str,
         current_version: typing.Optional[semver.VersionInfo] = None,
+        previous_version: typing.Optional[semver.VersionInfo] = None,
 ) -> set[rnm.ReleaseNote]:
     ''' Fetches and returns a set of release notes for the specified component.
 
     :param component: An instance of the Component class from the GCI component model.
     :param repo_path: The (local) path to the git-repository.
     :param current_version: Optional argument to retrieve release notes for a specific version.
     :return: A set of ReleaseNote objects for the specified component.
@@ -180,17 +181,18 @@
         current_version_tag = git_helper.repo.tag(source.access.ref)
     else:
         current_version_tag = git_helper.repo.tag(component_versions[current_version])
 
     if not current_version_tag:
         raise RuntimeError(f'cannot find ref {source.access.ref} in repo')
 
-    previous_version = rnu.find_next_smallest_version(
-        list(component_versions.keys()), current_version
-    )
+    if not previous_version:
+        previous_version = rnu.find_next_smallest_version(
+            list(component_versions.keys()), current_version
+        )
     previous_version_tag: typing.Optional[git.TagReference] = None
     if previous_version:
         previous_version_tag = git_helper.repo.tag(component_versions[previous_version])
 
     logger.debug(f'current: {current_version=}, {current_version_tag=}, ' +
                  f'previous: {previous_version=}, {previous_version_tag=}')
```

### Comparing `gardener-cicd-libs-1.2054.0/release_notes/markdown.py` & `gardener-cicd-libs-1.2055.0/release_notes/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,18 @@
         line: str,
         note: rnm.ReleaseNote,
         category: Title,
         group: Title,
     ) -> ListItem:
     return ListItem(
         level=1,
-        text=f'`[{group.display}]` {line} by {note.author} [{get_reference_for_note(note)}]',
+        text=(
+            f'`[{group.display}]` {line} by '
+            f'{note.source_block.author or note.author} [{get_reference_for_note(note)}]'
+        ),
     )
 
 
 def render(notes: set[rnm.ReleaseNote]):
     objs = []
 
     # order by component
```

### Comparing `gardener-cicd-libs-1.2054.0/release_notes/model.py` & `gardener-cicd-libs-1.2055.0/release_notes/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import dataclasses
 import logging
 import re
 import typing
 
+import requests
+
 import gci.componentmodel
 import git
 import github3.pulls
 
 import cnudie.util
+import cnudie.retrieve
 
 logger = logging.getLogger(__name__)
 
 '''
 This pattern matches code-blocks in the following format:
-```{category} {note_message}
+```{category} {note_message} [source component name] [reference-dependent str] [author]
 {note_message}
 ```
+with the three groups in "[]" being optional by virtue of not being present for commit-attached
+release note blocks.
 \x60 -> `
 '''
 _source_block_pattern = re.compile(
-    r'\x60{3}(?P<category>\w+)\s+(?P<target_group>\w+)\n(?P<note>.+?)\n\x60{3}',
+    pattern=(
+        r'\x60{3}\s*(?P<category>\w+)\s+(?P<target_group>\w+)\s*'
+        r'(?P<source_component_name>\S+)?\s?(?P<reference_str>\S+)?\s?(?P<author>\S+)?'
+        r'\n(?P<note>.+?)\n\x60{3}'
+    ),
    flags=re.DOTALL | re.IGNORECASE | re.MULTILINE
 )
 
 
 @dataclasses.dataclass(frozen=True)
 class Author:
     # for pull requests
@@ -98,39 +107,39 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class PullRequestReference(_Reference):
     ''' Represents the pull requests where the release note came from
     '''
     pull_request: github3.pulls.ShortPullRequest
+    source_block: 'SourceBlock'
 
     @property
     def identifier(self) -> str:
+        if self.source_block.reference_identifier:
+            return self.source_block.reference_identifier.strip('#')
         return str(self.pull_request.number)
 
 
-def create_commit_ref(commit: git.Commit) -> CommitReference:
-    return CommitReference(type=_ref_type_commit, commit=commit)
-
-
-def create_pull_request_ref(pull_request: github3.pulls.ShortPullRequest) -> PullRequestReference:
-    return PullRequestReference(type=_ref_type_pull, pull_request=pull_request)
-
-
 @dataclasses.dataclass(frozen=True)
 class SourceBlock:
     '''Represents the parsed release note code block within a pull request body or a commit message.
 
-    ```{category} {note_message}
+    ```{category} {note_message} [component name] [reference identifier] [author]
     {note_message}
     ```
+    with the triple of componentname, reference identifier, and author only being present for code-
+    blocks being attached to pull requests
     '''
     category: str
     target_group: str
     note_message: str
+    component_name: str | None
+    author: str | None
+    reference_identifier: str | None
 
     @property
     def identifier(self) -> str:
         ''' returns a human-readable identifier which can be used e.g. for duplicate checking.
         does not include line breaks or spaces
         '''
         return f'[{self.category}<{self.target_group}>]{self.note_message}' \
@@ -150,27 +159,47 @@
         if isinstance(other, ReleaseNote):
             return self.__eq__(other.source_block)
         if isinstance(other, SourceBlock):
             return hash(other) == hash(self)
         return False
 
 
+def create_commit_ref(commit: git.Commit, source_block: SourceBlock) -> CommitReference:
+    return CommitReference(type=_ref_type_commit, commit=commit)
+
+
+def create_pull_request_ref(
+        pull_request: github3.pulls.ShortPullRequest,
+        source_block: SourceBlock,
+    ) -> PullRequestReference:
+    return PullRequestReference(
+        type=_ref_type_pull,
+        pull_request=pull_request,
+        source_block=source_block,
+    )
+
+
 def iter_source_blocks(content: str) -> typing.Generator[SourceBlock, None, None]:
     ''' Searches for code blocks in release note notation and returns all found.
     Only valid note blocks are returned, which means that the format has been followed.
     However, it does not check if the category / group exists.
 
     :param content: the content to look for release notes in
     :return: a list of valid note blocks
     '''
     for res in _source_block_pattern.finditer(content.replace('\r\n', '\n')):
         try:
-            block = SourceBlock(category=res.group('category'),
-                                target_group=res.group('target_group'),
-                                note_message=res.group('note'))
+            block = SourceBlock(
+                category=res.group('category'),
+                target_group=res.group('target_group'),
+                note_message=res.group('note'),
+                author=res.group('author'),
+                reference_identifier=res.group('reference_str'),
+                component_name=res.group('source_component_name')
+            )
             if block.has_content():
                 yield block
         except IndexError as e:
             logger.debug(f'cannot find group in content: {e}')
             # group not found, ignore
             continue
 
@@ -197,41 +226,82 @@
     @property
     def reference_str(self) -> str:
         return f'{self.reference.type.identifier}{self.reference.identifier}'
 
     @property
     def block_str(self) -> str:
         src_blk = self.source_block
-        author = self.author.username or self.author.display_name.replace(' ', '-')
-        return f'```{src_blk.category} {src_blk.target_group} {self.source_component.name} ' \
-               f'{self.reference_str} {author}\n' \
-               f'{src_blk.note_message}\n```'
+        author = (
+            src_blk.author or self.author.username or self.author.display_name.replace(' ', '-')
+        )
+        return (
+            f'```{src_blk.category} {src_blk.target_group} {self.source_component.name} '
+            f'{self.reference_str} {author}\n'
+            f'{src_blk.note_message}\n```'
+        )
+
+
+def _source_component(
+    current_component: gci.componentmodel.Component,
+    source_component_name: str,
+) -> gci.componentmodel.Component | None:
+    try:
+        # try to fetch cd for the parsed source repo. The actual version does not matter,
+        # we're only interested in the components GithubAccess (we assume it does not
+        # change).
+        ctx_repo = current_component.current_repository_ctx()
+        component_descriptor_lookup = cnudie.retrieve.create_default_component_descriptor_lookup(
+            default_ctx_repo=ctx_repo,
+        )
+        source_component_descriptor = component_descriptor_lookup(
+            gci.componentmodel.ComponentIdentity(
+                name=source_component_name,
+                version=cnudie.retrieve.greatest_component_version(
+                    component_name=source_component_name,
+                    ctx_repo=ctx_repo,
+                    ignore_prerelease_versions=True,
+                ),
+            ),
+        )
+        return source_component_descriptor.component
+    except requests.exceptions.HTTPError:
+        logger.warning(
+            f'Unable to retrieve component descriptor for source component {source_component_name}'
+        )
+        return None
 
 
 def create_release_note_obj(
         source_block: SourceBlock,
         source_commit: git.Commit,
         raw_body: str,
         author: Author,
         target: typing.Union[git.Commit, github3.pulls.ShortPullRequest],
         source_component: gci.componentmodel.Component,
         current_component: gci.componentmodel.Component
 ) -> ReleaseNote:
     if isinstance(target, git.Commit):
-        ref = create_commit_ref(target)
+        ref = create_commit_ref(target, source_block)
     elif isinstance(target, github3.pulls.ShortPullRequest):
-        ref = create_pull_request_ref(target)
+        ref = create_pull_request_ref(target, source_block)
     else:
         raise ValueError('either target pull request or commit has to be passed')
 
+    if source_block.component_name:
+        source_component = _source_component(
+            current_component=current_component,
+            source_component_name=source_block.component_name,
+        )
+
     # access
     source_component_access = cnudie.util.determine_main_source_for_component(
         component=source_component,
         absent_ok=False
     ).access
+
     current_src_access = cnudie.util.determine_main_source_for_component(
         component=current_component,
         absent_ok=False
     ).access
 
     from_same_github_instance = current_src_access.hostname() in source_component_access.hostname()
     is_current_repo = current_component.name == source_component.name
```

### Comparing `gardener-cicd-libs-1.2054.0/release_notes/utils.py` & `gardener-cicd-libs-1.2055.0/release_notes/utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/reutil.py` & `gardener-cicd-libs-1.2055.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/saf/client.py` & `gardener-cicd-libs-1.2055.0/saf/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/saf/model.py` & `gardener-cicd-libs-1.2055.0/saf/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/setup.py` & `gardener-cicd-libs-1.2055.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/slackclient/__init__.py` & `gardener-cicd-libs-1.2055.0/slackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/slackclient/util.py` & `gardener-cicd-libs-1.2055.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/tarutil.py` & `gardener-cicd-libs-1.2055.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/__init__.py` & `gardener-cicd-libs-1.2055.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/_test_utils.py` & `gardener-cicd-libs-1.2055.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/__init__.py` & `gardener-cicd-libs-1.2055.0/test/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/traits/filter_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2055.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/release_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2055.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/container/__init__.py` & `gardener-cicd-libs-1.2055.0/test/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/__init__.py` & `gardener-cicd-libs-1.2055.0/test/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2055.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2055.0/test/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/release_notes/default_util.py` & `gardener-cicd-libs-1.2055.0/test/github/release_notes/default_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/release_notes/renderer_test.py` & `gardener-cicd-libs-1.2055.0/test/github/release_notes/renderer_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/github/release_notes/util_test.py` & `gardener-cicd-libs-1.2055.0/test/github/release_notes/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/kubeutil_test.py` & `gardener-cicd-libs-1.2055.0/test/kubeutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/product_/__init__.py` & `gardener-cicd-libs-1.2055.0/test/product_/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/reutil_test.py` & `gardener-cicd-libs-1.2055.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/test/version_test.py` & `gardener-cicd-libs-1.2055.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/unixutil/model.py` & `gardener-cicd-libs-1.2055.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/unixutil/scan.py` & `gardener-cicd-libs-1.2055.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2054.0/version.py` & `gardener-cicd-libs-1.2055.0/version.py`

 * *Files identical despite different names*

