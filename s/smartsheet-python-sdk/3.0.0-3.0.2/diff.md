# Comparing `tmp/smartsheet-python-sdk-3.0.0.tar.gz` & `tmp/smartsheet-python-sdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-python-sdk-3.0.0.tar", last modified: Wed Dec  7 13:48:33 2022, max compression
+gzip compressed data, was "smartsheet-python-sdk-3.0.2.tar", last modified: Mon May 15 09:58:07 2023, max compression
```

## Comparing `smartsheet-python-sdk-3.0.0.tar` & `smartsheet-python-sdk-3.0.2.tar`

### file list

```diff
@@ -1,260 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.128693 smartsheet-python-sdk-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.gitchangelog.rc
--rw-r--r--   0 runner    (1001) docker     (123)      482 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.gitchangelog.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.052693 smartsheet-python-sdk-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.060693 smartsheet-python-sdk-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.github/workflows/publish-distribution.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.github/workflows/publish-documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.github/workflows/test-build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/ADVANCED.md
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      420 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2022-12-07 13:48:33.128693 smartsheet-python-sdk-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.060693 smartsheet-python-sdk-3.0.0/docs-source/
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/docs-source/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/docs-source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/docs-source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-07 13:48:33.128693 smartsheet-python-sdk-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.076693 smartsheet-python-sdk-3.0.0/smartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/discussions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/favorites.py
--rw-r--r--   0 runner    (1001) docker     (123)    12011 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.112693 smartsheet-python-sdk-3.0.0/smartsheet/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/alternate_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/auto_number_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/automation_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/automation_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/boolean_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/bulk_item_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/bulk_item_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cell_data_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cell_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cell_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cell_link_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/chart_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/contact_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/container_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/cross_sheet_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/date_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/datetime_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/discussion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/downloaded_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.120693 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_parent_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_action_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_rule_disabled_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/cell_link_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/criteria_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/cross_sheet_reference_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/currency_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/day_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/day_ordinal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_obejct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/global_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/paper_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/predecessor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/publish_accessible_by.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/schedule_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/share_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/share_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_email_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_filter_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/system_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/update_request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/user_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/enums/widget_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/error_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/event_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/explicit_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/font_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/format_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/format_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/group_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/image_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/image_url_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/image_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/index_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/multi_contact_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/multi_picklist_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/multi_row_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/number_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/o_auth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/predecessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/predecessor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/primitive_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/profile_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/report_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/row_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/row_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/search_result_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/selection_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sent_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/share.py
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_filter_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_user_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/shortcut_data_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/shortcut_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sight_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sort_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/sort_specifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/string_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/summary_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/title_rich_text_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/web_content_widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_subscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/widget_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/widget_hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/passthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    70060 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/sights.py
--rw-r--r--   0 runner    (1001) docker     (123)    22520 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/smartsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-07 13:48:32.000000 smartsheet-python-sdk-3.0.0/smartsheet/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17550 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/smartsheet/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.120693 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2022-12-07 13:48:32.000000 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2022-12-07 13:48:33.000000 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 13:48:32.000000 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-07 13:48:32.000000 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-07 13:48:32.000000 smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.056693 smartsheet-python-sdk-3.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.124693 smartsheet-python-sdk-3.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.124693 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/calling_all_curs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/curly.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    65440 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/moe-curly.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/quote.txt
--rw-r--r--   0 runner    (1001) docker     (123)    90832 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/stooges_v1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    30550 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/fixtures/stooges_v2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_cross_sheet_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_discussions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_favorites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_home.py
--rw-r--r--   0 runner    (1001) docker     (123)   100219 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_model_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_multi_picklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_object_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_passthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_server_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_sheet_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_update_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/integration/test_zsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:48:33.128693 smartsheet-python-sdk-3.0.0/tests/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/mock_api_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_automation_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    20957 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_sights.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_change_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2022-12-07 13:48:17.000000 smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.589167 smartsheet-python-sdk-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.gitchangelog.rc
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.gitchangelog.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.561167 smartsheet-python-sdk-3.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.561167 smartsheet-python-sdk-3.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.561167 smartsheet-python-sdk-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.github/workflows/publish-distribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.github/workflows/publish-documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.github/workflows/test-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/ADVANCED.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-15 09:58:07.589167 smartsheet-python-sdk-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.565167 smartsheet-python-sdk-3.0.2/docs-source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/docs-source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/docs-source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/docs-source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-15 09:58:07.589167 smartsheet-python-sdk-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.565167 smartsheet-python-sdk-3.0.2/smartsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/discussions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/favorites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.577167 smartsheet-python-sdk-3.0.2/smartsheet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/alternate_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/auto_number_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/automation_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/automation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/boolean_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/bulk_item_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/bulk_item_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cell_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cell_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cell_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cell_link_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/chart_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/contact_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/container_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/cross_sheet_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/date_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/datetime_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/discussion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/downloaded_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.581167 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_parent_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_action_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_rule_disabled_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/cell_link_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/criteria_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/cross_sheet_reference_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/currency_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/day_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/day_ordinal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_obejct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/global_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/paper_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/predecessor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/publish_accessible_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/schedule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/share_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/share_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_email_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/system_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/update_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/user_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/enums/widget_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/error_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/event_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/explicit_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/font_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/format_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/format_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/group_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/image_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/image_url_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/image_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/index_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/multi_contact_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/multi_picklist_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/multi_row_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/number_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/o_auth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/predecessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/predecessor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/primitive_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/profile_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/report_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/row_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/row_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/search_result_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/selection_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sent_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_filter_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_user_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/shortcut_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/shortcut_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sight_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sort_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/sort_specifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/string_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/summary_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/title_rich_text_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/web_content_widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_subscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/widget_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/widget_hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70060 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/sights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22520 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/smartsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17550 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/smartsheet/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.581167 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 09:58:07.000000 smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.561167 smartsheet-python-sdk-3.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.585167 smartsheet-python-sdk-3.0.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.585167 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/calling_all_curs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/curly.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    65440 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/moe-curly.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/quote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    90832 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/stooges_v1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    30550 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/fixtures/stooges_v2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_cross_sheet_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_discussions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_home.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100219 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_model_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_multi_picklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_object_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_sheet_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_update_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/integration/test_zsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:58:07.589167 smartsheet-python-sdk-3.0.2/tests/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/mock_api_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_automation_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_sights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_change_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-05-15 09:57:50.000000 smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_serialization.py
```

### Comparing `smartsheet-python-sdk-3.0.0/.gitchangelog.rc` & `smartsheet-python-sdk-3.0.2/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/.github/workflows/publish-distribution.yaml` & `smartsheet-python-sdk-3.0.2/.github/workflows/publish-distribution.yaml`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/.github/workflows/publish-documentation.yaml` & `smartsheet-python-sdk-3.0.2/.github/workflows/publish-documentation.yaml`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/ADVANCED.md` & `smartsheet-python-sdk-3.0.2/ADVANCED.md`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/CHANGELOG.md` & `smartsheet-python-sdk-3.0.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [3.0.2] - 2023-05-15
+
+### Updated
+
+- Update urllib3 default retryable methods reference
+
+## [3.0.1] - 2023-03-31
+
+### Updated
+
+- Changing import order to better support later versions of python
+
 ## [3.0.0] - 2022-12-06
 
 ### Updated
 
 - Migrated SDK to new project
 
 ### Added
```

