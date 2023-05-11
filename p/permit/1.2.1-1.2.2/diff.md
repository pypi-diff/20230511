# Comparing `tmp/permit-1.2.1.tar.gz` & `tmp/permit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-1.2.1.tar", last modified: Tue Apr  4 21:11:39 2023, max compression
+gzip compressed data, was "permit-1.2.2.tar", last modified: Thu May 11 14:38:10 2023, max compression
```

## Comparing `permit-1.2.1.tar` & `permit-1.2.2.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.841758 permit-1.2.1/
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-1.2.1/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      453 2023-04-04 21:11:39.841606 permit-1.2.1/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     7297 2022-10-01 21:14:31.000000 permit-1.2.1/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.821953 permit-1.2.1/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:14:31.000000 permit-1.2.1/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.822708 permit-1.2.1/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    15305 2023-04-04 20:50:12.000000 permit-1.2.1/permit/api/client.py
--rw-r--r--   0 asafc      (501) staff       (20)     7362 2023-02-28 20:11:32.000000 permit-1.2.1/permit/api/client_sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.822800 permit-1.2.1/permit/cache/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/cache/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2884 2023-04-04 20:50:12.000000 permit-1.2.1/permit/client.py
--rw-r--r--   0 asafc      (501) staff       (20)     2170 2023-04-04 20:50:12.000000 permit-1.2.1/permit/config.py
--rw-r--r--   0 asafc      (501) staff       (20)       42 2023-04-04 20:50:12.000000 permit-1.2.1/permit/constants.py
--rw-r--r--   0 asafc      (501) staff       (20)      866 2023-02-28 20:23:37.000000 permit-1.2.1/permit/elements.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.823202 permit-1.2.1/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6798 2023-04-04 20:50:12.000000 permit-1.2.1/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-1.2.1/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     1495 2023-04-04 21:04:11.000000 permit-1.2.1/permit/exceptions.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.823323 permit-1.2.1/permit/instrument/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/instrument/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.823492 permit-1.2.1/permit/mutations/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/mutations/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    13857 2023-02-28 20:11:32.000000 permit-1.2.1/permit/mutations/client.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.823810 permit-1.2.1/permit/openapi/
--rw-r--r--   0 asafc      (501) staff       (20)      101 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.824004 permit-1.2.1/permit/openapi/api/
--rw-r--r--   0 asafc      (501) staff       (20)       47 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.824387 permit-1.2.1/permit/openapi/api/api_keys/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/api_keys/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      726 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/api_keys/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     2900 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/api_keys/get_api_key_scope.py
--rw-r--r--   0 asafc      (501) staff       (20)     5029 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/api_keys/get_environment_api_key.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.824564 permit-1.2.1/permit/openapi/api/authentication/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/authentication/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     3595 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/authentication/elements_login_as.py
--rw-r--r--   0 asafc      (501) staff       (20)      341 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/base.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.826169 permit-1.2.1/permit/openapi/api/environments/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/environments/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5109 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/environments/create_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     5105 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/environments/delete_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     5415 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/environments/get_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     6456 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/environments/list_environments.py
--rw-r--r--   0 asafc      (501) staff       (20)     5781 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/environments/update_environment.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.826826 permit-1.2.1/permit/openapi/api/opal_data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/opal_data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4979 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/opal_data/get_all_data.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/opal_data/get_data_for_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/opal_data/get_data_for_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5028 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/opal_data/get_pdp_info.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.827571 permit-1.2.1/permit/openapi/api/organizations/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/organizations/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4647 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/organizations/create_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     4437 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/organizations/delete_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     4932 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/organizations/get_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     5991 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/organizations/list_organizations.py
--rw-r--r--   0 asafc      (501) staff       (20)     5097 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/organizations/update_organization.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.828467 permit-1.2.1/permit/openapi/api/projects/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/projects/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4267 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/projects/create_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     4305 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/projects/delete_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     4547 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/projects/get_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     5658 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/projects/list_projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     4881 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/projects/update_project.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.829037 permit-1.2.1/permit/openapi/api/resource_actions/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/resource_actions/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7170 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_actions/create_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     7011 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_actions/delete_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     7069 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_actions/get_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     8107 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_actions/list_resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     8069 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_actions/update_resource_action.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.829613 permit-1.2.1/permit/openapi/api/resource_attributes/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/resource_attributes/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7433 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_attributes/create_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     7334 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_attributes/delete_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     7231 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_attributes/get_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     8173 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_attributes/list_resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     8428 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_attributes/update_resource_attribute.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.830583 permit-1.2.1/permit/openapi/api/resource_roles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/resource_roles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9926 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/add_parent_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7966 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/assign_permissions_to_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7588 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/create_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6901 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/delete_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6961 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/get_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8063 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/list_resource_roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     9533 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/remove_parent_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8017 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/remove_permissions_from_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8271 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resource_roles/update_resource_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.831241 permit-1.2.1/permit/openapi/api/resources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/resources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     8399 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/create_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     5917 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/delete_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     6068 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/get_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     8202 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/list_resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     8438 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/replace_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     6861 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/resources/update_resource.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.831649 permit-1.2.1/permit/openapi/api/role_assignments/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/role_assignments/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6767 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/role_assignments/assign_role.py
--rw-r--r--   0 asafc      (501) staff       (20)    11048 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/role_assignments/list_role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6772 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/role_assignments/unassign_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.832697 permit-1.2.1/permit/openapi/api/roles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/roles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     8630 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/add_parent_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6989 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/assign_permissions_to_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6371 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/create_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6013 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/delete_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     5880 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/get_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6999 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/list_roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     8237 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/remove_parent_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7040 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/remove_permissions_from_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7093 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/roles/update_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.833329 permit-1.2.1/permit/openapi/api/tenants/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/tenants/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6768 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/create_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     5842 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/delete_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     6023 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/get_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     8279 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/list_tenant_users.py
--rw-r--r--   0 asafc      (501) staff       (20)     7150 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/list_tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     6738 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/tenants/update_tenant.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.834160 permit-1.2.1/permit/openapi/api/users/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/users/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1371 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/api/users/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     7226 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/assign_role_to_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     7523 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/create_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5768 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/delete_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5905 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/get_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     7671 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/list_users.py
--rw-r--r--   0 asafc      (501) staff       (20)     7392 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/unassign_role_from_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     6573 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/api/users/update_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     1660 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/client.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.839900 permit-1.2.1/permit/openapi/models/
--rw-r--r--   0 asafc      (501) staff       (20)     3996 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      476 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/action_block_editable.py
--rw-r--r--   0 asafc      (501) staff       (20)      647 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/action_block_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      483 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/add_role_permissions.py
--rw-r--r--   0 asafc      (501) staff       (20)      230 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/api_key_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      691 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/api_key_scope_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      609 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/attribute_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      149 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/attribute_type.py
--rw-r--r--   0 asafc      (501) staff       (20)      635 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/environment_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1452 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/environment_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      671 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/environment_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      317 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/full_data.py
--rw-r--r--   0 asafc      (501) staff       (20)      255 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/http_validation_error.py
--rw-r--r--   0 asafc      (501) staff       (20)      684 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/organization_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1173 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/organization_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      706 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/organization_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      420 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/paginated_result_user_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      148 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/pdp_info_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      764 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/project_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1407 2023-02-28 20:24:10.000000 permit-1.2.1/permit/openapi/models/project_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      800 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/project_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      130 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/relations_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      469 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/remove_role_permissions.py
--rw-r--r--   0 asafc      (501) staff       (20)      651 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_action_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1949 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_action_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      457 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_action_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      849 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_attribute_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2224 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_attribute_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      635 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_attribute_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     2117 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     3074 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_read.py
--rw-r--r--   0 asafc      (501) staff       (20)     1895 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_replace.py
--rw-r--r--   0 asafc      (501) staff       (20)     1153 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2252 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_role_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      949 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_role_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     1930 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/resource_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      646 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_assignment_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1517 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_assignment_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      652 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_assignment_remove.py
--rw-r--r--   0 asafc      (501) staff       (20)      852 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_block.py
--rw-r--r--   0 asafc      (501) staff       (20)     1145 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      181 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/role_data.py
--rw-r--r--   0 asafc      (501) staff       (20)     2090 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      941 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/role_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      126 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/roles_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      832 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/tenant_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2072 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/tenant_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      655 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/tenant_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     1171 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/user_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      327 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/user_data.py
--rw-r--r--   0 asafc      (501) staff       (20)      369 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/user_login_request.py
--rw-r--r--   0 asafc      (501) staff       (20)      837 2023-02-28 20:23:01.000000 permit-1.2.1/permit/openapi/models/user_login_response.py
--rw-r--r--   0 asafc      (501) staff       (20)     1869 2023-04-04 20:50:12.000000 permit-1.2.1/permit/openapi/models/user_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      317 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/user_role.py
--rw-r--r--   0 asafc      (501) staff       (20)      470 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/user_role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      472 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/user_role_remove.py
--rw-r--r--   0 asafc      (501) staff       (20)      798 2023-02-28 20:21:17.000000 permit-1.2.1/permit/openapi/models/user_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      258 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/models/validation_error.py
--rw-r--r--   0 asafc      (501) staff       (20)      939 2023-02-28 20:11:32.000000 permit-1.2.1/permit/openapi/types.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.840319 permit-1.2.1/permit/resources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/resources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1014 2023-04-04 20:50:12.000000 permit-1.2.1/permit/resources/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     6402 2022-10-01 21:14:31.000000 permit-1.2.1/permit/resources/registry.py
--rw-r--r--   0 asafc      (501) staff       (20)     6398 2022-10-01 21:14:31.000000 permit-1.2.1/permit/resources/reporter.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2022-10-01 21:14:31.000000 permit-1.2.1/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.840709 permit-1.2.1/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      848 2022-10-01 21:14:31.000000 permit-1.2.1/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-1.2.1/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)      926 2023-02-28 20:11:32.000000 permit-1.2.1/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.822439 permit-1.2.1/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      453 2023-04-04 21:11:39.000000 permit-1.2.1/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     7955 2023-04-04 21:11:39.000000 permit-1.2.1/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-04-04 21:11:39.000000 permit-1.2.1/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       55 2023-04-04 21:11:39.000000 permit-1.2.1/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-04-04 21:11:39.000000 permit-1.2.1/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       55 2023-02-28 20:11:32.000000 permit-1.2.1/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-04-04 21:11:39.841797 permit-1.2.1/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      767 2023-04-04 21:04:18.000000 permit-1.2.1/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.841061 permit-1.2.1/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.1/tests/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-04-04 21:11:39.841421 permit-1.2.1/tests/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-02-28 20:11:32.000000 permit-1.2.1/tests/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2023-04-04 20:50:12.000000 permit-1.2.1/tests/api/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     8431 2023-04-04 20:50:12.000000 permit-1.2.1/tests/api/test_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     8489 2023-04-04 20:50:12.000000 permit-1.2.1/tests/api/test_client_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      532 2022-10-01 21:14:31.000000 permit-1.2.1/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     4429 2023-04-04 20:50:12.000000 permit-1.2.1/tests/test_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     4348 2023-04-04 20:50:12.000000 permit-1.2.1/tests/test_sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.039020 permit-1.2.2/
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-1.2.2/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      453 2023-05-11 14:38:10.038899 permit-1.2.2/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     7297 2022-10-01 21:14:31.000000 permit-1.2.2/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.021269 permit-1.2.2/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:14:31.000000 permit-1.2.2/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022236 permit-1.2.2/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    15873 2023-05-11 14:37:27.000000 permit-1.2.2/permit/api/client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7362 2023-05-11 14:06:27.000000 permit-1.2.2/permit/api/client_sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022336 permit-1.2.2/permit/cache/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/cache/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2884 2023-05-11 14:06:27.000000 permit-1.2.2/permit/client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2170 2023-05-11 14:06:27.000000 permit-1.2.2/permit/config.py
+-rw-r--r--   0 asafc      (501) staff       (20)       42 2023-04-04 20:50:12.000000 permit-1.2.2/permit/constants.py
+-rw-r--r--   0 asafc      (501) staff       (20)      866 2023-05-11 14:06:27.000000 permit-1.2.2/permit/elements.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022585 permit-1.2.2/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6798 2023-05-11 14:06:27.000000 permit-1.2.2/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-1.2.2/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1495 2023-05-11 14:06:31.000000 permit-1.2.2/permit/exceptions.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022677 permit-1.2.2/permit/instrument/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/instrument/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022851 permit-1.2.2/permit/mutations/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/mutations/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    13857 2023-05-11 14:06:27.000000 permit-1.2.2/permit/mutations/client.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023131 permit-1.2.2/permit/openapi/
+-rw-r--r--   0 asafc      (501) staff       (20)      101 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023330 permit-1.2.2/permit/openapi/api/
+-rw-r--r--   0 asafc      (501) staff       (20)       47 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023709 permit-1.2.2/permit/openapi/api/api_keys/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      726 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2900 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/get_api_key_scope.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5029 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/get_environment_api_key.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023876 permit-1.2.2/permit/openapi/api/authentication/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/authentication/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3595 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/authentication/elements_login_as.py
+-rw-r--r--   0 asafc      (501) staff       (20)      341 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/base.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.024464 permit-1.2.2/permit/openapi/api/environments/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5109 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/create_environment.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5105 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/delete_environment.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5415 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/get_environment.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6456 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/list_environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5781 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/update_environment.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.024917 permit-1.2.2/permit/openapi/api/opal_data/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4979 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_all_data.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_data_for_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_data_for_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5028 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_pdp_info.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.025494 permit-1.2.2/permit/openapi/api/organizations/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4647 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/create_organization.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4437 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/delete_organization.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4932 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/get_organization.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5991 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/list_organizations.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5097 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/update_organization.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.026045 permit-1.2.2/permit/openapi/api/projects/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4267 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/create_project.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4305 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/delete_project.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4547 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/get_project.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5658 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/list_projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4881 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/update_project.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.026587 permit-1.2.2/permit/openapi/api/resource_actions/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7170 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/create_resource_action.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7011 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/delete_resource_action.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7069 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/get_resource_action.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8107 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/list_resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8069 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/update_resource_action.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.027137 permit-1.2.2/permit/openapi/api/resource_attributes/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7433 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/create_resource_attribute.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7334 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/delete_resource_attribute.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7231 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/get_resource_attribute.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8173 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/list_resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8428 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/update_resource_attribute.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.028121 permit-1.2.2/permit/openapi/api/resource_roles/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9926 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/add_parent_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7966 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/assign_permissions_to_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7588 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/create_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6901 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/delete_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6961 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/get_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8063 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/list_resource_roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9533 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/remove_parent_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8017 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/remove_permissions_from_resource_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8271 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/update_resource_role.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.028754 permit-1.2.2/permit/openapi/api/resources/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8399 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/create_resource.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5917 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/delete_resource.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6068 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/get_resource.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8202 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/list_resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8438 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/replace_resource.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6861 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/update_resource.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.029120 permit-1.2.2/permit/openapi/api/role_assignments/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6767 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/assign_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)    11048 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/list_role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6772 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/unassign_role.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.030062 permit-1.2.2/permit/openapi/api/roles/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8630 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/add_parent_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6989 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/assign_permissions_to_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6371 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/create_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6013 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/delete_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5880 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/get_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6999 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/list_roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8237 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/remove_parent_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7040 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/remove_permissions_from_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7093 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/update_role.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.030768 permit-1.2.2/permit/openapi/api/tenants/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6768 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/create_tenant.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5842 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/delete_tenant.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6023 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/get_tenant.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8279 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/list_tenant_users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7150 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/list_tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6738 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/update_tenant.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.031677 permit-1.2.2/permit/openapi/api/users/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1371 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7226 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/assign_role_to_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7523 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/create_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5768 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/delete_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5905 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/get_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7671 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/list_users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7392 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/unassign_role_from_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6573 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/update_user.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1660 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/client.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037242 permit-1.2.2/permit/openapi/models/
+-rw-r--r--   0 asafc      (501) staff       (20)     3996 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      476 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/action_block_editable.py
+-rw-r--r--   0 asafc      (501) staff       (20)      647 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/action_block_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      483 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/add_role_permissions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      230 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/api_key_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      691 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/api_key_scope_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      609 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/attribute_block.py
+-rw-r--r--   0 asafc      (501) staff       (20)      149 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/attribute_type.py
+-rw-r--r--   0 asafc      (501) staff       (20)      635 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1452 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      671 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      317 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/full_data.py
+-rw-r--r--   0 asafc      (501) staff       (20)      255 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/http_validation_error.py
+-rw-r--r--   0 asafc      (501) staff       (20)      684 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1173 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      706 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      420 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/paginated_result_user_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      148 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/pdp_info_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      764 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1407 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      800 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      130 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/relations_block.py
+-rw-r--r--   0 asafc      (501) staff       (20)      469 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/remove_role_permissions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      651 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1949 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      457 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      849 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2224 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      635 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2117 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3074 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1895 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_replace.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1153 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2252 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      949 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1930 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      646 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1517 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      652 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_remove.py
+-rw-r--r--   0 asafc      (501) staff       (20)      852 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_block.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1145 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)      181 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_data.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2090 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      941 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      126 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/roles_block.py
+-rw-r--r--   0 asafc      (501) staff       (20)      832 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2072 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      655 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1171 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)      327 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_data.py
+-rw-r--r--   0 asafc      (501) staff       (20)      369 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_login_request.py
+-rw-r--r--   0 asafc      (501) staff       (20)      837 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_login_response.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1869 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_read.py
+-rw-r--r--   0 asafc      (501) staff       (20)      317 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role.py
+-rw-r--r--   0 asafc      (501) staff       (20)      470 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role_create.py
+-rw-r--r--   0 asafc      (501) staff       (20)      472 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role_remove.py
+-rw-r--r--   0 asafc      (501) staff       (20)      798 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_update.py
+-rw-r--r--   0 asafc      (501) staff       (20)      258 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/validation_error.py
+-rw-r--r--   0 asafc      (501) staff       (20)      939 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/types.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037605 permit-1.2.2/permit/resources/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1014 2023-04-04 20:50:12.000000 permit-1.2.2/permit/resources/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6402 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/registry.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6398 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/reporter.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2022-10-01 21:14:31.000000 permit-1.2.2/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037966 permit-1.2.2/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      848 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)      926 2023-05-11 14:06:27.000000 permit-1.2.2/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.021942 permit-1.2.2/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      453 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     7955 2023-05-11 14:38:10.000000 permit-1.2.2/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       55 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       55 2023-05-11 14:06:27.000000 permit-1.2.2/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-11 14:38:10.039055 permit-1.2.2/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      767 2023-05-11 14:37:27.000000 permit-1.2.2/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.038315 permit-1.2.2/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/tests/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.038733 permit-1.2.2/tests/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8431 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/test_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8489 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/test_client_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      532 2022-10-01 21:14:31.000000 permit-1.2.2/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4429 2023-05-11 14:06:27.000000 permit-1.2.2/tests/test_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4348 2023-05-11 14:06:27.000000 permit-1.2.2/tests/test_sync.py
```

### Comparing `permit-1.2.1/README.md` & `permit-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/__init__.py` & `permit-1.2.2/permit/__init__.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/api/client.py` & `permit-1.2.2/permit/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,39 +6,50 @@
 from uuid import UUID
 
 from loguru import logger
 from pydantic import BaseModel
 from typing_extensions import ParamSpec
 
 from permit.config import PermitConfig
