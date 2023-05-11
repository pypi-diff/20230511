# Comparing `tmp/aliyun-python-sdk-quickbi-public-2.1.1.tar.gz` & `tmp/aliyun-python-sdk-quickbi-public-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-quickbi-public-2.1.1.tar", last modified: Thu Sep  8 13:27:20 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-quickbi-public-2.1.2.tar", last modified: Thu May 11 02:50:51 2023, max compression
```

## Comparing `aliyun-python-sdk-quickbi-public-2.1.1.tar` & `aliyun-python-sdk-quickbi-public-2.1.2.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/
--rw-r--r--   0 root         (0) root         (0)      575 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1592 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1592 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6237 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/
--rw-r--r--   0 root         (0) root         (0)     1256 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1972 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1950 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1415 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1960 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1407 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1554 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1558 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1789 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py
--rw-r--r--   0 root         (0) root         (0)     1363 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1594 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py
--rw-r--r--   0 root         (0) root         (0)     1357 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py
--rw-r--r--   0 root         (0) root         (0)     2710 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1911 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1280 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1375 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1182 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1401 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1397 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1405 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1218 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1186 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1196 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1228 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1188 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1403 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1401 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1729 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1391 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2105 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1202 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1208 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1202 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1025 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1202 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1226 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1198 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1188 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1280 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1401 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1208 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1545 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1411 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1030 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1199 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1218 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py
--rw-r--r--   0 root         (0) root         (0)     1984 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2175 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1184 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1761 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1600 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py
--rw-r--r--   0 root         (0) root         (0)     1357 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1612 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1240 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1568 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1375 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1678 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1936 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1534 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1572 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2022-09-08 13:27:20.000000 aliyun-python-sdk-quickbi-public-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-05-11 02:50:51.000000 aliyun-python-sdk-quickbi-public-2.1.2/setup.py
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/LICENSE` & `aliyun-python-sdk-quickbi-public-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/PKG-INFO` & `aliyun-python-sdk-quickbi-public-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-quickbi-public
-Version: 2.1.1
+Version: 2.1.2
 Summary: The quickbi-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-quickbi-public
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/README.rst` & `aliyun-python-sdk-quickbi-public-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-quickbi-public
-Version: 2.1.1
+Version: 2.1.2
 Summary: The quickbi-public module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-quickbi-public
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyun_python_sdk_quickbi_public.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py
 aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py
+aliyunsdkquickbi_public/request/v20220101/AllotDatasetAccelerationTaskRequest.py
 aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py
 aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py
 aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py
 aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py
 aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py
 aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py
 aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py
@@ -35,24 +36,26 @@
 aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py
 aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py
 aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py
 aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py
 aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py
 aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py
 aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py
+aliyunsdkquickbi_public/request/v20220101/ListApiDatasourceRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py
 aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py
+aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py
 aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionRuleUsersRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddDataLevelPermissionRuleUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddDataLevelPermissionRuleUsers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddDataLevelPermissionRuleUsers','2.2.0')
 		self.set_method('POST')
 
 	def get_AddUserModel(self): # String
 		return self.get_query_params().get('AddUserModel')
 
 	def set_AddUserModel(self, AddUserModel):  # String
 		self.add_query_param('AddUserModel', AddUserModel)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddDataLevelPermissionWhiteListRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddDataLevelPermissionWhiteListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddDataLevelPermissionWhiteList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddDataLevelPermissionWhiteList','2.2.0')
 		self.set_method('POST')
 
 	def get_TargetType(self): # String
 		return self.get_query_params().get('TargetType')
 
 	def set_TargetType(self, TargetType):  # String
 		self.add_query_param('TargetType', TargetType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddShareReportRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddShareReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddShareReport','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddShareReport','2.2.0')
 		self.set_method('POST')
 
 	def get_AuthPoint(self): # Integer
 		return self.get_query_params().get('AuthPoint')
 
 	def set_AuthPoint(self, AuthPoint):  # Integer
 		self.add_query_param('AuthPoint', AuthPoint)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMemberRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddUserGroupMemberRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserGroupMember','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserGroupMember','2.2.0')
 		self.set_method('POST')
 
 	def get_UserIdList(self): # String
 		return self.get_query_params().get('UserIdList')
 
 	def set_UserIdList(self, UserIdList):  # String
 		self.add_query_param('UserIdList', UserIdList)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserGroupMembersRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddUserGroupMembersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserGroupMembers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserGroupMembers','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupIds(self): # String
 		return self.get_query_params().get('UserGroupIds')
 
 	def set_UserGroupIds(self, UserGroupIds):  # String
 		self.add_query_param('UserGroupIds', UserGroupIds)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUser','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUser','2.2.0')
 		self.set_method('POST')
 
 	def get_AdminUser(self): # Boolean
 		return self.get_query_params().get('AdminUser')
 
 	def set_AdminUser(self, AdminUser):  # Boolean
 		self.add_query_param('AdminUser', AdminUser)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserTagMetaRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddUserTagMetaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserTagMeta','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserTagMeta','2.2.0')
 		self.set_method('POST')
 
 	def get_TagDescription(self): # String
 		return self.get_query_params().get('TagDescription')
 
 	def set_TagDescription(self, TagDescription):  # String
 		self.add_query_param('TagDescription', TagDescription)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddUserToWorkspaceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AddUserToWorkspaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserToWorkspace','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddUserToWorkspace','2.2.0')
 		self.set_method('POST')
 
 	def get_RoleId(self): # Long
 		return self.get_query_params().get('RoleId')
 
 	def set_RoleId(self, RoleId):  # Long
 		self.add_query_param('RoleId', RoleId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class AddWorkspaceUsersRequest(RpcRequest):
+class UpdateWorkspaceUsersRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddWorkspaceUsers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateWorkspaceUsersRole','2.2.0')
 		self.set_method('POST')
 
 	def get_UserIds(self): # String
 		return self.get_query_params().get('UserIds')
 
 	def set_UserIds(self, UserIds):  # String
 		self.add_query_param('UserIds', UserIds)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AuthorizeMenuRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class AuthorizeMenuRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AuthorizeMenu','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AuthorizeMenu','2.2.0')
 		self.set_method('POST')
 
 	def get_DataPortalId(self): # String
 		return self.get_query_params().get('DataPortalId')
 
 	def set_DataPortalId(self, DataPortalId):  # String
 		self.add_query_param('DataPortalId', DataPortalId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/BatchAddFeishuUsersRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class BatchAddFeishuUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'BatchAddFeishuUsers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'BatchAddFeishuUsers','2.2.0')
 		self.set_method('POST')
 
 	def get_IsAdmin(self): # Boolean
 		return self.get_query_params().get('IsAdmin')
 
 	def set_IsAdmin(self, IsAdmin):  # Boolean
 		self.add_query_param('IsAdmin', IsAdmin)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelAuthorizationMenuRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class CancelAuthorizationMenuRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelAuthorizationMenu','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelAuthorizationMenu','2.2.0')
 		self.set_method('POST')
 
 	def get_DataPortalId(self): # String
 		return self.get_query_params().get('DataPortalId')
 
 	def set_DataPortalId(self, DataPortalId):  # String
 		self.add_query_param('DataPortalId', DataPortalId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class CancelCollectionRequest(RpcRequest):
+class CheckReadableRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelCollection','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CheckReadable','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelReportShareRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class CancelReportShareRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelReportShare','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelReportShare','2.2.0')
 		self.set_method('POST')
 
 	def get_ReportId(self): # String
 		return self.get_query_params().get('ReportId')
 
 	def set_ReportId(self, ReportId):  # String
 		self.add_query_param('ReportId', ReportId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ChangeVisibilityModelRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ChangeVisibilityModelRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ChangeVisibilityModel','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ChangeVisibilityModel','2.2.0')
 		self.set_method('POST')
 
 	def get_DataPortalId(self): # String
 		return self.get_query_params().get('DataPortalId')
 
 	def set_DataPortalId(self, DataPortalId):  # String
 		self.add_query_param('DataPortalId', DataPortalId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CheckReadableRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class CheckReadableRequest(RpcRequest):
+class SaveFavoritesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CheckReadable','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SaveFavorites','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateTicketRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class CreateTicketRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CreateTicket','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CreateTicket','2.2.0')
 		self.set_method('POST')
 
 	def get_ExpireTime(self): # Integer
 		return self.get_query_params().get('ExpireTime')
 
 	def set_ExpireTime(self, ExpireTime):  # Integer
 		self.add_query_param('ExpireTime', ExpireTime)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CreateUserGroupRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class CreateUserGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CreateUserGroup','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CreateUserGroup','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupId(self): # String
 		return self.get_query_params().get('UserGroupId')
 
 	def set_UserGroupId(self, UserGroupId):  # String
 		self.add_query_param('UserGroupId', UserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DelayTicketExpireTimeRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DelayTicketExpireTimeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DelayTicketExpireTime','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DelayTicketExpireTime','2.2.0')
 		self.set_method('POST')
 
 	def get_ExpireTime(self): # Integer
 		return self.get_query_params().get('ExpireTime')
 
 	def set_ExpireTime(self, ExpireTime):  # Integer
 		self.add_query_param('ExpireTime', ExpireTime)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelPermissionRuleUsersRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteDataLevelPermissionRuleUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteDataLevelPermissionRuleUsers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteDataLevelPermissionRuleUsers','2.2.0')
 		self.set_method('POST')
 
 	def get_DeleteUserModel(self): # String
 		return self.get_query_params().get('DeleteUserModel')
 
 	def set_DeleteUserModel(self, DeleteUserModel):  # String
 		self.add_query_param('DeleteUserModel', DeleteUserModel)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteDataLevelRuleConfigRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteDataLevelRuleConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteDataLevelRuleConfig','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteDataLevelRuleConfig','2.2.0')
 		self.set_method('POST')
 
 	def get_RuleId(self): # String
 		return self.get_query_params().get('RuleId')
 
 	def set_RuleId(self, RuleId):  # String
 		self.add_query_param('RuleId', RuleId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteTicketRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteTicketRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteTicket','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteTicket','2.2.0')
 		self.set_method('POST')
 
 	def get_Ticket(self): # String
 		return self.get_query_params().get('Ticket')
 
 	def set_Ticket(self, Ticket):  # String
 		self.add_query_param('Ticket', Ticket)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserFromWorkspaceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserFromWorkspaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserFromWorkspace','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserFromWorkspace','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMemberRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserGroupMemberRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroupMember','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroupMember','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupId(self): # String
 		return self.get_query_params().get('UserGroupId')
 
 	def set_UserGroupId(self, UserGroupId):  # String
 		self.add_query_param('UserGroupId', UserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupMembersRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserGroupMembersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroupMembers','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroupMembers','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupIds(self): # String
 		return self.get_query_params().get('UserGroupIds')
 
 	def set_UserGroupIds(self, UserGroupIds):  # String
 		self.add_query_param('UserGroupIds', UserGroupIds)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroup','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserGroup','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupId(self): # String
 		return self.get_query_params().get('UserGroupId')
 
 	def set_UserGroupId(self, UserGroupId):  # String
 		self.add_query_param('UserGroupId', UserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUser','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUser','2.2.0')
 		self.set_method('POST')
 
 	def get_TransferUserId(self): # String
 		return self.get_query_params().get('TransferUserId')
 
 	def set_TransferUserId(self, TransferUserId):  # String
 		self.add_query_param('TransferUserId', TransferUserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/DeleteUserTagMetaRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class DeleteUserTagMetaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserTagMeta','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'DeleteUserTagMeta','2.2.0')
 		self.set_method('POST')
 
 	def get_TagId(self): # String
 		return self.get_query_params().get('TagId')
 
 	def set_TagId(self, TagId):  # String
 		self.add_query_param('TagId', TagId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/GetUserGroupInfoRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class GetUserGroupInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'GetUserGroupInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'GetUserGroupInfo','2.2.0')
 		self.set_method('POST')
 
 	def get_Keyword(self): # String
 		return self.get_query_params().get('Keyword')
 
 	def set_Keyword(self, Keyword):  # String
 		self.add_query_param('Keyword', Keyword)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListByUserGroupIdRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListByUserGroupIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListByUserGroupId','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListByUserGroupId','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupIds(self): # String
 		return self.get_query_params().get('UserGroupIds')
 
 	def set_UserGroupIds(self, UserGroupIds):  # String
 		self.add_query_param('UserGroupIds', UserGroupIds)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCollectionsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListCollectionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListCollections','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListCollections','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListCubeDataLevelPermissionConfigRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListCubeDataLevelPermissionConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListCubeDataLevelPermissionConfig','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListCubeDataLevelPermissionConfig','2.2.0')
 		self.set_method('POST')
 
 	def get_RuleType(self): # String
 		return self.get_query_params().get('RuleType')
 
 	def set_RuleType(self, RuleType):  # String
 		self.add_query_param('RuleType', RuleType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListDataLevelPermissionWhiteListRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListDataLevelPermissionWhiteListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListDataLevelPermissionWhiteList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListDataLevelPermissionWhiteList','2.2.0')
 		self.set_method('POST')
 
 	def get_RuleType(self): # String
 		return self.get_query_params().get('RuleType')
 
 	def set_RuleType(self, RuleType):  # String
 		self.add_query_param('RuleType', RuleType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListFavoriteReportsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListFavoriteReportsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListFavoriteReports','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListFavoriteReports','2.2.0')
 		self.set_method('POST')
 
 	def get_TreeType(self): # String
 		return self.get_query_params().get('TreeType')
 
 	def set_TreeType(self, TreeType):  # String
 		self.add_query_param('TreeType', TreeType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenuAuthorizationRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListPortalMenuAuthorizationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListPortalMenuAuthorization','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListPortalMenuAuthorization','2.2.0')
 		self.set_method('POST')
 
 	def get_DataPortalId(self): # String
 		return self.get_query_params().get('DataPortalId')
 
 	def set_DataPortalId(self, DataPortalId):  # String
 		self.add_query_param('DataPortalId', DataPortalId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListPortalMenusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListPortalMenusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListPortalMenus','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListPortalMenus','2.2.0')
 		self.set_method('POST')
 
 	def get_DataPortalId(self): # String
 		return self.get_query_params().get('DataPortalId')
 
 	def set_DataPortalId(self, DataPortalId):  # String
 		self.add_query_param('DataPortalId', DataPortalId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListRecentViewReportsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListRecentViewReportsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListRecentViewReports','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListRecentViewReports','2.2.0')
 		self.set_method('POST')
 
 	def get_OffsetDay(self): # Integer
 		return self.get_query_params().get('OffsetDay')
 
 	def set_OffsetDay(self, OffsetDay):  # Integer
 		self.add_query_param('OffsetDay', OffsetDay)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListSharedReportsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListSharedReportsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListSharedReports','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListSharedReports','2.2.0')
 		self.set_method('POST')
 
 	def get_TreeType(self): # String
 		return self.get_query_params().get('TreeType')
 
 	def set_TreeType(self, TreeType):  # String
 		self.add_query_param('TreeType', TreeType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ListUserGroupsByUserIdRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ListUserGroupsByUserIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListUserGroupsByUserId','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ListUserGroupsByUserId','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDataServiceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryDataServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDataService','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDataService','2.2.0')
 		self.set_method('POST')
 
 	def get_ReturnFields(self): # String
 		return self.get_query_params().get('ReturnFields')
 
 	def set_ReturnFields(self, ReturnFields):  # String
 		self.add_query_param('ReturnFields', ReturnFields)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryDatasetDetailInfoRequest(RpcRequest):
+class QueryDatasetInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetDetailInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetInfo','2.2.0')
 		self.set_method('POST')
 
 	def get_DatasetId(self): # String
 		return self.get_query_params().get('DatasetId')
 
 	def set_DatasetId(self, DatasetId):  # String
 		self.add_query_param('DatasetId', DatasetId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetDetailInfoRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryDatasetInfoRequest(RpcRequest):
+class QueryDatasetDetailInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetDetailInfo','2.2.0')
 		self.set_method('POST')
 
 	def get_DatasetId(self): # String
 		return self.get_query_params().get('DatasetId')
 
 	def set_DatasetId(self, DatasetId):  # String
 		self.add_query_param('DatasetId', DatasetId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryDatasetListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetList','2.2.0')
 		self.set_method('POST')
 
 	def get_PageNum(self): # Integer
 		return self.get_query_params().get('PageNum')
 
 	def set_PageNum(self, PageNum):  # Integer
 		self.add_query_param('PageNum', PageNum)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryDatasetSwitchInfoRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryDatasetSwitchInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetSwitchInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryDatasetSwitchInfo','2.2.0')
 		self.set_method('POST')
 
 	def get_CubeId(self): # String
 		return self.get_query_params().get('CubeId')
 
 	def set_CubeId(self, CubeId):  # String
 		self.add_query_param('CubeId', CubeId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,13 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryEmbeddedInfoRequest(RpcRequest):
+class QueryTicketInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryEmbeddedInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryTicketInfo','2.2.0')
 		self.set_method('POST')
 
+	def get_Ticket(self): # String
+		return self.get_query_params().get('Ticket')
+
+	def set_Ticket(self, Ticket):  # String
+		self.add_query_param('Ticket', Ticket)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryEmbeddedStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryEmbeddedStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryEmbeddedStatus','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryEmbeddedStatus','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryOrganizationWorkspaceListRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryOrganizationWorkspaceListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryOrganizationWorkspaceList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryOrganizationWorkspaceList','2.2.0')
 		self.set_method('POST')
 
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryReadableResourcesListByUserIdRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryReadableResourcesListByUserIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryReadableResourcesListByUserId','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryReadableResourcesListByUserId','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryShareListRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryShareListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryShareList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryShareList','2.2.0')
 		self.set_method('POST')
 
 	def get_ReportId(self): # String
 		return self.get_query_params().get('ReportId')
 
 	def set_ReportId(self, ReportId):  # String
 		self.add_query_param('ReportId', ReportId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QuerySharesToUserListRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QuerySharesToUserListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QuerySharesToUserList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QuerySharesToUserList','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryTicketInfoRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryTicketInfoRequest(RpcRequest):
+class QueryWorksBloodRelationshipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryTicketInfo','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksBloodRelationship','2.2.0')
 		self.set_method('POST')
 
-	def get_Ticket(self): # String
-		return self.get_query_params().get('Ticket')
+	def get_WorksId(self): # String
+		return self.get_query_params().get('WorksId')
 
-	def set_Ticket(self, Ticket):  # String
-		self.add_query_param('Ticket', Ticket)
+	def set_WorksId(self, WorksId):  # String
+		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupListByParentIdRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserGroupListByParentIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserGroupListByParentId','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserGroupListByParentId','2.2.0')
 		self.set_method('POST')
 
 	def get_ParentUserGroupId(self): # String
 		return self.get_query_params().get('ParentUserGroupId')
 
 	def set_ParentUserGroupId(self, ParentUserGroupId):  # String
 		self.add_query_param('ParentUserGroupId', ParentUserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserGroupMemberRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserGroupMemberRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserGroupMember','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserGroupMember','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupId(self): # String
 		return self.get_query_params().get('UserGroupId')
 
 	def set_UserGroupId(self, UserGroupId):  # String
 		self.add_query_param('UserGroupId', UserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByAccountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserInfoByAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserInfoByAccount','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserInfoByAccount','2.2.0')
 		self.set_method('POST')
 
 	def get_Account(self): # String
 		return self.get_query_params().get('Account')
 
 	def set_Account(self, Account):  # String
 		self.add_query_param('Account', Account)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserInfoByUserIdRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserInfoByUserIdRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserInfoByUserId','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserInfoByUserId','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserList','2.2.0')
 		self.set_method('GET')
 
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserRoleInfoInWorkspaceRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserRoleInfoInWorkspaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserRoleInfoInWorkspace','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserRoleInfoInWorkspace','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagMetaListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserTagMetaListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserTagMetaList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserTagMetaList','2.2.0')
 		self.set_method('GET')
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryUserTagValueListRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryUserTagValueListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserTagValueList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryUserTagValueList','2.2.0')
 		self.set_method('GET')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksBloodRelationshipRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryWorksBloodRelationshipRequest(RpcRequest):
+class QueryWorksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksBloodRelationship','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorks','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByOrganizationRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryWorksByOrganizationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksByOrganization','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksByOrganization','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksType(self): # String
 		return self.get_query_params().get('WorksType')
 
 	def set_WorksType(self, WorksType):  # String
 		self.add_query_param('WorksType', WorksType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorksByWorkspaceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryWorksByWorkspaceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksByWorkspace','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorksByWorkspace','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksType(self): # String
 		return self.get_query_params().get('WorksType')
 
 	def set_WorksType(self, WorksType):  # String
 		self.add_query_param('WorksType', WorksType)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorksRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/CancelCollectionRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,18 +15,23 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class QueryWorksRequest(RpcRequest):
+class CancelCollectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorks','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'CancelCollection','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
+
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/QueryWorkspaceUserListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class QueryWorkspaceUserListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorkspaceUserList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'QueryWorkspaceUserList','2.2.0')
 		self.set_method('POST')
 
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ResultCallbackRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class ResultCallbackRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ResultCallback','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ResultCallback','2.2.0')
 		self.set_method('POST')
 
 	def get_HandleReason(self): # String
 		return self.get_query_params().get('HandleReason')
 
 	def set_HandleReason(self, HandleReason):  # String
 		self.add_query_param('HandleReason', HandleReason)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SaveFavoritesRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class SaveFavoritesRequest(RpcRequest):
+class UpdateUserTagValueRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SaveFavorites','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserTagValue','2.2.0')
 		self.set_method('POST')
 
-	def get_WorksId(self): # String
-		return self.get_query_params().get('WorksId')
+	def get_TagValue(self): # String
+		return self.get_query_params().get('TagValue')
 
-	def set_WorksId(self, WorksId):  # String
-		self.add_query_param('WorksId', WorksId)
+	def set_TagValue(self, TagValue):  # String
+		self.add_query_param('TagValue', TagValue)
+	def get_TagId(self): # String
+		return self.get_query_params().get('TagId')
+
+	def set_TagId(self, TagId):  # String
+		self.add_query_param('TagId', TagId)
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionExtraConfigRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class SetDataLevelPermissionExtraConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionExtraConfig','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionExtraConfig','2.2.0')
 		self.set_method('POST')
 
 	def get_MissHitPolicy(self): # String
 		return self.get_query_params().get('MissHitPolicy')
 
 	def set_MissHitPolicy(self, MissHitPolicy):  # String
 		self.add_query_param('MissHitPolicy', MissHitPolicy)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionRuleConfigRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class SetDataLevelPermissionRuleConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionRuleConfig','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionRuleConfig','2.2.0')
 		self.set_method('POST')
 
 	def get_RuleModel(self): # String
 		return self.get_query_params().get('RuleModel')
 
 	def set_RuleModel(self, RuleModel):  # String
 		self.add_query_param('RuleModel', RuleModel)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/SetDataLevelPermissionWhiteListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class SetDataLevelPermissionWhiteListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionWhiteList','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'SetDataLevelPermissionWhiteList','2.2.0')
 		self.set_method('POST')
 
 	def get_WhiteListModel(self): # String
 		return self.get_query_params().get('WhiteListModel')
 
 	def set_WhiteListModel(self, WhiteListModel):  # String
 		self.add_query_param('WhiteListModel', WhiteListModel)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateDataLevelPermissionStatusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateDataLevelPermissionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateDataLevelPermissionStatus','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateDataLevelPermissionStatus','2.2.0')
 		self.set_method('POST')
 
 	def get_IsOpen(self): # Integer
 		return self.get_query_params().get('IsOpen')
 
 	def set_IsOpen(self, IsOpen):  # Integer
 		self.add_query_param('IsOpen', IsOpen)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateEmbeddedStatusRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateEmbeddedStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateEmbeddedStatus','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateEmbeddedStatus','2.2.0')
 		self.set_method('POST')
 
 	def get_WorksId(self): # String
 		return self.get_query_params().get('WorksId')
 
 	def set_WorksId(self, WorksId):  # String
 		self.add_query_param('WorksId', WorksId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateTicketNumRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateTicketNumRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateTicketNum','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateTicketNum','2.2.0')
 		self.set_method('POST')
 
 	def get_Ticket(self): # String
 		return self.get_query_params().get('Ticket')
 
 	def set_Ticket(self, Ticket):  # String
 		self.add_query_param('Ticket', Ticket)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateUserGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserGroup','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserGroup','2.2.0')
 		self.set_method('POST')
 
 	def get_UserGroupId(self): # String
 		return self.get_query_params().get('UserGroupId')
 
 	def set_UserGroupId(self, UserGroupId):  # String
 		self.add_query_param('UserGroupId', UserGroupId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUser','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUser','2.2.0')
 		self.set_method('POST')
 
 	def get_AdminUser(self): # Boolean
 		return self.get_query_params().get('AdminUser')
 
 	def set_AdminUser(self, AdminUser):  # Boolean
 		self.add_query_param('AdminUser', AdminUser)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagMetaRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class UpdateUserTagMetaRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserTagMeta','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserTagMeta','2.2.0')
 		self.set_method('POST')
 
 	def get_TagDescription(self): # String
 		return self.get_query_params().get('TagDescription')
 
 	def set_TagDescription(self, TagDescription):  # String
 		self.add_query_param('TagDescription', TagDescription)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateUserTagValueRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class UpdateUserTagValueRequest(RpcRequest):
+class UpdateWorkspaceUserRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateUserTagValue','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateWorkspaceUserRole','2.2.0')
 		self.set_method('POST')
 
-	def get_TagValue(self): # String
-		return self.get_query_params().get('TagValue')
+	def get_RoleId(self): # Long
+		return self.get_query_params().get('RoleId')
 
-	def set_TagValue(self, TagValue):  # String
-		self.add_query_param('TagValue', TagValue)
-	def get_TagId(self): # String
-		return self.get_query_params().get('TagId')
-
-	def set_TagId(self, TagId):  # String
-		self.add_query_param('TagId', TagId)
+	def set_RoleId(self, RoleId):  # Long
+		self.add_query_param('RoleId', RoleId)
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
+	def get_WorkspaceId(self): # String
+		return self.get_query_params().get('WorkspaceId')
+
+	def set_WorkspaceId(self, WorkspaceId):  # String
+		self.add_query_param('WorkspaceId', WorkspaceId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUserRoleRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/AddWorkspaceUsersRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class UpdateWorkspaceUserRoleRequest(RpcRequest):
+class AddWorkspaceUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateWorkspaceUserRole','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'AddWorkspaceUsers','2.2.0')
 		self.set_method('POST')
 
+	def get_UserIds(self): # String
+		return self.get_query_params().get('UserIds')
+
+	def set_UserIds(self, UserIds):  # String
+		self.add_query_param('UserIds', UserIds)
 	def get_RoleId(self): # Long
 		return self.get_query_params().get('RoleId')
 
 	def set_RoleId(self, RoleId):  # Long
 		self.add_query_param('RoleId', RoleId)
-	def get_UserId(self): # String
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self, UserId):  # String
-		self.add_query_param('UserId', UserId)
 	def get_WorkspaceId(self): # String
 		return self.get_query_params().get('WorkspaceId')
 
 	def set_WorkspaceId(self, WorkspaceId):  # String
 		self.add_query_param('WorkspaceId', WorkspaceId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/UpdateWorkspaceUsersRoleRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/ModifyApiDatasourceParametersRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class UpdateWorkspaceUsersRoleRequest(RpcRequest):
+class ModifyApiDatasourceParametersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'UpdateWorkspaceUsersRole','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'ModifyApiDatasourceParameters','2.2.0')
 		self.set_method('POST')
 
-	def get_UserIds(self): # String
-		return self.get_query_params().get('UserIds')
+	def get_Parameters(self): # String
+		return self.get_query_params().get('Parameters')
 
-	def set_UserIds(self, UserIds):  # String
-		self.add_query_param('UserIds', UserIds)
-	def get_RoleId(self): # Long
-		return self.get_query_params().get('RoleId')
+	def set_Parameters(self, Parameters):  # String
+		self.add_query_param('Parameters', Parameters)
+	def get_ApiId(self): # String
+		return self.get_query_params().get('ApiId')
 
-	def set_RoleId(self, RoleId):  # Long
-		self.add_query_param('RoleId', RoleId)
+	def set_ApiId(self, ApiId):  # String
+		self.add_query_param('ApiId', ApiId)
 	def get_WorkspaceId(self): # String
 		return self.get_query_params().get('WorkspaceId')
 
 	def set_WorkspaceId(self, WorkspaceId):  # String
 		self.add_query_param('WorkspaceId', WorkspaceId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py` & `aliyun-python-sdk-quickbi-public-2.1.2/aliyunsdkquickbi_public/request/v20220101/WithdrawAllUserGroupsRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
 class WithdrawAllUserGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'WithdrawAllUserGroups','quickbi')
+		RpcRequest.__init__(self, 'quickbi-public', '2022-01-01', 'WithdrawAllUserGroups','2.2.0')
 		self.set_method('POST')
 
 	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # String
 		self.add_query_param('UserId', UserId)
```

### Comparing `aliyun-python-sdk-quickbi-public-2.1.1/setup.py` & `aliyun-python-sdk-quickbi-public-2.1.2/setup.py`

 * *Files identical despite different names*