### Comparing `smartsheet-python-sdk-3.0.0/LICENSE.md` & `smartsheet-python-sdk-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/Makefile` & `smartsheet-python-sdk-3.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/PKG-INFO` & `smartsheet-python-sdk-3.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: smartsheet-python-sdk
-Version: 3.0.0
+Version: 3.0.2
 Summary: Library that uses Python to connect to Smartsheet services (using API 2.0).
 Home-page: http://smartsheet-platform.github.io/api-docs/
 Author: Smartsheet
-Author-email: api@smartsheet.com
+Author-email: sdk@smartsheet.com
 License: Apache-2.0
 Keywords: Smartsheet,Collaboration,Project Management,Excel,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 Provides-Extra: test
 Provides-Extra: develop
 License-File: LICENSE.md
 License-File: NOTICE
 
 # Smartsheet Python SDK
 
-[![Build Status](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml/badge.svg)](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml) [![PyPI version](https://badge.fury.io/py/smartsheet-python-sdk.svg)](https://badge.fury.io/py/smartsheet-python-sdk)
+[![Build Status](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml/badge.svg)](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml) [![Coverage Status](https://coveralls.io/repos/github/smartsheet/smartsheet-python-sdk/badge.svg?branch=mainline)](https://coveralls.io/github/smartsheet/smartsheet-python-sdk?branch=mainline) [![PyPI version](https://badge.fury.io/py/smartsheet-python-sdk.svg)](https://badge.fury.io/py/smartsheet-python-sdk)
 
 A library for connecting to the [Smartsheet API](https://smartsheet.redoc.ly) from Python applications.
 
 ## Requirements
 
 The SDK is compatible with [actively supported](https://devguide.python.org/versions/#versions) Python versions `3.10`, `3.9`, `3.8`, `3.7`.
 
@@ -74,7 +74,21 @@
 2. [Python SDK documentation](https://smartsheet.github.io/smartsheet-python-sdk/)
 3. [Smartsheet API Documentation](https://smartsheet.redoc.ly)
 
 ## Advanced Topics
 
 For details about logging, testing, how to use a passthrough option, and how to override HTTP client behavior,
 see [Advanced Topics](ADVANCED.md).
+
+## Developer Agreement
+
+Review the [Developer Program Agreement](https://www.smartsheet.com/legal/developer-program-agreement).
+
+## Acknowledgements
+
+We would like to thank the following people for their contributions to this project:
+
+* Tim Wells - [timwellswa](https://github.com/timwellswa)
+* Scott Wimer - [happybob007](https://github.com/happybob007)
+* Steve Weil - [seweil](https://github.com/seweil)
+* Kevin Fansler - [kfansler](https://github.com/kfansler)
+* Nathan Armstrong - [armstnp](https://github.com/armstnp)
```

### Comparing `smartsheet-python-sdk-3.0.0/docs-source/Makefile` & `smartsheet-python-sdk-3.0.2/docs-source/Makefile`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/docs-source/conf.py` & `smartsheet-python-sdk-3.0.2/docs-source/conf.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/docs-source/index.rst` & `smartsheet-python-sdk-3.0.2/docs-source/index.rst`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/setup.cfg` & `smartsheet-python-sdk-3.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [wheel]
 universal = 1
 
 [tool:pytest]
 addopts = -ra --color=yes --showlocals --verbose --ignore=docs --ignore=examples --tb=native --reruns 2  --reruns-delay 3
 log_cli = true
-log_level = NOTSET
+log_level = ERROR
 
 [coverage:run]
 omit = 
 	smartsheet/exceptions.py
 
 [coverage:report]
 exclude_lines =
```

### Comparing `smartsheet-python-sdk-3.0.0/setup.py` & `smartsheet-python-sdk-3.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
 setup(
     name=NAME,
     description='Library that uses Python to connect to Smartsheet services (using API 2.0).',
     author='Smartsheet',
-    author_email='api@smartsheet.com',
+    author_email='sdk@smartsheet.com',
     url='http://smartsheet-platform.github.io/api-docs/',
     license='Apache-2.0',
     keywords=['Smartsheet', 'Collaboration', 'Project Management', 'Excel', 'spreadsheet'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
@@ -68,18 +68,20 @@
     packages=find_packages(),
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     extras_require={
         'test': [
             'coverage',
+            'coveralls',
             'pytest'
         ],
         'develop': [
             'coverage',
+            'coveralls[yaml]',
             'pytest',
             'pytest-instafail'
         ]
     },
     tests_require=['pytest', 'pytest-rerunfailures'],
     cmdclass={
         'test': PyTest
```

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/__init__.py` & `smartsheet-python-sdk-3.0.2/smartsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/attachments.py` & `smartsheet-python-sdk-3.0.2/smartsheet/attachments.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/cells.py` & `smartsheet-python-sdk-3.0.2/smartsheet/cells.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/contacts.py` & `smartsheet-python-sdk-3.0.2/smartsheet/contacts.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/discussions.py` & `smartsheet-python-sdk-3.0.2/smartsheet/discussions.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/events.py` & `smartsheet-python-sdk-3.0.2/smartsheet/events.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/exceptions.py` & `smartsheet-python-sdk-3.0.2/smartsheet/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/favorites.py` & `smartsheet-python-sdk-3.0.2/smartsheet/favorites.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/folders.py` & `smartsheet-python-sdk-3.0.2/smartsheet/folders.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/groups.py` & `smartsheet-python-sdk-3.0.2/smartsheet/groups.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/home.py` & `smartsheet-python-sdk-3.0.2/smartsheet/home.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/images.py` & `smartsheet-python-sdk-3.0.2/smartsheet/images.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/__init__.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/access_token.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/access_token.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/account.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/account.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/alternate_email.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/alternate_email.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/attachment.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/attachment.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/auto_number_format.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/auto_number_format.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/automation_action.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/automation_action.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/automation_rule.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/automation_rule.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/boolean_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/boolean_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/bulk_item_failure.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/bulk_item_failure.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/bulk_item_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/bulk_item_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cell.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cell.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cell_data_item.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cell_data_item.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cell_history.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cell_history.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cell_link.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cell_link.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cell_link_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cell_link_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/chart_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/chart_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/column.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/column.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/comment.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/comment.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/contact.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/contact.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/contact_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/contact_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/container_destination.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/container_destination.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_destination.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_destination.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_directive.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_directive.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/copy_or_move_row_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/copy_or_move_row_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/criteria.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/criteria.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/cross_sheet_reference.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/cross_sheet_reference.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/currency.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/currency.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/date_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/date_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/datetime_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/datetime_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/discussion.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/discussion.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/downloaded_file.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/downloaded_file.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/duration.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/duration.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/email.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/email.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/__init__.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/access_level.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/access_level.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_parent_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_parent_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_sub_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_sub_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/attachment_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/attachment_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_action_frequency.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_action_frequency.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_action_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_action_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/automation_rule_disabled_reason.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/automation_rule_disabled_reason.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/cell_link_status.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/cell_link_status.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/column_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/column_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/criteria_target.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/criteria_target.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/cross_sheet_reference_status.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/cross_sheet_reference_status.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/currency_code.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/currency_code.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/day_descriptors.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/day_descriptors.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/day_ordinal.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/day_ordinal.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_action.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_action.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_obejct_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_obejct_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/event_source.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/event_source.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/global_template.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/global_template.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/operator.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/operator.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/paper_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/paper_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/predecessor_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/predecessor_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/publish_accessible_by.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/publish_accessible_by.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/schedule_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/schedule_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/share_scope.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/share_scope.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/share_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/share_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_email_format.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_email_format.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_filter_operator.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_filter_operator.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sheet_filter_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sheet_filter_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/sort_direction.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/sort_direction.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/symbol.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/symbol.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/system_column_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/system_column_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/update_request_status.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/update_request_status.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/user_status.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/enums/widget_type.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/enums/widget_type.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/error.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/error.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/error_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/error_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/event.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/event.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/event_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/event_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/explicit_null.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/explicit_null.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/favorite.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/favorite.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/folder.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/folder.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/font_family.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/font_family.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/format_details.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/format_details.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/format_tables.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/format_tables.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/group.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/group.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/group_member.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/group_member.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/home.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/home.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/hyperlink.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/image.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/image.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/image_url.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/image_url.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/image_url_map.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/image_url_map.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/image_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/image_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/index_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/index_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/json_object.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/json_object.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/multi_contact_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/multi_contact_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/multi_picklist_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/multi_picklist_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/multi_row_email.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/multi_row_email.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/number_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/number_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/o_auth_error.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/o_auth_error.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/predecessor.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/predecessor.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/predecessor_list.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/predecessor_list.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/primitive_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/primitive_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/profile_image.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/profile_image.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/project_settings.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/project_settings.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/recipient.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/recipient.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report_cell.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report_cell.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report_column.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report_column.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report_publish.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report_publish.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report_row.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report_row.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/report_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/report_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/row.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/row.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/row_email.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/row_email.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/row_mapping.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/row_mapping.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/schedule.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/schedule.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/scope.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/scope.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/search_result.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/search_result.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/search_result_item.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/search_result_item.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/selection_range.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/selection_range.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sent_update_request.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sent_update_request.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/server_info.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/server_info.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/share.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/share.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_email.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_email.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_filter.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_filter.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_filter_details.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_filter_details.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_publish.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_publish.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_summary.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_summary.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_user_permissions.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_user_permissions.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sheet_user_settings.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sheet_user_settings.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/shortcut_data_item.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/shortcut_data_item.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/shortcut_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/shortcut_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sight.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sight.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sight_publish.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sight_publish.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sort_criterion.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sort_criterion.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/sort_specifier.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/sort_specifier.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/source.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/source.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/string_object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/string_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/summary_field.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/summary_field.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/template.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/template.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/title_rich_text_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/title_rich_text_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/update_request.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/update_request.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/user.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/user.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/user_model.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/user_model.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/user_profile.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/version.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/version.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/web_content_widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/web_content_widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/webhook.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/webhook.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_secret.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_secret.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_stats.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_stats.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/webhook_subscope.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/webhook_subscope.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/widget.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/widget.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/widget_content.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/widget_content.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/widget_hyperlink.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/widget_hyperlink.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/models/workspace.py` & `smartsheet-python-sdk-3.0.2/smartsheet/models/workspace.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/object_value.py` & `smartsheet-python-sdk-3.0.2/smartsheet/object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/passthrough.py` & `smartsheet-python-sdk-3.0.2/smartsheet/passthrough.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/reports.py` & `smartsheet-python-sdk-3.0.2/smartsheet/reports.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/search.py` & `smartsheet-python-sdk-3.0.2/smartsheet/search.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/server.py` & `smartsheet-python-sdk-3.0.2/smartsheet/server.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/session.py` & `smartsheet-python-sdk-3.0.2/smartsheet/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def pinned_session(pool_maxsize=8):
     http_adapter = _SSLAdapter(
         pool_connections=4,
         pool_maxsize=pool_maxsize,
         max_retries=Retry(
-            total=1, method_whitelist=Retry.DEFAULT_METHOD_WHITELIST.union(["POST"])
+            total=1, allowed_methods=Retry.DEFAULT_ALLOWED_METHODS.union(["POST"])
         ),
     )
 
     _session = requests.session()
     _session.hooks = {"response": redact_token}
     _session.mount("https://", http_adapter)
```

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/sheets.py` & `smartsheet-python-sdk-3.0.2/smartsheet/sheets.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/sights.py` & `smartsheet-python-sdk-3.0.2/smartsheet/sights.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/smartsheet.py` & `smartsheet-python-sdk-3.0.2/smartsheet/smartsheet.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/templates.py` & `smartsheet-python-sdk-3.0.2/smartsheet/templates.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/token.py` & `smartsheet-python-sdk-3.0.2/smartsheet/token.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/types.py` & `smartsheet-python-sdk-3.0.2/smartsheet/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=C0111,R0902,R0913,W4904,W0706
+# pylint: disable=C0111,R0902,R0913,W4904,W0706,W0237
 # Smartsheet Python SDK.
 #
 # Copyright 2016 Smartsheet.com, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"): you may
 # not use this file except in compliance with the License. You may obtain
 # a copy of the License at
@@ -12,19 +12,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 try:
-    # For Python versions 2.7 and 3.3 to 3.9, import from collections
-    from collections import MutableSequence
-except ImportError:
     # For Python version >= 3.10 import from collections.abc
     from collections.abc import MutableSequence
+except ImportError:
+    # For Python versions 2.7 and 3.3 to 3.9, import from collections
+    from collections import MutableSequence
 
 import importlib
 import json
 import logging
 from datetime import datetime
 from enum import Enum
```

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/users.py` & `smartsheet-python-sdk-3.0.2/smartsheet/users.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/util.py` & `smartsheet-python-sdk-3.0.2/smartsheet/util.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/webhooks.py` & `smartsheet-python-sdk-3.0.2/smartsheet/webhooks.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet/workspaces.py` & `smartsheet-python-sdk-3.0.2/smartsheet/workspaces.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/PKG-INFO` & `smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: smartsheet-python-sdk
-Version: 3.0.0
+Version: 3.0.2
 Summary: Library that uses Python to connect to Smartsheet services (using API 2.0).
 Home-page: http://smartsheet-platform.github.io/api-docs/
 Author: Smartsheet
-Author-email: api@smartsheet.com
+Author-email: sdk@smartsheet.com
 License: Apache-2.0
 Keywords: Smartsheet,Collaboration,Project Management,Excel,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 Provides-Extra: test
 Provides-Extra: develop
 License-File: LICENSE.md
 License-File: NOTICE
 
 # Smartsheet Python SDK
 
-[![Build Status](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml/badge.svg)](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml) [![PyPI version](https://badge.fury.io/py/smartsheet-python-sdk.svg)](https://badge.fury.io/py/smartsheet-python-sdk)
+[![Build Status](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml/badge.svg)](https://github.com/smartsheet/smartsheet-python-sdk/actions/workflows/test-build.yaml) [![Coverage Status](https://coveralls.io/repos/github/smartsheet/smartsheet-python-sdk/badge.svg?branch=mainline)](https://coveralls.io/github/smartsheet/smartsheet-python-sdk?branch=mainline) [![PyPI version](https://badge.fury.io/py/smartsheet-python-sdk.svg)](https://badge.fury.io/py/smartsheet-python-sdk)
 
 A library for connecting to the [Smartsheet API](https://smartsheet.redoc.ly) from Python applications.
 
 ## Requirements
 
 The SDK is compatible with [actively supported](https://devguide.python.org/versions/#versions) Python versions `3.10`, `3.9`, `3.8`, `3.7`.
 
@@ -74,7 +74,21 @@
 2. [Python SDK documentation](https://smartsheet.github.io/smartsheet-python-sdk/)
 3. [Smartsheet API Documentation](https://smartsheet.redoc.ly)
 
 ## Advanced Topics
 
 For details about logging, testing, how to use a passthrough option, and how to override HTTP client behavior,
 see [Advanced Topics](ADVANCED.md).
+
+## Developer Agreement
+
+Review the [Developer Program Agreement](https://www.smartsheet.com/legal/developer-program-agreement).
+
+## Acknowledgements
+
+We would like to thank the following people for their contributions to this project:
+
+* Tim Wells - [timwellswa](https://github.com/timwellswa)
+* Scott Wimer - [happybob007](https://github.com/happybob007)
+* Steve Weil - [seweil](https://github.com/seweil)
+* Kevin Fansler - [kfansler](https://github.com/kfansler)
+* Nathan Armstrong - [armstnp](https://github.com/armstnp)
```

### Comparing `smartsheet-python-sdk-3.0.0/smartsheet_python_sdk.egg-info/SOURCES.txt` & `smartsheet-python-sdk-3.0.2/smartsheet_python_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 LICENSE.md
 Makefile
 NOTICE
 README.md
 pylintrc
 setup.cfg
 setup.py
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/publish-distribution.yaml
 .github/workflows/publish-documentation.yaml
 .github/workflows/test-build.yaml
 docs-source/Makefile
 docs-source/conf.py
 docs-source/index.rst
 smartsheet/__init__.py
```

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/README.md` & `smartsheet-python-sdk-3.0.2/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/conftest.py` & `smartsheet-python-sdk-3.0.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/fixtures/curly.jpg` & `smartsheet-python-sdk-3.0.2/tests/integration/fixtures/curly.jpg`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/fixtures/moe-curly.jpg` & `smartsheet-python-sdk-3.0.2/tests/integration/fixtures/moe-curly.jpg`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/fixtures/stooges_v1.jpg` & `smartsheet-python-sdk-3.0.2/tests/integration/fixtures/stooges_v1.jpg`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/fixtures/stooges_v2.jpg` & `smartsheet-python-sdk-3.0.2/tests/integration/fixtures/stooges_v2.jpg`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_attachments.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_columns.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_columns.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_contacts.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_contacts.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_cross_sheet_references.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_cross_sheet_references.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_discussions.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_discussions.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_events.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_events.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_favorites.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_favorites.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_folders.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_folders.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_groups.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_groups.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_home.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_home.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_model_attributes.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_model_attributes.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_multi_picklist.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_multi_picklist.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_object_value.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_object_value.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_passthrough.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_regression.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_regression.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_reports.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_reports.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_rows.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_rows.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_sheet_summary.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_sheet_summary.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_sheets.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_sheets.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_templates.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_templates.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_update_requests.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_update_requests.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_users.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_users.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_webhooks.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_workspaces.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/integration/test_zsearch.py` & `smartsheet-python-sdk-3.0.2/tests/integration/test_zsearch.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/mock_api_test_helper.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/mock_api_test_helper.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_automation_rules.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_automation_rules.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_columns.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_columns.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_rows.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_rows.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_sheets.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_sheets.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_api_sights.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_api_sights.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_change_agent.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_change_agent.py`

 * *Files identical despite different names*

### Comparing `smartsheet-python-sdk-3.0.0/tests/mock_api/test_mock_serialization.py` & `smartsheet-python-sdk-3.0.2/tests/mock_api/test_mock_serialization.py`

 * *Files identical despite different names*