-from permit.exceptions import raise_for_error, raise_for_error_by_action
+from permit.exceptions import (
+    PermitException,
+    raise_for_error,
+    raise_for_error_by_action,
+)
 from permit.openapi import AuthenticatedClient
 from permit.openapi.api.api_keys import get_api_key_scope
 from permit.openapi.api.authentication import elements_login_as
 from permit.openapi.api.resources import (
     create_resource,
     delete_resource,
     get_resource,
     update_resource,
 )
 from permit.openapi.api.role_assignments import (
     assign_role,
     list_role_assignments,
     unassign_role,
 )
-from permit.openapi.api.roles import create_role, delete_role, get_role, update_role
+from permit.openapi.api.roles import (
+    create_role,
+    delete_role,
+    get_role,
+    list_roles,
+    update_role,
+)
 from permit.openapi.api.tenants import (
     create_tenant,
     delete_tenant,
     get_tenant,
     list_tenants,
     update_tenant,
 )
 from permit.openapi.api.users import create_user, delete_user, get_user, update_user
 from permit.openapi.models import (
+    HTTPValidationError,
     ResourceCreate,
     ResourceRead,
     ResourceUpdate,
     RoleAssignmentCreate,
     RoleAssignmentRead,
     RoleAssignmentRemove,
     RoleCreate,
@@ -176,14 +187,27 @@
             self.scope.environment_id.hex,
             resource_key,
             client=self.client,
         )
         raise_for_error_by_action(resource, "resource", resource_key)
         return resource
 
