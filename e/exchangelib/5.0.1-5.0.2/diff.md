# Comparing `tmp/exchangelib-5.0.1.tar.gz` & `tmp/exchangelib-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchangelib-5.0.1.tar", last modified: Fri Mar 31 05:47:09 2023, max compression
+gzip compressed data, was "exchangelib-5.0.2.tar", last modified: Thu Apr 13 18:04:18 2023, max compression
```

## Comparing `exchangelib-5.0.1.tar` & `exchangelib-5.0.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.792228 exchangelib-5.0.1/
--rw-r--r--   0 erik       (501) staff       (20)    37894 2023-03-31 05:46:03.000000 exchangelib-5.0.1/CHANGELOG.md
--rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.0.1/LICENSE
--rw-r--r--   0 erik       (501) staff       (20)       75 2022-01-03 12:16:38.000000 exchangelib-5.0.1/MANIFEST.in
--rw-r--r--   0 erik       (501) staff       (20)     2885 2023-03-31 05:47:09.792289 exchangelib-5.0.1/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1978 2022-09-28 08:45:58.000000 exchangelib-5.0.1/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.776853 exchangelib-5.0.1/exchangelib/
--rw-r--r--   0 erik       (501) staff       (20)     2819 2023-03-31 05:44:39.000000 exchangelib-5.0.1/exchangelib/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    31152 2022-11-23 00:50:30.000000 exchangelib-5.0.1/exchangelib/account.py
--rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.0.1/exchangelib/attachments.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.778007 exchangelib-5.0.1/exchangelib/autodiscover/
--rw-r--r--   0 erik       (501) staff       (20)      499 2022-11-23 00:50:30.000000 exchangelib-5.0.1/exchangelib/autodiscover/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.0.1/exchangelib/autodiscover/cache.py
--rw-r--r--   0 erik       (501) staff       (20)    22506 2022-11-30 21:43:31.000000 exchangelib-5.0.1/exchangelib/autodiscover/discovery.py
--rw-r--r--   0 erik       (501) staff       (20)     1830 2022-11-22 19:07:43.000000 exchangelib-5.0.1/exchangelib/autodiscover/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)     4193 2022-10-10 07:45:39.000000 exchangelib-5.0.1/exchangelib/configuration.py
--rw-r--r--   0 erik       (501) staff       (20)    12447 2022-11-21 22:38:53.000000 exchangelib-5.0.1/exchangelib/credentials.py
--rw-r--r--   0 erik       (501) staff       (20)    31303 2022-11-30 18:39:17.000000 exchangelib-5.0.1/exchangelib/errors.py
--rw-r--r--   0 erik       (501) staff       (20)    11472 2022-10-07 07:59:43.000000 exchangelib-5.0.1/exchangelib/ewsdatetime.py
--rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.0.1/exchangelib/extended_properties.py
--rw-r--r--   0 erik       (501) staff       (20)    61782 2022-11-30 22:06:40.000000 exchangelib-5.0.1/exchangelib/fields.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.778707 exchangelib-5.0.1/exchangelib/folders/
--rw-r--r--   0 erik       (501) staff       (20)     4226 2022-11-07 14:00:40.000000 exchangelib-5.0.1/exchangelib/folders/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)    39105 2023-03-29 18:15:54.000000 exchangelib-5.0.1/exchangelib/folders/base.py
--rw-r--r--   0 erik       (501) staff       (20)    23778 2022-10-07 07:55:45.000000 exchangelib-5.0.1/exchangelib/folders/collections.py
--rw-r--r--   0 erik       (501) staff       (20)    18017 2023-03-29 18:15:54.000000 exchangelib-5.0.1/exchangelib/folders/known_folders.py
--rw-r--r--   0 erik       (501) staff       (20)     6876 2022-11-24 12:35:51.000000 exchangelib-5.0.1/exchangelib/folders/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    15627 2023-03-29 18:15:54.000000 exchangelib-5.0.1/exchangelib/folders/roots.py
--rw-r--r--   0 erik       (501) staff       (20)     2934 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/indexed_properties.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.779680 exchangelib-5.0.1/exchangelib/items/
--rw-r--r--   0 erik       (501) staff       (20)     3353 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/items/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/items/base.py
--rw-r--r--   0 erik       (501) staff       (20)    20435 2022-10-07 07:55:45.000000 exchangelib-5.0.1/exchangelib/items/calendar_item.py
--rw-r--r--   0 erik       (501) staff       (20)    14624 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/items/contact.py
--rw-r--r--   0 erik       (501) staff       (20)    18039 2022-12-02 20:29:28.000000 exchangelib-5.0.1/exchangelib/items/item.py
--rw-r--r--   0 erik       (501) staff       (20)     8914 2023-03-29 18:18:14.000000 exchangelib-5.0.1/exchangelib/items/message.py
--rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/items/post.py
--rw-r--r--   0 erik       (501) staff       (20)     5631 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/items/task.py
--rw-r--r--   0 erik       (501) staff       (20)    81744 2022-11-28 19:14:45.000000 exchangelib-5.0.1/exchangelib/properties.py
--rw-r--r--   0 erik       (501) staff       (20)    34775 2022-11-30 21:39:47.000000 exchangelib-5.0.1/exchangelib/protocol.py
--rw-r--r--   0 erik       (501) staff       (20)    29338 2022-10-07 08:02:07.000000 exchangelib-5.0.1/exchangelib/queryset.py
--rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.0.1/exchangelib/recurrence.py
--rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.0.1/exchangelib/restriction.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.786252 exchangelib-5.0.1/exchangelib/services/
--rw-r--r--   0 erik       (501) staff       (20)     3601 2022-11-22 19:07:43.000000 exchangelib-5.0.1/exchangelib/services/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/archive_item.py
--rw-r--r--   0 erik       (501) staff       (20)    46340 2023-03-28 12:39:41.000000 exchangelib-5.0.1/exchangelib/services/common.py
--rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.0.1/exchangelib/services/convert_id.py
--rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/services/copy_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/create_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1883 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/create_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/create_item.py
--rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/services/create_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/delete_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/delete_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/delete_item.py
--rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.0.1/exchangelib/services/delete_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/empty_folder.py
--rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/expand_dl.py
--rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/export_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3632 2022-11-11 08:05:01.000000 exchangelib-5.0.1/exchangelib/services/find_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.0.1/exchangelib/services/find_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.0.1/exchangelib/services/find_people.py
--rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_attachment.py
--rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_delegate.py
--rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2503 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_mail_tips.py
--rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_persona.py
--rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_room_lists.py
--rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_rooms.py
--rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_searchable_mailboxes.py
--rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_server_time_zones.py
--rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_streaming_events.py
--rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_user_availability.py
--rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/get_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/get_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     4338 2022-11-30 21:48:55.000000 exchangelib-5.0.1/exchangelib/services/get_user_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/mark_as_junk.py
--rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/move_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/move_item.py
--rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.0.1/exchangelib/services/resolve_names.py
--rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/send_item.py
--rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.0.1/exchangelib/services/send_notification.py
--rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/set_user_oof_settings.py
--rw-r--r--   0 erik       (501) staff       (20)     4579 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/subscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     3756 2022-11-11 08:05:01.000000 exchangelib-5.0.1/exchangelib/services/sync_folder_hierarchy.py
--rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.0.1/exchangelib/services/sync_folder_items.py
--rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/services/unsubscribe.py
--rw-r--r--   0 erik       (501) staff       (20)     7591 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/update_folder.py
--rw-r--r--   0 erik       (501) staff       (20)     4776 2022-10-07 07:55:45.000000 exchangelib-5.0.1/exchangelib/services/update_item.py
--rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/update_user_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.0.1/exchangelib/services/upload_items.py
--rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.0.1/exchangelib/settings.py
--rw-r--r--   0 erik       (501) staff       (20)     7823 2022-11-30 21:40:36.000000 exchangelib-5.0.1/exchangelib/transport.py
--rw-r--r--   0 erik       (501) staff       (20)    33292 2022-11-30 20:59:23.000000 exchangelib-5.0.1/exchangelib/util.py
--rw-r--r--   0 erik       (501) staff       (20)    13862 2022-11-24 09:26:20.000000 exchangelib-5.0.1/exchangelib/version.py
--rw-r--r--   0 erik       (501) staff       (20)    38139 2023-03-01 20:37:44.000000 exchangelib-5.0.1/exchangelib/winzone.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.777559 exchangelib-5.0.1/exchangelib.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     2885 2023-03-31 05:47:09.000000 exchangelib-5.0.1/exchangelib.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     3813 2023-03-31 05:47:09.000000 exchangelib-5.0.1/exchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-03-31 05:47:09.000000 exchangelib-5.0.1/exchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2022-01-03 12:18:48.000000 exchangelib-5.0.1/exchangelib.egg-info/not-zip-safe
--rw-r--r--   0 erik       (501) staff       (20)      312 2023-03-31 05:47:09.000000 exchangelib-5.0.1/exchangelib.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       12 2023-03-31 05:47:09.000000 exchangelib-5.0.1/exchangelib.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       81 2022-08-22 13:30:34.000000 exchangelib-5.0.1/pyproject.toml
--rw-r--r--   0 erik       (501) staff       (20)      154 2023-03-31 05:47:09.792513 exchangelib-5.0.1/setup.cfg
--rwxr-xr-x   0 erik       (501) staff       (20)     2393 2023-03-31 05:44:04.000000 exchangelib-5.0.1/setup.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-03-31 05:47:09.792096 exchangelib-5.0.1/tests/
--rw-r--r--   0 erik       (501) staff       (20)    14715 2022-11-30 18:48:03.000000 exchangelib-5.0.1/tests/test_account.py
--rw-r--r--   0 erik       (501) staff       (20)    15618 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_attachments.py
--rw-r--r--   0 erik       (501) staff       (20)    35973 2022-11-30 18:11:39.000000 exchangelib-5.0.1/tests/test_autodiscover.py
--rw-r--r--   0 erik       (501) staff       (20)     1834 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_build.py
--rw-r--r--   0 erik       (501) staff       (20)     4400 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_configuration.py
--rw-r--r--   0 erik       (501) staff       (20)     3830 2022-11-22 18:30:26.000000 exchangelib-5.0.1/tests/test_credentials.py
--rw-r--r--   0 erik       (501) staff       (20)      209 2022-11-24 10:58:56.000000 exchangelib-5.0.1/tests/test_errors.py
--rw-r--r--   0 erik       (501) staff       (20)    11982 2022-12-01 22:41:04.000000 exchangelib-5.0.1/tests/test_ewsdatetime.py
--rw-r--r--   0 erik       (501) staff       (20)    18545 2022-11-24 11:58:56.000000 exchangelib-5.0.1/tests/test_extended_properties.py
--rw-r--r--   0 erik       (501) staff       (20)    12255 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_field.py
--rw-r--r--   0 erik       (501) staff       (20)    46328 2023-03-29 18:15:54.000000 exchangelib-5.0.1/tests/test_folder.py
--rw-r--r--   0 erik       (501) staff       (20)    11305 2022-11-07 14:13:49.000000 exchangelib-5.0.1/tests/test_properties.py
--rw-r--r--   0 erik       (501) staff       (20)    47390 2022-11-21 22:41:30.000000 exchangelib-5.0.1/tests/test_protocol.py
--rw-r--r--   0 erik       (501) staff       (20)     3298 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_queryset.py
--rw-r--r--   0 erik       (501) staff       (20)     3816 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_recurrence.py
--rw-r--r--   0 erik       (501) staff       (20)     8397 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_restriction.py
--rw-r--r--   0 erik       (501) staff       (20)    18677 2022-11-30 20:54:49.000000 exchangelib-5.0.1/tests/test_services.py
--rw-r--r--   0 erik       (501) staff       (20)     3963 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_source.py
--rw-r--r--   0 erik       (501) staff       (20)     3550 2022-11-10 14:56:43.000000 exchangelib-5.0.1/tests/test_transport.py
--rw-r--r--   0 erik       (501) staff       (20)    15961 2023-03-01 20:38:00.000000 exchangelib-5.0.1/tests/test_util.py
--rw-r--r--   0 erik       (501) staff       (20)     6055 2022-08-22 13:30:34.000000 exchangelib-5.0.1/tests/test_version.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.187622 exchangelib-5.0.2/
+-rw-r--r--   0 erik       (501) staff       (20)    37984 2023-04-13 18:02:52.000000 exchangelib-5.0.2/CHANGELOG.md
+-rw-r--r--   0 erik       (501) staff       (20)     1313 2022-01-03 12:16:38.000000 exchangelib-5.0.2/LICENSE
+-rw-r--r--   0 erik       (501) staff       (20)       75 2022-01-03 12:16:38.000000 exchangelib-5.0.2/MANIFEST.in
+-rw-r--r--   0 erik       (501) staff       (20)     2885 2023-04-13 18:04:18.187687 exchangelib-5.0.2/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1978 2022-09-28 08:45:58.000000 exchangelib-5.0.2/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.176642 exchangelib-5.0.2/exchangelib/
+-rw-r--r--   0 erik       (501) staff       (20)     2819 2023-04-13 18:02:42.000000 exchangelib-5.0.2/exchangelib/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    31152 2022-11-23 00:50:30.000000 exchangelib-5.0.2/exchangelib/account.py
+-rw-r--r--   0 erik       (501) staff       (20)     9526 2022-11-24 11:30:07.000000 exchangelib-5.0.2/exchangelib/attachments.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.177983 exchangelib-5.0.2/exchangelib/autodiscover/
+-rw-r--r--   0 erik       (501) staff       (20)      499 2022-11-23 00:50:30.000000 exchangelib-5.0.2/exchangelib/autodiscover/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     5986 2022-11-17 13:10:32.000000 exchangelib-5.0.2/exchangelib/autodiscover/cache.py
+-rw-r--r--   0 erik       (501) staff       (20)    22506 2022-11-30 21:43:31.000000 exchangelib-5.0.2/exchangelib/autodiscover/discovery.py
+-rw-r--r--   0 erik       (501) staff       (20)     1830 2022-11-22 19:07:43.000000 exchangelib-5.0.2/exchangelib/autodiscover/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)     4193 2022-10-10 07:45:39.000000 exchangelib-5.0.2/exchangelib/configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)    12447 2022-11-21 22:38:53.000000 exchangelib-5.0.2/exchangelib/credentials.py
+-rw-r--r--   0 erik       (501) staff       (20)    31303 2022-11-30 18:39:17.000000 exchangelib-5.0.2/exchangelib/errors.py
+-rw-r--r--   0 erik       (501) staff       (20)    11472 2022-10-07 07:59:43.000000 exchangelib-5.0.2/exchangelib/ewsdatetime.py
+-rw-r--r--   0 erik       (501) staff       (20)    12821 2022-11-24 11:54:53.000000 exchangelib-5.0.2/exchangelib/extended_properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    61782 2022-11-30 22:06:40.000000 exchangelib-5.0.2/exchangelib/fields.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.178716 exchangelib-5.0.2/exchangelib/folders/
+-rw-r--r--   0 erik       (501) staff       (20)     4226 2022-11-07 14:00:40.000000 exchangelib-5.0.2/exchangelib/folders/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)    39081 2023-04-13 17:51:42.000000 exchangelib-5.0.2/exchangelib/folders/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    23778 2022-10-07 07:55:45.000000 exchangelib-5.0.2/exchangelib/folders/collections.py
+-rw-r--r--   0 erik       (501) staff       (20)    18017 2023-03-29 18:15:54.000000 exchangelib-5.0.2/exchangelib/folders/known_folders.py
+-rw-r--r--   0 erik       (501) staff       (20)     6876 2022-11-24 12:35:51.000000 exchangelib-5.0.2/exchangelib/folders/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    15880 2023-04-13 17:50:41.000000 exchangelib-5.0.2/exchangelib/folders/roots.py
+-rw-r--r--   0 erik       (501) staff       (20)     2934 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/indexed_properties.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.179647 exchangelib-5.0.2/exchangelib/items/
+-rw-r--r--   0 erik       (501) staff       (20)     3353 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/items/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     9898 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/items/base.py
+-rw-r--r--   0 erik       (501) staff       (20)    20435 2022-10-07 07:55:45.000000 exchangelib-5.0.2/exchangelib/items/calendar_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    14624 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/items/contact.py
+-rw-r--r--   0 erik       (501) staff       (20)    18039 2022-12-02 20:29:28.000000 exchangelib-5.0.2/exchangelib/items/item.py
+-rw-r--r--   0 erik       (501) staff       (20)     8914 2023-03-29 18:18:14.000000 exchangelib-5.0.2/exchangelib/items/message.py
+-rw-r--r--   0 erik       (501) staff       (20)     1405 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/items/post.py
+-rw-r--r--   0 erik       (501) staff       (20)     5631 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/items/task.py
+-rw-r--r--   0 erik       (501) staff       (20)    81744 2022-11-28 19:14:45.000000 exchangelib-5.0.2/exchangelib/properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    34775 2022-11-30 21:39:47.000000 exchangelib-5.0.2/exchangelib/protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)    29338 2022-10-07 08:02:07.000000 exchangelib-5.0.2/exchangelib/queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)    13139 2022-10-07 08:02:07.000000 exchangelib-5.0.2/exchangelib/recurrence.py
+-rw-r--r--   0 erik       (501) staff       (20)    25489 2022-10-07 08:04:06.000000 exchangelib-5.0.2/exchangelib/restriction.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.184950 exchangelib-5.0.2/exchangelib/services/
+-rw-r--r--   0 erik       (501) staff       (20)     3601 2022-11-22 19:07:43.000000 exchangelib-5.0.2/exchangelib/services/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     1247 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/archive_item.py
+-rw-r--r--   0 erik       (501) staff       (20)    46340 2023-03-28 12:39:41.000000 exchangelib-5.0.2/exchangelib/services/common.py
+-rw-r--r--   0 erik       (501) staff       (20)     2097 2022-11-07 14:52:15.000000 exchangelib-5.0.2/exchangelib/services/convert_id.py
+-rw-r--r--   0 erik       (501) staff       (20)      209 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/services/copy_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1532 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/create_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1883 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/create_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4272 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/create_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      686 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/services/create_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)      969 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/delete_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)      931 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/delete_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     2504 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/delete_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      710 2022-08-22 13:30:33.000000 exchangelib-5.0.2/exchangelib/services/delete_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1088 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/empty_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)      889 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/expand_dl.py
+-rw-r--r--   0 erik       (501) staff       (20)     1060 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/export_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3632 2022-11-11 08:05:01.000000 exchangelib-5.0.2/exchangelib/services/find_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4326 2022-11-11 08:05:01.000000 exchangelib-5.0.2/exchangelib/services/find_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4768 2022-11-11 08:05:01.000000 exchangelib-5.0.2/exchangelib/services/find_people.py
+-rw-r--r--   0 erik       (501) staff       (20)     5392 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_attachment.py
+-rw-r--r--   0 erik       (501) staff       (20)     1914 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_delegate.py
+-rw-r--r--   0 erik       (501) staff       (20)     1186 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2503 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1627 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1576 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_mail_tips.py
+-rw-r--r--   0 erik       (501) staff       (20)     1127 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_persona.py
+-rw-r--r--   0 erik       (501) staff       (20)      696 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_room_lists.py
+-rw-r--r--   0 erik       (501) staff       (20)      785 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_rooms.py
+-rw-r--r--   0 erik       (501) staff       (20)     2114 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_searchable_mailboxes.py
+-rw-r--r--   0 erik       (501) staff       (20)     1475 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_server_time_zones.py
+-rw-r--r--   0 erik       (501) staff       (20)     5077 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_streaming_events.py
+-rw-r--r--   0 erik       (501) staff       (20)     2217 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_user_availability.py
+-rw-r--r--   0 erik       (501) staff       (20)     1584 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/get_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     1518 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/get_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4338 2022-11-30 21:48:55.000000 exchangelib-5.0.2/exchangelib/services/get_user_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     1085 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/mark_as_junk.py
+-rw-r--r--   0 erik       (501) staff       (20)     1276 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/move_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     1237 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/move_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     4812 2022-11-11 12:12:44.000000 exchangelib-5.0.2/exchangelib/services/resolve_names.py
+-rw-r--r--   0 erik       (501) staff       (20)     1243 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/send_item.py
+-rw-r--r--   0 erik       (501) staff       (20)     1603 2022-11-10 14:59:43.000000 exchangelib-5.0.2/exchangelib/services/send_notification.py
+-rw-r--r--   0 erik       (501) staff       (20)     1503 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/set_user_oof_settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     4579 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/subscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     3756 2022-11-11 08:05:01.000000 exchangelib-5.0.2/exchangelib/services/sync_folder_hierarchy.py
+-rw-r--r--   0 erik       (501) staff       (20)     3590 2022-11-11 12:09:18.000000 exchangelib-5.0.2/exchangelib/services/sync_folder_items.py
+-rw-r--r--   0 erik       (501) staff       (20)      738 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/services/unsubscribe.py
+-rw-r--r--   0 erik       (501) staff       (20)     7591 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/update_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)     4776 2022-10-07 07:55:45.000000 exchangelib-5.0.2/exchangelib/services/update_item.py
+-rw-r--r--   0 erik       (501) staff       (20)      663 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/update_user_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     2113 2022-11-07 13:44:09.000000 exchangelib-5.0.2/exchangelib/services/upload_items.py
+-rw-r--r--   0 erik       (501) staff       (20)     3907 2022-08-22 13:30:34.000000 exchangelib-5.0.2/exchangelib/settings.py
+-rw-r--r--   0 erik       (501) staff       (20)     7823 2022-11-30 21:40:36.000000 exchangelib-5.0.2/exchangelib/transport.py
+-rw-r--r--   0 erik       (501) staff       (20)    33292 2022-11-30 20:59:23.000000 exchangelib-5.0.2/exchangelib/util.py
+-rw-r--r--   0 erik       (501) staff       (20)    13862 2022-11-24 09:26:20.000000 exchangelib-5.0.2/exchangelib/version.py
+-rw-r--r--   0 erik       (501) staff       (20)    38139 2023-03-01 20:37:44.000000 exchangelib-5.0.2/exchangelib/winzone.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.177366 exchangelib-5.0.2/exchangelib.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     2885 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     3813 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/not-zip-safe
+-rw-r--r--   0 erik       (501) staff       (20)      312 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       12 2023-04-13 18:04:18.000000 exchangelib-5.0.2/exchangelib.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       81 2022-08-22 13:30:34.000000 exchangelib-5.0.2/pyproject.toml
+-rw-r--r--   0 erik       (501) staff       (20)      154 2023-04-13 18:04:18.187960 exchangelib-5.0.2/setup.cfg
+-rwxr-xr-x   0 erik       (501) staff       (20)     2429 2023-04-13 18:04:16.000000 exchangelib-5.0.2/setup.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-04-13 18:04:18.187501 exchangelib-5.0.2/tests/
+-rw-r--r--   0 erik       (501) staff       (20)    14715 2022-11-30 18:48:03.000000 exchangelib-5.0.2/tests/test_account.py
+-rw-r--r--   0 erik       (501) staff       (20)    15618 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_attachments.py
+-rw-r--r--   0 erik       (501) staff       (20)    35973 2022-11-30 18:11:39.000000 exchangelib-5.0.2/tests/test_autodiscover.py
+-rw-r--r--   0 erik       (501) staff       (20)     1834 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_build.py
+-rw-r--r--   0 erik       (501) staff       (20)     4400 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_configuration.py
+-rw-r--r--   0 erik       (501) staff       (20)     3830 2022-11-22 18:30:26.000000 exchangelib-5.0.2/tests/test_credentials.py
+-rw-r--r--   0 erik       (501) staff       (20)      209 2022-11-24 10:58:56.000000 exchangelib-5.0.2/tests/test_errors.py
+-rw-r--r--   0 erik       (501) staff       (20)    11982 2022-12-01 22:41:04.000000 exchangelib-5.0.2/tests/test_ewsdatetime.py
+-rw-r--r--   0 erik       (501) staff       (20)    18545 2022-11-24 11:58:56.000000 exchangelib-5.0.2/tests/test_extended_properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    12255 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_field.py
+-rw-r--r--   0 erik       (501) staff       (20)    46501 2023-04-13 17:45:27.000000 exchangelib-5.0.2/tests/test_folder.py
+-rw-r--r--   0 erik       (501) staff       (20)    11305 2022-11-07 14:13:49.000000 exchangelib-5.0.2/tests/test_properties.py
+-rw-r--r--   0 erik       (501) staff       (20)    47390 2022-11-21 22:41:30.000000 exchangelib-5.0.2/tests/test_protocol.py
+-rw-r--r--   0 erik       (501) staff       (20)     3298 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_queryset.py
+-rw-r--r--   0 erik       (501) staff       (20)     3816 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_recurrence.py
+-rw-r--r--   0 erik       (501) staff       (20)     8397 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_restriction.py
+-rw-r--r--   0 erik       (501) staff       (20)    18677 2022-11-30 20:54:49.000000 exchangelib-5.0.2/tests/test_services.py
+-rw-r--r--   0 erik       (501) staff       (20)     3963 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_source.py
+-rw-r--r--   0 erik       (501) staff       (20)     3550 2022-11-10 14:56:43.000000 exchangelib-5.0.2/tests/test_transport.py
+-rw-r--r--   0 erik       (501) staff       (20)    15961 2023-03-01 20:38:00.000000 exchangelib-5.0.2/tests/test_util.py
+-rw-r--r--   0 erik       (501) staff       (20)     6055 2022-08-22 13:30:34.000000 exchangelib-5.0.2/tests/test_version.py
```

### Comparing `exchangelib-5.0.1/CHANGELOG.md` & `exchangelib-5.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Change Log
 ==========
 
 HEAD
 ----
 
 