+    @lazy_load_scope
+    async def list_roles(self, page: int = 1, per_page: int = 100) -> List[RoleRead]:
+        roles = await list_roles.asyncio(
+            self.scope.project_id.hex,
+            self.scope.environment_id.hex,
+            page=page,
+            per_page=per_page,
+            client=self.client,
+        )
+        if isinstance(roles, HTTPValidationError):
+            raise PermitException(f"list_roles failed: {roles.detail}")
+        return roles
+
     # endregion
     # region write api ---------------------------------------------------------------
 
     @lazy_load_scope
     async def sync_user(self, user: Union[UserCreate, dict]) -> UserRead:
         if isinstance(user, dict):
             key = user.pop("key", None)
```

### Comparing `permit-1.2.1/permit/api/client_sync.py` & `permit-1.2.2/permit/api/client_sync.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/client.py` & `permit-1.2.2/permit/client.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/config.py` & `permit-1.2.2/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/elements.py` & `permit-1.2.2/permit/elements.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/enforcement/enforcer.py` & `permit-1.2.2/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/enforcement/interfaces.py` & `permit-1.2.2/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/exceptions.py` & `permit-1.2.2/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/mutations/client.py` & `permit-1.2.2/permit/mutations/client.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/api_keys/api.py` & `permit-1.2.2/permit/openapi/api/api_keys/api.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/api_keys/get_api_key_scope.py` & `permit-1.2.2/permit/openapi/api/api_keys/get_api_key_scope.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/api_keys/get_environment_api_key.py` & `permit-1.2.2/permit/openapi/api/api_keys/get_environment_api_key.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/authentication/elements_login_as.py` & `permit-1.2.2/permit/openapi/api/authentication/elements_login_as.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/environments/create_environment.py` & `permit-1.2.2/permit/openapi/api/environments/create_environment.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/environments/delete_environment.py` & `permit-1.2.2/permit/openapi/api/environments/delete_environment.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/environments/get_environment.py` & `permit-1.2.2/permit/openapi/api/environments/get_environment.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/environments/list_environments.py` & `permit-1.2.2/permit/openapi/api/environments/list_environments.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/environments/update_environment.py` & `permit-1.2.2/permit/openapi/api/environments/update_environment.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/opal_data/get_all_data.py` & `permit-1.2.2/permit/openapi/api/opal_data/get_all_data.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/opal_data/get_data_for_role.py` & `permit-1.2.2/permit/openapi/api/opal_data/get_data_for_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/opal_data/get_data_for_user.py` & `permit-1.2.2/permit/openapi/api/opal_data/get_data_for_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/opal_data/get_pdp_info.py` & `permit-1.2.2/permit/openapi/api/opal_data/get_pdp_info.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/organizations/create_organization.py` & `permit-1.2.2/permit/openapi/api/organizations/create_organization.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/organizations/delete_organization.py` & `permit-1.2.2/permit/openapi/api/organizations/delete_organization.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/organizations/get_organization.py` & `permit-1.2.2/permit/openapi/api/organizations/get_organization.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/organizations/list_organizations.py` & `permit-1.2.2/permit/openapi/api/organizations/list_organizations.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/organizations/update_organization.py` & `permit-1.2.2/permit/openapi/api/organizations/update_organization.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/projects/create_project.py` & `permit-1.2.2/permit/openapi/api/projects/create_project.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/projects/delete_project.py` & `permit-1.2.2/permit/openapi/api/projects/delete_project.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/projects/get_project.py` & `permit-1.2.2/permit/openapi/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/projects/list_projects.py` & `permit-1.2.2/permit/openapi/api/projects/list_projects.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/projects/update_project.py` & `permit-1.2.2/permit/openapi/api/projects/update_project.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_actions/create_resource_action.py` & `permit-1.2.2/permit/openapi/api/resource_actions/create_resource_action.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_actions/delete_resource_action.py` & `permit-1.2.2/permit/openapi/api/resource_actions/delete_resource_action.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_actions/get_resource_action.py` & `permit-1.2.2/permit/openapi/api/resource_actions/get_resource_action.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_actions/list_resource_actions.py` & `permit-1.2.2/permit/openapi/api/resource_actions/list_resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_actions/update_resource_action.py` & `permit-1.2.2/permit/openapi/api/resource_actions/update_resource_action.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_attributes/create_resource_attribute.py` & `permit-1.2.2/permit/openapi/api/resource_attributes/create_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_attributes/delete_resource_attribute.py` & `permit-1.2.2/permit/openapi/api/resource_attributes/delete_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_attributes/get_resource_attribute.py` & `permit-1.2.2/permit/openapi/api/resource_attributes/get_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_attributes/list_resource_attributes.py` & `permit-1.2.2/permit/openapi/api/resource_attributes/list_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_attributes/update_resource_attribute.py` & `permit-1.2.2/permit/openapi/api/resource_attributes/update_resource_attribute.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/add_parent_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/add_parent_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/assign_permissions_to_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/assign_permissions_to_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/create_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/create_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/delete_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/delete_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/get_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/get_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/list_resource_roles.py` & `permit-1.2.2/permit/openapi/api/resource_roles/list_resource_roles.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/remove_parent_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/remove_parent_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/remove_permissions_from_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/remove_permissions_from_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resource_roles/update_resource_role.py` & `permit-1.2.2/permit/openapi/api/resource_roles/update_resource_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/create_resource.py` & `permit-1.2.2/permit/openapi/api/resources/create_resource.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/delete_resource.py` & `permit-1.2.2/permit/openapi/api/resources/delete_resource.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/get_resource.py` & `permit-1.2.2/permit/openapi/api/resources/get_resource.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/list_resources.py` & `permit-1.2.2/permit/openapi/api/resources/list_resources.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/replace_resource.py` & `permit-1.2.2/permit/openapi/api/resources/replace_resource.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/resources/update_resource.py` & `permit-1.2.2/permit/openapi/api/resources/update_resource.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/role_assignments/assign_role.py` & `permit-1.2.2/permit/openapi/api/role_assignments/assign_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/role_assignments/list_role_assignments.py` & `permit-1.2.2/permit/openapi/api/role_assignments/list_role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/role_assignments/unassign_role.py` & `permit-1.2.2/permit/openapi/api/role_assignments/unassign_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/add_parent_role.py` & `permit-1.2.2/permit/openapi/api/roles/add_parent_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/assign_permissions_to_role.py` & `permit-1.2.2/permit/openapi/api/roles/assign_permissions_to_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/create_role.py` & `permit-1.2.2/permit/openapi/api/roles/create_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/delete_role.py` & `permit-1.2.2/permit/openapi/api/roles/delete_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/get_role.py` & `permit-1.2.2/permit/openapi/api/roles/get_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/list_roles.py` & `permit-1.2.2/permit/openapi/api/roles/list_roles.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/remove_parent_role.py` & `permit-1.2.2/permit/openapi/api/roles/remove_parent_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/remove_permissions_from_role.py` & `permit-1.2.2/permit/openapi/api/roles/remove_permissions_from_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/roles/update_role.py` & `permit-1.2.2/permit/openapi/api/roles/update_role.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/create_tenant.py` & `permit-1.2.2/permit/openapi/api/tenants/create_tenant.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/delete_tenant.py` & `permit-1.2.2/permit/openapi/api/tenants/delete_tenant.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/get_tenant.py` & `permit-1.2.2/permit/openapi/api/tenants/get_tenant.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/list_tenant_users.py` & `permit-1.2.2/permit/openapi/api/tenants/list_tenant_users.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/list_tenants.py` & `permit-1.2.2/permit/openapi/api/tenants/list_tenants.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/tenants/update_tenant.py` & `permit-1.2.2/permit/openapi/api/tenants/update_tenant.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/api.py` & `permit-1.2.2/permit/openapi/api/users/api.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/assign_role_to_user.py` & `permit-1.2.2/permit/openapi/api/users/assign_role_to_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/create_user.py` & `permit-1.2.2/permit/openapi/api/users/create_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/delete_user.py` & `permit-1.2.2/permit/openapi/api/users/delete_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/get_user.py` & `permit-1.2.2/permit/openapi/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/list_users.py` & `permit-1.2.2/permit/openapi/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/unassign_role_from_user.py` & `permit-1.2.2/permit/openapi/api/users/unassign_role_from_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/api/users/update_user.py` & `permit-1.2.2/permit/openapi/api/users/update_user.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/client.py` & `permit-1.2.2/permit/openapi/client.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/__init__.py` & `permit-1.2.2/permit/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/action_block_read.py` & `permit-1.2.2/permit/openapi/models/action_block_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/api_key_scope_read.py` & `permit-1.2.2/permit/openapi/models/api_key_scope_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/attribute_block.py` & `permit-1.2.2/permit/openapi/models/attribute_block.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/environment_create.py` & `permit-1.2.2/permit/openapi/models/environment_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/environment_read.py` & `permit-1.2.2/permit/openapi/models/environment_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/environment_update.py` & `permit-1.2.2/permit/openapi/models/environment_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/organization_create.py` & `permit-1.2.2/permit/openapi/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/organization_read.py` & `permit-1.2.2/permit/openapi/models/organization_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/organization_update.py` & `permit-1.2.2/permit/openapi/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/project_create.py` & `permit-1.2.2/permit/openapi/models/project_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/project_read.py` & `permit-1.2.2/permit/openapi/models/project_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/project_update.py` & `permit-1.2.2/permit/openapi/models/project_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_action_create.py` & `permit-1.2.2/permit/openapi/models/resource_action_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_action_read.py` & `permit-1.2.2/permit/openapi/models/resource_action_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_attribute_create.py` & `permit-1.2.2/permit/openapi/models/resource_attribute_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_attribute_read.py` & `permit-1.2.2/permit/openapi/models/resource_attribute_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_attribute_update.py` & `permit-1.2.2/permit/openapi/models/resource_attribute_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_create.py` & `permit-1.2.2/permit/openapi/models/resource_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_read.py` & `permit-1.2.2/permit/openapi/models/resource_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_replace.py` & `permit-1.2.2/permit/openapi/models/resource_replace.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_role_create.py` & `permit-1.2.2/permit/openapi/models/resource_role_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_role_read.py` & `permit-1.2.2/permit/openapi/models/resource_role_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_role_update.py` & `permit-1.2.2/permit/openapi/models/resource_role_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/resource_update.py` & `permit-1.2.2/permit/openapi/models/resource_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_assignment_create.py` & `permit-1.2.2/permit/openapi/models/role_assignment_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_assignment_read.py` & `permit-1.2.2/permit/openapi/models/role_assignment_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_assignment_remove.py` & `permit-1.2.2/permit/openapi/models/role_assignment_remove.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_block.py` & `permit-1.2.2/permit/openapi/models/role_block.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_create.py` & `permit-1.2.2/permit/openapi/models/role_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_read.py` & `permit-1.2.2/permit/openapi/models/role_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/role_update.py` & `permit-1.2.2/permit/openapi/models/role_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/tenant_create.py` & `permit-1.2.2/permit/openapi/models/tenant_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/tenant_read.py` & `permit-1.2.2/permit/openapi/models/tenant_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/tenant_update.py` & `permit-1.2.2/permit/openapi/models/tenant_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/user_create.py` & `permit-1.2.2/permit/openapi/models/user_create.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/user_login_response.py` & `permit-1.2.2/permit/openapi/models/user_login_response.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/user_read.py` & `permit-1.2.2/permit/openapi/models/user_read.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/models/user_update.py` & `permit-1.2.2/permit/openapi/models/user_update.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/openapi/types.py` & `permit-1.2.2/permit/openapi/types.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/resources/interfaces.py` & `permit-1.2.2/permit/resources/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/resources/registry.py` & `permit-1.2.2/permit/resources/registry.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/resources/reporter.py` & `permit-1.2.2/permit/resources/reporter.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/sync.py` & `permit-1.2.2/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/utils/context.py` & `permit-1.2.2/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit/utils/sync.py` & `permit-1.2.2/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/permit.egg-info/SOURCES.txt` & `permit-1.2.2/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/setup.py` & `permit-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="1.2.1",
+    version="1.2.2",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     python_requires=">=3.7",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
     classifiers=[
```

### Comparing `permit-1.2.1/tests/api/conftest.py` & `permit-1.2.2/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/tests/api/test_client.py` & `permit-1.2.2/tests/api/test_client.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/tests/api/test_client_sync.py` & `permit-1.2.2/tests/api/test_client_sync.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/tests/conftest.py` & `permit-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/tests/test_client.py` & `permit-1.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.1/tests/test_sync.py` & `permit-1.2.2/tests/test_sync.py`

 * *Files identical despite different names*