+5.0.2
+-----
+- Fix bug where certain folders were being assigned the wrong Python class.
+
+
 5.0.1
 -----
 - Fix PyPI package. No source code changes.
 
 
 5.0.0
 -----
```

### Comparing `exchangelib-5.0.1/LICENSE` & `exchangelib-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/PKG-INFO` & `exchangelib-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.0.1
+Version: 5.0.2
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Home-page: https://github.com/ecederstrand/exchangelib
 Author: Erik Cederstrand
 Author-email: erik@cederstrand.dk
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
```

### Comparing `exchangelib-5.0.1/README.md` & `exchangelib-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/__init__.py` & `exchangelib-5.0.2/exchangelib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .properties import UID, Attendee, Body, DLMailbox, HTMLBody, ItemId, Mailbox, Room, RoomList
 from .protocol import BaseProtocol, FailFast, FaultTolerance, NoVerifyHTTPAdapter, TLSClientAuth
 from .restriction import Q
 from .settings import OofSettings
 from .transport import BASIC, CBA, DIGEST, GSSAPI, NTLM, OAUTH2, SSPI
 from .version import Build, Version
 
-__version__ = "5.0.1"
+__version__ = "5.0.2"
 
 __all__ = [
     "__version__",
     "AcceptItem",
     "Account",
     "Attendee",
     "BASIC",
```

### Comparing `exchangelib-5.0.1/exchangelib/account.py` & `exchangelib-5.0.2/exchangelib/account.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/attachments.py` & `exchangelib-5.0.2/exchangelib/attachments.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/autodiscover/cache.py` & `exchangelib-5.0.2/exchangelib/autodiscover/cache.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/autodiscover/discovery.py` & `exchangelib-5.0.2/exchangelib/autodiscover/discovery.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/autodiscover/protocol.py` & `exchangelib-5.0.2/exchangelib/autodiscover/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/configuration.py` & `exchangelib-5.0.2/exchangelib/configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/credentials.py` & `exchangelib-5.0.2/exchangelib/credentials.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/errors.py` & `exchangelib-5.0.2/exchangelib/errors.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/ewsdatetime.py` & `exchangelib-5.0.2/exchangelib/ewsdatetime.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/extended_properties.py` & `exchangelib-5.0.2/exchangelib/extended_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/fields.py` & `exchangelib-5.0.2/exchangelib/fields.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/folders/__init__.py` & `exchangelib-5.0.2/exchangelib/folders/__init__.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/folders/base.py` & `exchangelib-5.0.2/exchangelib/folders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,15 +904,15 @@
             # https://docs.microsoft.com/en-us/powershell/module/exchange/client-access/Set-MailboxRegionalConfiguration
             #
             # Instead, search for a folder class using the localized name. If none are found, fall back to getting the
             # folder class by the "FolderClass" value.
             #
             # The returned XML may contain neither folder class nor name. In that case, we default to the generic
             # Folder class.
-            if folder.name and folder.folder_class:
+            if folder.name:
                 with suppress(KeyError):
                     # TODO: fld_class.LOCALIZED_NAMES is most definitely neither complete nor authoritative
                     folder_cls = root.folder_cls_from_folder_name(
                         folder_name=folder.name,
                         folder_class=folder.folder_class,
                         locale=root.account.locale,
                     )
```

### Comparing `exchangelib-5.0.1/exchangelib/folders/collections.py` & `exchangelib-5.0.2/exchangelib/folders/collections.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/folders/known_folders.py` & `exchangelib-5.0.2/exchangelib/folders/known_folders.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/folders/queryset.py` & `exchangelib-5.0.2/exchangelib/folders/queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/folders/roots.py` & `exchangelib-5.0.2/exchangelib/folders/roots.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,21 +199,27 @@
 
     @classmethod
     def folder_cls_from_folder_name(cls, folder_name, folder_class, locale):
         """Return the folder class that matches a localized folder name. Take into account the 'folder_class' of the
         folder, to not identify an 'IPF.Note' folder as a 'Calendar' class just because it's called e.g. 'Kalender' and
         the locale is 'da_DK'.
 
+        Some folders, e.g. `System`, don't define a `folder_class`. For these folders, we match on localized folder name
+        if the folder class does not have its 'CONTAINER_CLASS' set.
+
         :param folder_name:
         :param folder_class:
         :param locale: a string, e.g. 'da_DK'
         """
         for folder_cls in cls.WELLKNOWN_FOLDERS + NON_DELETABLE_FOLDERS + MISC_FOLDERS:
-            if folder_cls.CONTAINER_CLASS == folder_class and folder_name.lower() in folder_cls.localized_names(locale):
-                return folder_cls
+            if folder_cls.CONTAINER_CLASS != folder_class:
+                continue
+            if folder_name.lower() not in folder_cls.localized_names(locale):
+                continue
+            return folder_cls
         raise KeyError()
 
     def __getstate__(self):
         # The lock cannot be pickled
         state = {k: getattr(self, k) for k in self._slots_keys}
         del state["_subfolders_lock"]
         return state
```

### Comparing `exchangelib-5.0.1/exchangelib/indexed_properties.py` & `exchangelib-5.0.2/exchangelib/indexed_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/__init__.py` & `exchangelib-5.0.2/exchangelib/items/__init__.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/base.py` & `exchangelib-5.0.2/exchangelib/items/base.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/calendar_item.py` & `exchangelib-5.0.2/exchangelib/items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/contact.py` & `exchangelib-5.0.2/exchangelib/items/contact.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/item.py` & `exchangelib-5.0.2/exchangelib/items/item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/message.py` & `exchangelib-5.0.2/exchangelib/items/message.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/post.py` & `exchangelib-5.0.2/exchangelib/items/post.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/items/task.py` & `exchangelib-5.0.2/exchangelib/items/task.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/properties.py` & `exchangelib-5.0.2/exchangelib/properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/protocol.py` & `exchangelib-5.0.2/exchangelib/protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/queryset.py` & `exchangelib-5.0.2/exchangelib/queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/recurrence.py` & `exchangelib-5.0.2/exchangelib/recurrence.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/restriction.py` & `exchangelib-5.0.2/exchangelib/restriction.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/__init__.py` & `exchangelib-5.0.2/exchangelib/services/__init__.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/archive_item.py` & `exchangelib-5.0.2/exchangelib/services/archive_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/common.py` & `exchangelib-5.0.2/exchangelib/services/common.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/convert_id.py` & `exchangelib-5.0.2/exchangelib/services/convert_id.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/create_attachment.py` & `exchangelib-5.0.2/exchangelib/services/create_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/create_folder.py` & `exchangelib-5.0.2/exchangelib/services/create_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/create_item.py` & `exchangelib-5.0.2/exchangelib/services/create_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/create_user_configuration.py` & `exchangelib-5.0.2/exchangelib/services/create_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/delete_attachment.py` & `exchangelib-5.0.2/exchangelib/services/delete_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/delete_folder.py` & `exchangelib-5.0.2/exchangelib/services/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/delete_item.py` & `exchangelib-5.0.2/exchangelib/services/delete_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/delete_user_configuration.py` & `exchangelib-5.0.2/exchangelib/services/delete_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/empty_folder.py` & `exchangelib-5.0.2/exchangelib/services/empty_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/expand_dl.py` & `exchangelib-5.0.2/exchangelib/services/expand_dl.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/export_items.py` & `exchangelib-5.0.2/exchangelib/services/export_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/find_folder.py` & `exchangelib-5.0.2/exchangelib/services/find_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/find_item.py` & `exchangelib-5.0.2/exchangelib/services/find_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/find_people.py` & `exchangelib-5.0.2/exchangelib/services/find_people.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_attachment.py` & `exchangelib-5.0.2/exchangelib/services/get_attachment.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_delegate.py` & `exchangelib-5.0.2/exchangelib/services/get_delegate.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_events.py` & `exchangelib-5.0.2/exchangelib/services/get_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_folder.py` & `exchangelib-5.0.2/exchangelib/services/get_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_item.py` & `exchangelib-5.0.2/exchangelib/services/get_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_mail_tips.py` & `exchangelib-5.0.2/exchangelib/services/get_mail_tips.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_persona.py` & `exchangelib-5.0.2/exchangelib/services/get_persona.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_room_lists.py` & `exchangelib-5.0.2/exchangelib/services/get_room_lists.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_rooms.py` & `exchangelib-5.0.2/exchangelib/services/get_rooms.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_searchable_mailboxes.py` & `exchangelib-5.0.2/exchangelib/services/get_searchable_mailboxes.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_server_time_zones.py` & `exchangelib-5.0.2/exchangelib/services/get_server_time_zones.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_streaming_events.py` & `exchangelib-5.0.2/exchangelib/services/get_streaming_events.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_user_availability.py` & `exchangelib-5.0.2/exchangelib/services/get_user_availability.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_user_configuration.py` & `exchangelib-5.0.2/exchangelib/services/get_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_user_oof_settings.py` & `exchangelib-5.0.2/exchangelib/services/get_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/get_user_settings.py` & `exchangelib-5.0.2/exchangelib/services/get_user_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/mark_as_junk.py` & `exchangelib-5.0.2/exchangelib/services/mark_as_junk.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/move_folder.py` & `exchangelib-5.0.2/exchangelib/services/move_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/move_item.py` & `exchangelib-5.0.2/exchangelib/services/move_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/resolve_names.py` & `exchangelib-5.0.2/exchangelib/services/resolve_names.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/send_item.py` & `exchangelib-5.0.2/exchangelib/services/send_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/send_notification.py` & `exchangelib-5.0.2/exchangelib/services/send_notification.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/set_user_oof_settings.py` & `exchangelib-5.0.2/exchangelib/services/set_user_oof_settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/subscribe.py` & `exchangelib-5.0.2/exchangelib/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/sync_folder_hierarchy.py` & `exchangelib-5.0.2/exchangelib/services/sync_folder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/sync_folder_items.py` & `exchangelib-5.0.2/exchangelib/services/sync_folder_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/unsubscribe.py` & `exchangelib-5.0.2/exchangelib/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/update_folder.py` & `exchangelib-5.0.2/exchangelib/services/update_folder.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/update_item.py` & `exchangelib-5.0.2/exchangelib/services/update_item.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/update_user_configuration.py` & `exchangelib-5.0.2/exchangelib/services/update_user_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/services/upload_items.py` & `exchangelib-5.0.2/exchangelib/services/upload_items.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/settings.py` & `exchangelib-5.0.2/exchangelib/settings.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/transport.py` & `exchangelib-5.0.2/exchangelib/transport.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/util.py` & `exchangelib-5.0.2/exchangelib/util.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/version.py` & `exchangelib-5.0.2/exchangelib/version.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib/winzone.py` & `exchangelib-5.0.2/exchangelib/winzone.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/exchangelib.egg-info/PKG-INFO` & `exchangelib-5.0.2/exchangelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangelib
-Version: 5.0.1
+Version: 5.0.2
 Summary: Client for Microsoft Exchange Web Services (EWS)
 Home-page: https://github.com/ecederstrand/exchangelib
 Author: Erik Cederstrand
 Author-email: erik@cederstrand.dk
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/ecederstrand/exchangelib/issues
 Project-URL: Documentation, https://ecederstrand.github.io/exchangelib/
```

### Comparing `exchangelib-5.0.1/exchangelib.egg-info/SOURCES.txt` & `exchangelib-5.0.2/exchangelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/setup.py` & `exchangelib-5.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """
 Release notes:
 *  Install pdoc3, wheel, twine
 * Bump version in exchangelib/__init__.py
 * Bump version in CHANGELOG.md
-* Generate documentation: pdoc3 --html exchangelib -o docs --force
+* Generate documentation: pdoc3 --html exchangelib -o docs --force && pre-commit run end-of-file-fixer
 * Commit and push changes
 * Build package: rm -rf build dist && python setup.py sdist bdist_wheel
 * Push to PyPI: twine upload dist/*
 * Create release on GitHub
 """
 from pathlib import Path
```

### Comparing `exchangelib-5.0.1/tests/test_account.py` & `exchangelib-5.0.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_attachments.py` & `exchangelib-5.0.2/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_autodiscover.py` & `exchangelib-5.0.2/tests/test_autodiscover.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_build.py` & `exchangelib-5.0.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_configuration.py` & `exchangelib-5.0.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_credentials.py` & `exchangelib-5.0.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_ewsdatetime.py` & `exchangelib-5.0.2/tests/test_ewsdatetime.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_extended_properties.py` & `exchangelib-5.0.2/tests/test_extended_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_field.py` & `exchangelib-5.0.2/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_folder.py` & `exchangelib-5.0.2/tests/test_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     NON_DELETABLE_FOLDERS,
     SHALLOW,
     AllContacts,
     AllItems,
     ApplicationData,
     Birthdays,
     Calendar,
+    CommonViews,
     Companies,
     Contacts,
     ConversationSettings,
     CrawlerData,
     DefaultFoldersChangeHistory,
     DeletedItems,
     DistinguishedFolderId,
@@ -685,14 +686,18 @@
             self.account.root.clear_cache()
             test_folder = f / misleading_name
             self.assertEqual(type(test_folder), Messages)
             self.assertEqual(test_folder.folder_class, Messages.CONTAINER_CLASS)
         finally:
             self.account.locale = old_locale
 
+        # Also test folders that don't have a CONTAINER_CLASS
+        f = self.account.root / "Common Views"
+        self.assertIsInstance(f, CommonViews)
+
     def test_wipe_without_empty(self):
         name = get_random_string(16)
         f = Messages(parent=self.account.inbox, name=name).save()
         Messages(parent=f, name=get_random_string(16)).save()
         self.assertEqual(len(list(f.children)), 1)
         tmp = f.empty
         try:
```

### Comparing `exchangelib-5.0.1/tests/test_properties.py` & `exchangelib-5.0.2/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_protocol.py` & `exchangelib-5.0.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_queryset.py` & `exchangelib-5.0.2/tests/test_queryset.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_recurrence.py` & `exchangelib-5.0.2/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_restriction.py` & `exchangelib-5.0.2/tests/test_restriction.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_services.py` & `exchangelib-5.0.2/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_source.py` & `exchangelib-5.0.2/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_transport.py` & `exchangelib-5.0.2/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_util.py` & `exchangelib-5.0.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `exchangelib-5.0.1/tests/test_version.py` & `exchangelib-5.0.2/tests/test_version.py`

 * *Files identical despite different names*

