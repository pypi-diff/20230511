# Comparing `tmp/fastapi_all_out-0.2.8.tar.gz` & `tmp/fastapi_all_out-0.3.0.tar.gz`

## Comparing `fastapi_all_out-0.2.8.tar` & `fastapi_all_out-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/app.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    33315 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/lazy.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0    18042 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/conntection.py
+-rw-r--r--   0        0        0    34462 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/temp_code.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    24940 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/email_change.html
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.3.0/PKG-INFO
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/app.py` & `fastapi_all_out-0.3.0/fastapi_all_out/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             **kwargs
     ) -> None:
         kwargs.setdefault('swagger_ui_parameters', {"operationsSorter": "method", "docExpansion": "none"})
         exception_handlers = kwargs.get('exception_handlers', {})
         kwargs['exception_handlers'] = {**default_exception_handlers, **exception_handlers}
         if add_auth_dependency:
             dependencies = kwargs.get('dependencies', [])
-            kwargs['dependencies'] = [Depends(get_auth_backend().authenticate()), *dependencies]
+            kwargs['dependencies'] = [Depends(get_auth_backend().authenticate_dependency()), *dependencies]
         super().__init__(**kwargs)
 
         if db_config:
             match db_provider:
                 case MainDB.tortoise:
                     from fastapi_all_out.contrib.tortoise import conntection
                     db_on_start = conntection.on_start(config=db_config)
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.3.0/fastapi_all_out/code_responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,25 +104,34 @@
                 },
             }
         return responses
 
 
 class DefaultCodes(BaseCodes):
     OK = 200, 'ОК'
-    not_found = 404, 'Item not found :('
+    not_found = 404, 'Item not found.'
     fields_error = 400, 'Fix all fields errors.'
 
+    code_incorrect = 400, 'Code is incorrect.'
+    code_expired = 400, 'Code is expired.'
+
     activation_email = 201, 'We sent activation code to your email.\nCheck spam if you can`t find it.'
     activation_email_resend = 400, 'Your activation code is expired, we sent new one to your email.\n' \
                                    'Check spam if you can`t find it.'
     activation_email_check = 400, 'Check code on your email.\nCheck spam if you can`t find it.'
-
-    activation_email_code_incorrect = 400, 'Your activation code is incorrect :('
     already_active = 400, 'You are already active.\nTry to sign in.'
 
+    email_change_email = 200, 'We sent confirmation code to your email.\nCheck spam if you can`t find it.'
+    email_changed = 200, 'Email changed successfully'
+    email_new_is_old = 400, 'New email is equal to old one.'
+
+    password_changed = 200, 'Password changed successfully.'
+    password_reset = 200, 'Password reset successfully.'
+    password_reset_email = 200, 'We sent password change link to your email.\nCheck spam if you can`t find it.'
+
     invalid_token = 401, "Authorization token is incorrect"
     expired_token = 401, "Authorization is expired"
     not_authenticated = 401, "Not authenticated"
     permission_denied = 403, "Permission denied"
 
     @classmethod
     def auth_errors(cls) -> tuple:
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/lazy.py` & `fastapi_all_out-0.3.0/fastapi_all_out/lazy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from importlib import import_module
 from typing import Any, TYPE_CHECKING, Type, TypeVar
+from copy import deepcopy
 
-from pydantic.utils import import_string
+from pydantic.utils import import_string, deep_update
 
 from fastapi_all_out.settings import MainDB, BaseSettings,\
-    MAIN_DB, USER_MODEL, REPOSITORY, USER_REPOSITORY, USER_SERVICE, MAIL_SENDER, CODES, AUTH
+    MAIN_DB, USER_MODEL, REPOSITORY, USER_REPOSITORY, USER_SERVICE, MAIL_SETTINGS, CODES, AUTH
 
 if TYPE_CHECKING:
     from fastapi_all_out.code_responses import DefaultCodes
     from fastapi_all_out.routers.base_repository import BaseRepository
     from fastapi_all_out.auth.user_service import BaseUserService
-    from fastapi_all_out.mailing import MailSender
-    from fastapi_all_out.auth.base import AuthBackend
+    from fastapi_all_out.mailing import MailSender, MailSettingsType
+    from fastapi_all_out.auth.base import AuthBackend, BaseUser
 
 
 _T = TypeVar('_T')
 
 
 def get_settings(var: str, default: Any = '__undefined__') -> Any:
     settings = import_module('settings')
@@ -55,15 +56,15 @@
     return import_settings('CODES', CODES)
 
 
 def get_user_model_path() -> str:
     return get_settings('USER_MODEL', USER_MODEL)
 
 
-def get_user_model():
+def get_user_model() -> "BaseUser":
     return import_settings('USER_MODEL', USER_MODEL)
 
 
 def get_repository() -> Type["BaseRepository"]:
     main_db = get_main_db().value
     return import_settings('REPOSITORY', REPOSITORY.format(main_db.lower(), main_db.title()))
 
@@ -74,16 +75,23 @@
 
 
 def get_user_service() -> Type["BaseUserService"]:
     main_db = get_main_db().value
     return import_settings('USER_SERVICE', USER_SERVICE.format(main_db.lower(), main_db.title()))
 
 
+def get_mail_settings() -> "MailSettingsType":
+    mail_settings = get_settings('MAIL_SETTINGS', {})
+    if mail_settings:
+        mail_settings = deepcopy(mail_settings)
+    return deep_update(mail_settings, deepcopy(MAIL_SETTINGS))
+
+
 def get_mail_sender() -> "MailSender":
-    return import_settings('MAIL_SENDER', MAIL_SENDER)
+    return import_string(get_mail_settings()['sender'])
 
 
 AUTH_BACKEND = None
 
 
 def get_auth_backend() -> "AuthBackend":
     global AUTH_BACKEND
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/models.py` & `fastapi_all_out-0.3.0/fastapi_all_out/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/responses.py` & `fastapi_all_out-0.3.0/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/settings.py` & `fastapi_all_out-0.3.0/fastapi_all_out/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 
 from pydantic import BaseSettings as PydanticBaseSettings, DirectoryPath, AnyHttpUrl
 
 
 MODE = os.environ.get('MODE') or 'DEBUG'
@@ -34,15 +35,25 @@
 REPOSITORY = f'{lib}.contrib.{{}}.repository.{{}}Repository'
 USER_REPOSITORY = f'{lib}.contrib.{{}}.user_repository.{{}}UserRepository'
 USER_SERVICE = f'{lib}.contrib.{{}}.user_service.{{}}UserService'
 AUTH = {
     'strategy': (f'{lib}.auth.jwt.strategy.RS256JWTAuthStrategy', {'private_key': None, 'public_key': None}),
     'backend': (f'{lib}.auth.jwt.backend.JWTAuthBackend', {}),
 }
-MAIL_SENDER = f'{lib}.mailing.mail_sender'
+MAIL_SETTINGS = {
+    'sender': f'{lib}.mailing.mail_sender',
+    'endpoints': {
+        'activation': 'confirm',
+        'email_change': 'email_change',
+        'password_reset': 'password_reset',
+    },
+    'temp_code_duration': {
+        '_default': timedelta(hours=1),
+    }
+}
 CODES = f'{lib}.code_responses.DefaultCodes'
 
 
 try:
     from fastapi_mail import ConnectionConfig
 
     class MailingConfig(ConnectionConfig):
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/base.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 from abc import ABC, abstractmethod
-from datetime import datetime
-from typing import Callable, Coroutine, Any, Optional
+from datetime import datetime, timedelta
+from typing import Callable, Coroutine, Any, Optional, Protocol
 from uuid import UUID
 
 from fastapi import APIRouter
+
+from fastapi_all_out.enums import TempCodeTriggers
 from fastapi_all_out.lazy import get_codes
 
 
 Codes = get_codes()
 
 
 class AuthStrategy(ABC):
     authorize_response_model: Any
 
-    def authorize(self, user) -> Any: ...
+    def authorize(self, user: "BaseUser") -> Any: ...
 
 
 class AuthBackend(ABC):
 
     strategy: "AuthStrategy"
 
+    def authorize(self, user: "BaseUser") -> Any:
+        return self.strategy.authorize(user=user)
+
     @abstractmethod
-    def authorize(self, user: "BaseUser") -> Any: ...
+    def authenticate_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
+
+    @abstractmethod
+    def auth_required_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
-    def authenticate(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
+    def load_user_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
-    def auth_required(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
+    def load_user_optionally_dependency(self) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
     @abstractmethod
-    def with_permissions(self, *permissions: tuple[str, str]) -> Callable[[], Coroutine[Any, Any, None]]: ...
+    def with_permissions_dependency(self, *permissions: tuple[str, str]) -> Callable[[], Coroutine[Any, Any, None]]: ...
 
-    def create_router(
-            self,
-            add_login_route: bool = True,
-            add_logout_route: bool = True,
-            **kwargs
-    ) -> APIRouter:
+    def create_router(self, add_login_route: bool = True, add_logout_route: bool = True, **kwargs) -> APIRouter:
         kwargs.setdefault('prefix', '/auth/jwt')
         kwargs.setdefault('tags', ['auth'])
         router = APIRouter(**kwargs)
         if add_login_route:
             self.add_login_route(router)
         if add_logout_route:
             self.add_logout_route(router)
@@ -60,15 +63,14 @@
     username: Optional[str]
     email: Optional[str]
     password_hash: str
     password_change_dt: datetime
     password_salt: str
     is_superuser: bool
     is_active: bool
-    is_verified: bool
     created_at: datetime
     EMAIL_FIELD: str
     AUTH_FIELDS: tuple[str, ...]
 
     @property
     def is_authenticated(self) -> bool:
         raise NotImplementedError()
@@ -84,17 +86,19 @@
     def has_permissions(self, *permissions) -> tuple[str, str]:
         raise NotImplementedError()
 
 
 class SimpleUser(BaseUser):
     pk: Any
 
-    def __init__(self, pk: int | UUID | str, username: str):
+    def __init__(self, pk: int | UUID | str, username: str, **kwargs):
         self.pk = pk
         self.username = username
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
     @property
     def is_authenticated(self) -> bool:
         return True
 
     @property
     def display_name(self) -> str:
@@ -112,7 +116,20 @@
 
     @property
     def display_name(self) -> str:
         return ""
 
     def is_simple(self) -> bool:
         return True
+
+
+class TempCodeProto(Protocol):
+    code: str
+    expired_at: datetime
+    trigger: TempCodeTriggers
+    extras: Optional[dict[str, Any] | list[Any]]
+
+    @property
+    def duration(self) -> timedelta: ...
+
+    @property
+    def is_expired(self) -> bool: ...
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fastapi_all_out.pydantic import CamelModel, Password, Username, RelatedList, CamelModelORM
 from fastapi_all_out.models import max_len_of
 from fastapi_all_out.lazy import get_user_model, get_schema
 from fastapi_all_out.schemas import PermissionRead
 
 
 __all__ = [
-    "PasswordsPair", "BaseLoginPasswordSchema", "LoginPasswordSchema",
+    "PasswordsPair", "ChangePassword", "BaseLoginPasswordSchema", "LoginPasswordSchema",
     "UserRead", "UserMeRead", "UserEdit", "UserMeEdit", "UserCreate", "UserRegistration",
 ]
 
 UserModel = get_user_model()
 Username = get_schema(Username, field=True)
 Password = get_schema(Password, field=True)
 
@@ -107,7 +107,17 @@
     groups: list[int]
     is_superuser: Optional[bool]
     is_active: Optional[bool]
 
 
 class UserRegistration(PasswordsPair, UserWriteBase):
     pass
+
+
+class ChangePassword(PasswordsPair):
+    old_password: str
+
+    @validator('old_password')
+    def new_is_not_old(cls, v: str, values: dict[str, Any]):
+        if v == values.get('password'):
+            raise ValueError('newPasswordIsEqualToOld')
+        return v
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Callable, Coroutine, Any
+from warnings import warn
+from typing import Callable, Coroutine, Any, cast
 
 from fastapi import APIRouter, Request, BackgroundTasks, Response, Body, Depends
 from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
 
 from fastapi_all_out.lazy import get_schema, get_user_model, get_user_repository, get_user_service, get_codes,\
     get_settings_obj
 from fastapi_all_out.routers.exceptions import ItemNotFound
@@ -27,77 +28,113 @@
 )
 
 
 class JWTAuthBackend(AuthBackend):
 
     strategy: "JWTAuthStrategy"
     oauth: OAuth2PasswordBearer
-    _authenticate: Callable[[], Coroutine[Any, Any, None]]
-    _auth_required: Callable[[], Coroutine[Any, Any, None]]
+    _authenticate: Callable[[Request, str], Coroutine[Any, Any, None]]
+    _auth_required: Callable[[Request], Coroutine[Any, Any, None]]
+    _load_user: Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]
+    _load_user_optionally: Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]
 
     def __init__(self, strategy: "JWTAuthStrategy", oauth: OAuth2PasswordBearer = oauth2_default):
         assert isinstance(strategy, JWTAuthStrategy)
         self.strategy = strategy
         self.oauth = oauth
 
-    def authorize(self, user: BaseUser) -> Any:
-        return self.strategy.authorize(user)
-
-    def authenticate(self) -> Callable[[], Coroutine[Any, Any, None]]:
+    def authenticate_dependency(self) -> Callable[[Request, str], Coroutine[Any, Any, None]]:
         if not hasattr(self, '_authenticate'):
             oauth_schema = self.oauth
             authenticate_handler = self.strategy.authenticate
 
-            async def wrapper(request: Request, token: str = Depends(oauth_schema)) -> None:
+            async def authenticate(request: Request, token: str = Depends(oauth_schema)) -> None:
                 token_data = await authenticate_handler(token)
                 if token_data is None:
                     request.scope['auth'] = None
                     request.scope['user'] = UnauthenticatedUser()
                 else:
                     user = token_data.user
                     request.scope['auth'] = token_data
-                    request.scope['user'] = SimpleUser(pk=user.get_pk(), username=user.username)
+                    request.scope['user'] = SimpleUser(
+                        pk=user.get_pk(), username=user.username, **user.dict(exclude={'username'})
+                    )
 
-            self._authenticate = wrapper
+            self._authenticate = authenticate
 
         return self._authenticate
 
-    def auth_required(self) -> Callable[[], Coroutine[Any, Any, None]]:
+    def auth_required_dependency(self) -> Callable[[Request], Coroutine[Any, Any, None]]:
         if not hasattr(self, '_auth_required'):
-            async def wrapper(request: Request) -> None:
-                user: BaseUser = request.user
+            async def auth_required(request: Request) -> None:
+                user = cast(SimpleUser | UnauthenticatedUser, request.user)
                 if not user.is_authenticated:
                     raise Codes.not_authenticated.err()
 
-            self._auth_required = wrapper
+            self._auth_required = auth_required
         return self._auth_required
 
-    def with_permissions(self, *permissions: tuple[str, str]) -> Callable[[], Coroutine[Any, Any, None]]:
-        async def wrapper(
+    def load_user_dependency(self) -> Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]:
+        if not hasattr(self, '_load_user'):
+            async def load_user(
+                    request: Request,
+                    background_tasks: BackgroundTasks,
+                    response: Response,
+                    _=Depends(self.auth_required_dependency())
+            ) -> None:
+                user = cast(SimpleUser, request.user)
+                if user.is_simple:
+                    try:
+                        request.scope['user'] = await UserRepository(
+                            request=request, background_tasks=background_tasks, response=response
+                        ).get_one(user.pk)
+                    except ItemNotFound:
+                        raise Codes.not_authenticated.err()
+                else:
+                    warn('What matters? User must be simple there')
+
+            self._load_user = load_user
+        return self._load_user
+
+    def load_user_optionally_dependency(self) -> Callable[[Request], Coroutine[Any, Any, None]]:
+        if not hasattr(self, '_load_user_optionally'):
+            async def load_user_optionally(
+                    request: Request,
+                    background_tasks: BackgroundTasks,
+                    response: Response,
+            ):
+                user = cast(SimpleUser | UnauthenticatedUser, request.user)
+                if not user.is_authenticated:
+                    return
+                if user.is_simple:
+                    try:
+                        request.scope['user'] = await UserRepository(
+                            request=request, background_tasks=background_tasks, response=response
+                        ).get_one(user.pk)
+                    except ItemNotFound:
+                        return
+                else:
+                    warn('What matters? User must be simple there')
+
+            self._load_user_optionally = load_user_optionally
+        return self._load_user_optionally
+
+    def with_permissions_dependency(
+            self,
+            *permissions: tuple[str, str],
+    ) -> Callable[[Request, BackgroundTasks, Response], Coroutine[Any, Any, None]]:
+        async def with_permissions(
                 request: Request,
-                background_tasks: BackgroundTasks,
-                response: Response,
+                _=Depends(self.load_user_dependency())
         ) -> None:
-            user: BaseUser = request.user
-            if not user.is_authenticated:
-                raise Codes.not_authenticated.err()
-            if user.is_simple:
-                user: SimpleUser
-                try:
-                    user_db = await UserRepository(
-                        request=request, background_tasks=background_tasks, response=response
-                    ).get_one(user.pk)
-                    request.scope['user'] = user = user_db
-                except ItemNotFound:
-                    raise Codes.not_authenticated.err()
-
+            user = cast(BaseUser, request.user)
             if not (user.is_superuser or user.has_permissions(*permissions)):
                 raise Codes.permission_denied.err()
 
-        return wrapper
+        return with_permissions
 
     def create_router(self, add_refresh_route: bool = True, **kwargs) -> APIRouter:
         router = super().create_router(**kwargs)
         if add_refresh_route:
             self.add_refresh_route(router)
         return router
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/schemas.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/jwt/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.3.0/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/conntection.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/conntection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+from typing import Type, cast
+
 from tortoise import Tortoise, connections
 from tortoise.log import logger
 
+from fastapi_all_out.models import BaseModel
+
 
 async def connect_db(config: dict = None):
     await Tortoise.init(config=config)
     logger.info(f'Tortoise-ORM started, {connections._get_storage()}, {Tortoise.apps}')
 
 
 async def close_db_connection():
     await connections.close_all()
     logger.info("Tortoise-ORM shutdown")
 
 
 def on_start(config: dict = None):
-    async def wrapper():
+    async def tortoise_on_start():
         await connect_db(config)
         await check_permissions()
 
-    return wrapper
+    return tortoise_on_start
 
 
 on_shutdown = close_db_connection
 
 
 async def check_permissions():
     from .models import ContentType, Permission
     from aerich.models import Aerich
-    all_models = list(Tortoise.apps.get('models').values())
+    # The requirement is to use only the fastapi_all_our.contrib.tortoise.models.BaseModel, not tortoise.Model
+    all_models = cast(list[Type[BaseModel]], list(Tortoise.apps.get('models').values()))
     if ContentType not in all_models:
         return
     old_names = [ct.name async for ct in ContentType.all()]
     new_names = []
     for model in all_models:
         if model is not Aerich and model is not ContentType:
             model_name = model.__name__
@@ -47,16 +52,16 @@
 
     create_perms: list[Permission] = []
     delete_perm_ids: list[int] = []
     for ct in content_types:
         ContentType.instances_by_id[ct.id] = ct
         ContentType.instances_by_name[ct.name] = ct
 
-        model = Tortoise.apps['models'][ct.name]
-        need_perm_names: list[str] = ['get', 'create', 'edit', 'delete', *getattr(model, 'ADDITIONAL_PERMS', ())]
+        model: Type[BaseModel] = Tortoise.apps['models'][ct.name]  # type: ignore
+        need_perm_names: list[str] = [*model.BASE_PERMISSIONS, *model.EXTRA_PERMISSIONS]
         for perm in filter(lambda p: p.content_type_id == ct.id, permissions):
             if perm.name in need_perm_names:
                 need_perm_names.remove(perm.name)
             else:
                 delete_perm_ids.append(perm.id)
         if need_perm_names:
             create_perms.extend(Permission(content_type=ct, name=perm_name) for perm_name in need_perm_names)
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import warnings
 from collections import defaultdict
-from typing import Any, Optional, TypeVar, TYPE_CHECKING, Type
+from typing import Any, Optional, TypeVar, Type, Callable, Coroutine
 
 from tortoise.models import MetaInfo
 from tortoise.fields import ManyToManyRelation, Field, DatetimeField, TimeField
 from tortoise.queryset import QuerySet
 from tortoise.transactions import in_transaction
 
+from fastapi_all_out.lazy import get_auth_backend, get_settings
+from fastapi_all_out.routers.utils import SORT, FILTERS
 from fastapi_all_out.routers.base_repository import BaseRepository, PK, ModelPrefix, Updated
 from fastapi_all_out.routers.exceptions import ItemNotFound, ObjectErrors, FieldError, NotUnique, ListFieldError,\
     NotFoundFK, FieldRequired
 from .repository_meta import TortoiseRepositoryMeta
 from .models import BaseModel
 
-if TYPE_CHECKING:
-    from fastapi_all_out.routers.filters import BaseFilter
-
 
 DB_MODEL = TypeVar('DB_MODEL', bound=BaseModel)
+DEBUG = get_settings('DEBUG')
 
 
 class TortoiseRepository(BaseRepository[DB_MODEL], metaclass=TortoiseRepositoryMeta):
     opts: MetaInfo
     node_key = 'parent_id'
 
     select_related: tuple[str]
@@ -61,16 +62,16 @@
     def qs_prefetch_related(self) -> set[str]:
         return set()
 
     async def get_all(
             self,
             skip: Optional[int],
             limit: Optional[int],
-            sort: list[str],
-            filters: list["BaseFilter"],
+            sort: SORT,
+            filters: FILTERS,
     ) -> tuple[list[DB_MODEL], int]:
         query = self.get_queryset()
         for f in filters:
             query = f.filter(query)
         base_query = query
         if sort:
             query = query.order_by(*sort)
@@ -405,14 +406,20 @@
             instance: DB_MODEL,
             field_name: str,
             data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> Optional[DB_MODEL]:
         o2o_instance: Optional[DB_MODEL] = getattr(instance, field_name)
+        if isinstance(o2o_instance, QuerySet):
+            if DEBUG:
+                warnings.warn(f'{field_name} if not fetched at {instance}')
+            await instance.fetch_related(field_name)
+            o2o_instance: Optional[DB_MODEL] = getattr(instance, field_name)
+
         o2o_data = data.get(field_name)
         if o2o_data is None:
             if o2o_instance is not None:
                 await o2o_instance.delete()
             return None
         if o2o_instance is not None:
             await self.edit(
@@ -436,14 +443,20 @@
             instance: DB_MODEL,
             field_name: str,
             data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
     ) -> None:
         back_o2o_instance = getattr(instance, field_name)
+        if isinstance(back_o2o_instance, QuerySet):
+            if DEBUG:
+                warnings.warn(f'{field_name} if not fetched at {instance}')
+            await instance.fetch_related(field_name)
+            back_o2o_instance: Optional[DB_MODEL] = getattr(instance, field_name)
+
         back_o2o_data = data.get(field_name)
         back_o2o_field = instance._meta.fields_map[field_name]
         back_o2o_model: Type[DB_MODEL] = back_o2o_field.related_model
         back_o2o_source_field = back_o2o_model._meta \
             .fields_map[back_o2o_field.relation_source_field] \
             .reference.model_field_name
         if back_o2o_instance is not None:
@@ -805,14 +818,22 @@
             raise errors
 
     async def _check_unique_default(self, model: Type[DB_MODEL], field_name: str, value: Any) -> bool:
         if field_name in model.IEXACT_FIELDS:
             field_name = field_name + '__iexact'
         return not await model.filter(**{field_name: value}).exists()
 
+    def with_model_permissions(cls, *names: str) -> Callable[[...], Coroutine[Any, Any, None]]:
+        permissions: set[str] = set()
+        for name in names:
+            if not (name in cls.model.BASE_PERMISSIONS or name in cls.model.EXTRA_PERMISSIONS):
+                raise Exception(f'{cls.model} don`t have {name} permission')
+            permissions.add(name)
+        return get_auth_backend().with_permissions_dependency(*((cls.model.__name__, name) for name in permissions))
+
     @classmethod
     def _get_bfk_model(cls, model: Type[BaseModel], field_name: str) -> Type[BaseModel]:
         return model._meta.fields_map[field_name].related_model
 
     @classmethod
     def _get_pk_attr(cls, model: Type[BaseModel]) -> str:
         return model._meta.pk_attr
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/user_repository.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from typing import Type, Any
+from typing import Type, Any, TYPE_CHECKING
 
 from fastapi_all_out.lazy import get_user_model, get_user_service
+from fastapi_all_out.routers.base_repository import ModelPrefix
 from .repository import TortoiseRepository
 from .user_service import USER_MODEL
-from ...routers.base_repository import ModelPrefix
+
 
 UserService = get_user_service()
 
 
 class TortoiseUserRepository(TortoiseRepository[USER_MODEL]):
     model = get_user_model()
 
     pass_check_required: dict[str, set[str]] = {'': {'password_hash', 'password_change_dt', 'password_salt'}}
 
     async def handle_create_(
             self,
-            model: Type["USER_MODEL"],
+            model: Type[USER_MODEL],
             data: dict[str, Any],
             exclude: set[str],
             prefix: ModelPrefix,
             defaults: dict[str, Any] = None,
             commit: bool = True,
     ) -> USER_MODEL:
         password = data.pop('password')
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/user_service.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/user_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,57 @@
 from random import choices
 from string import hexdigits
-from typing import TypeVar, Type, Literal, Optional
+from typing import TypeVar, Type, Optional, cast, Any
 
 from tortoise import timezone
 
 from fastapi_all_out.auth.user_service import BaseUserService, UNUSED_PASSWORD_PREFIX
-from fastapi_all_out.lazy import get_user_model, get_mail_sender
+from fastapi_all_out.lazy import get_user_model
 from fastapi_all_out.enums import TempCodeTriggers
-from .models import UserWithPermissions, BaseTempCode, get_field_param, max_len_of
+from .models import TempCode, BaseUser, max_len_of, get_field_param
 
 
-USER_MODEL = TypeVar("USER_MODEL", bound=UserWithPermissions)
-UserModel: Type[UserWithPermissions] = get_user_model()
-mail_sender = get_mail_sender()
+USER_MODEL = TypeVar("USER_MODEL", bound=BaseUser)
+UserModel = cast(Type[BaseUser], get_user_model())
 
 
 class TortoiseUserService(BaseUserService[USER_MODEL]):
+    _temp_code_model: Type[TempCode]
 
     def set_password(self, password: Optional[str]) -> None:
         user = self.user
         user.password_change_dt = timezone.now()
         user.password_salt = ''.join(choices(hexdigits, k=max_len_of(UserModel)('password_salt')))
         if password:
             user.password_hash = self.get_password_hash(password)
         else:
             user.password_hash = UNUSED_PASSWORD_PREFIX + self.get_password_hash(''.join(choices(hexdigits, k=30)))
 
-    async def get_or_create_temp_code(self, trigger: TempCodeTriggers) -> tuple[BaseTempCode, bool]:
-        await self.user.fetch_related('temp_code')
-        temp_code = self.user.temp_code
-        created = False
-        if temp_code:
-            if trigger != temp_code.trigger:
-                await temp_code.update(trigger)
-                created = True
-        else:
-            temp_code = await get_field_param(UserModel, 'temp_code', 'related_model') \
-                .create(user=self.user, trigger=trigger)
-            created = True
-        return temp_code, created
-
-    async def update_or_create_temp_code(self, trigger: TempCodeTriggers) -> BaseTempCode:
-        temp_code, created = await self.get_or_create_temp_code(trigger)
-        if not created:
-            await temp_code.update(trigger)
-        return temp_code
-
-    async def send_activation_email(self) -> None:
-        temp_code = await self.update_or_create_temp_code(trigger=TempCodeTriggers.EmailActivation)
-        await mail_sender.activation_email(
-            to=self.user.email,
-            username=self.user.username,
-            uuid=self.user.uuid,
-            temp_code=temp_code.code,
-            duration=temp_code.DURATION_TEXT,
-        )
-
-    async def send_password_reset_email(self) -> None:
-        temp_code = await self.update_or_create_temp_code(trigger=TempCodeTriggers.PwdReset)
-        await mail_sender.password_reset_email(
-            to=self.user.email,
-            username=self.user.username,
-            uuid=self.user.uuid,
-            temp_code=temp_code.code,
-            duration=temp_code.DURATION_TEXT,
-        )
-
-    def check_temp_code_error(self, code: str, trigger: TempCodeTriggers) -> Literal['expired', 'incorrect'] | None:
-        tc = self.user.temp_code
-        if tc.expired:
-            return 'expired'
-        if not tc.correct(code, trigger):
-            return 'incorrect'
-
-    async def activate(self) -> None:
-        self.user.is_active = True
-        await self.user.temp_code.delete()
-        await self.user.save(force_update=True, update_fields=['is_active'])
+    async def update_password(self, password: str) -> None:
+        self.set_password(password)
+        await self.user.save(force_update=True, update_fields=['password_hash', 'password_change_dt', 'password_salt'])
+
+    @classmethod
+    def get_temp_code_model(cls) -> Type[TempCode]:
+        if not hasattr(cls, '_temp_code_model'):
+            cls._temp_code_model = get_field_param(UserModel, 'temp_code', 'related_model')
+        return cls._temp_code_model
+
+    async def create_temp_code(
+            self, trigger: TempCodeTriggers, extras: dict[str, Any] | list[Any] = None
+    ) -> TempCode:
+        return await self.get_temp_code_model().new(user=self.user, trigger=trigger, extras=extras)
+
+    async def get_temp_code(
+            self, trigger: TempCodeTriggers
+    ) -> Optional[TempCode]:
+        return await self.get_temp_code_model().get_or_none(user=self.user, trigger=trigger)
+
+    async def update_temp_code(
+            self, temp_code: TempCode, extras: dict[str, Any] | list[Any] = None
+    ) -> None:
+        await temp_code.update(extras=extras)
+
+    async def delete_temp_code(
+            self, temp_code: TempCode
+    ) -> None:
+        await temp_code.delete()
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/temp_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,67 @@
-import random
+from typing import Union, Callable, Optional, Any, Self
+from datetime import timedelta, datetime
 from string import ascii_uppercase, digits
-from typing import Literal, Optional, Union, Callable
-from datetime import datetime, timedelta
-from uuid import UUID, uuid4
+from random import choices
 
 from tortoise import fields, timezone
 
-from fastapi_all_out.lazy import get_user_model_path
 from fastapi_all_out.enums import TempCodeTriggers
-from . import BaseModel, PermissionMixin, max_len_of
+from fastapi_all_out.lazy import get_user_model_path, get_mail_settings
+from . import max_len_of
+from . import BaseModel, BaseUser
 
 
-USER_GET_BY_FIELDS = Literal['id', 'email', 'username', 'phone']
-
-
-class BaseUser(BaseModel):
-    id: int
-    uuid: UUID = fields.UUIDField(default=uuid4, unique=True)
-    username: Optional[str] = fields.CharField(max_length=40, unique=True, null=True)
-    email: Optional[str] = fields.CharField(max_length=256, unique=True, null=True)
-    AUTH_FIELDS = ('email', 'username')
-    IEXACT_FIELDS = ('email', 'username')
-    EMAIL_FIELD = 'email'
-
-    password_hash: str = fields.CharField(max_length=200)
-    password_change_dt: datetime = fields.DatetimeField()
-    password_salt: str = fields.CharField(max_length=50)
-
-    is_superuser: bool = fields.BooleanField(default=False)
-    is_active: bool = fields.BooleanField(default=True)
-    created_at: datetime = fields.DatetimeField(auto_now_add=True)
-
-    temp_code: Union["BaseTempCode", fields.BackwardOneToOneRelation["BaseTempCode"]]
+class TempCode(BaseModel):
+    id: int = fields.BigIntField(pk=True)
+    user: Union["BaseUser", fields.ForeignKeyRelation["BaseUser"]] = fields.ForeignKeyField(
+        get_user_model_path(), related_name='temp_code', on_delete=fields.CASCADE
+    )
+    code: str = fields.CharField(max_length=6)
+    expired_at: datetime = fields.DatetimeField()
+    trigger: TempCodeTriggers = fields.CharEnumField(TempCodeTriggers)
+    extras: Optional[dict[str, Any] | list[Any]] = fields.JSONField(null=True)
 
     class Meta:
         abstract = True
+        unique_together = ('user', 'trigger')
 
     @property
-    def is_authenticated(self) -> bool:
-        return True
-
-    @property
-    def display_name(self) -> str:
-        return self.username
+    def duration(self) -> timedelta:
+        return get_tempcode_durations(self.trigger)
 
     @property
-    def is_simple(self) -> bool:
-        return False
+    def is_expired(self) -> bool:
+        return timezone.now() > self.expired_at
 
+    @classmethod
+    async def new(
+            cls,
+            user: BaseUser,
+            trigger: TempCodeTriggers,
+            extras: Optional[dict[str, Any] | list[Any]] = None
+    ) -> Self:
+        return await cls.create(
+            user=user,
+            code=get_random_tempcode(max_len_of(cls)('code'))(),
+            expired_at=timezone.now() + get_tempcode_durations(trigger),
+            trigger=trigger,
+            extras=extras
+        )
 
-class UserWithPermissions(BaseUser, PermissionMixin):
-    class Meta:
-        abstract = True
+    async def update(self, extras: Optional[dict[str, Any] | list[Any]] = None):
+        self.code = get_random_tempcode(max_len_of(self.__class__)('code'))()
+        self.expired_at = timezone.now() + self.duration
+        if extras:
+            self.extras = extras
+        await self.save(force_update=True, update_fields=('code', 'expired_at', 'extras'))
 
 
 def get_random_tempcode(code_len: int) -> Callable[[], str]:
-    return lambda: ''.join(random.choices(ascii_uppercase + digits, k=code_len))
+    return lambda: ''.join(choices(ascii_uppercase + digits, k=code_len))
 
 
-class BaseTempCode(BaseModel):
-    id: int = fields.BigIntField(pk=True)
-    user: UserWithPermissions | fields.OneToOneRelation[UserWithPermissions] = fields.OneToOneField(
-        get_user_model_path(), related_name='temp_code', on_delete=fields.CASCADE
-    )
-    code: str = fields.CharField(max_length=6, default=get_random_tempcode(6))
-    dt: datetime = fields.DatetimeField(auto_now=True)
-    trigger: TempCodeTriggers = fields.CharEnumField(TempCodeTriggers)
-    DURATION = timedelta(hours=1)
-    DURATION_TEXT = '1 hour'
+durations = get_mail_settings()['temp_code_duration']
 
-    async def update(self, trigger: TempCodeTriggers):
-        self.code = get_random_tempcode(max_len_of(self.__class__)('code'))()
-        self.dt = timezone.now()
-        self.trigger = trigger
-        await self.save(force_update=True, update_fields=('code', 'dt', 'trigger'))
 
-    @property
-    def expired_at(self) -> datetime:
-        return self.dt + self.DURATION
-
-    @property
-    def expired(self) -> bool:
-        return self.expired_at < timezone.now()
-
-    def correct(self, code: str, trigger: TempCodeTriggers) -> bool:
-        return code == self.code and trigger == self.trigger
-
-    class Meta:
-        abstract = True
+def get_tempcode_durations(trigger: TempCodeTriggers) -> timedelta:
+    return durations.get(trigger) or durations['_default']
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.3.0/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/management/command.py` & `fastapi_all_out-0.3.0/fastapi_all_out/management/command.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/camel_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         fragments.append(temp[0] + ''.join(elem.title() for elem in temp[1:]))
     return '__'.join(fragments)
 
 
 try:
     import orjson
 
-    def dumps(v, *, default):
-        return orjson.dumps(v, default=default).decode()
+    def dumps(v, *, default, **kwargs):
+        return orjson.dumps(v, default=default, **kwargs).decode()
 
     loads = orjson.loads
 except ImportError:
     import json
     dumps = json.dumps
     loads = json.loads
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.3.0/fastapi_all_out/pydantic/fields/username.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/base_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import abstractmethod
 from typing import Type, Any, TypeVar, Generic, Optional, Callable, Coroutine, TypedDict
 from uuid import UUID
 
 from fastapi import Request, BackgroundTasks, Response
 
-from fastapi_all_out.lazy import get_auth_backend
-from .filters import BaseFilter
+from .utils import SORT, FILTERS
 
 
 SERVICE = TypeVar('SERVICE', bound="BaseCRUDService")
 PK = TypeVar('PK', int, UUID)
 DB_MODEL = TypeVar('DB_MODEL')
 
 
@@ -58,24 +57,29 @@
             return self.request.scope['route'].path
 
     @property
     def request_method(self) -> Optional[str]:
         if self.request:
             return self.request.method.upper()
 
+    @property
+    def current_route_name(self) -> Optional[str]:
+        if self.request:
+            return self.request.scope['route'].name
+
     @abstractmethod
     def get_queryset(self): ...
 
     @abstractmethod
     async def get_all(
             self,
             skip: Optional[int],
             limit: Optional[int],
-            sort: list[str],
-            filters: list[BaseFilter],
+            sort: SORT,
+            filters: FILTERS,
     ) -> tuple[list[DB_MODEL], int]: ...
 
     @abstractmethod
     async def get_many(self, item_ids: list[PK]) -> list[DB_MODEL]: ...
 
     @abstractmethod
     async def get_one(self, item_id: PK, *, field_name: str = 'pk') -> DB_MODEL: ...
@@ -122,16 +126,16 @@
     @abstractmethod
     async def delete_many(self, instances: list[PK]) -> int: ...
 
     @abstractmethod
     async def delete_one(self, instance: DB_MODEL) -> None: ...
 
     @classmethod
-    def with_model_permissions(cls, name: str) -> Callable[[...], Coroutine[Any, Any, None]]:
-        return get_auth_backend().with_permissions((cls.model.__name__, name))
+    @abstractmethod
+    def with_model_permissions(cls, *names: str) -> Callable[[...], Coroutine[Any, Any, None]]: ...
 
     @classmethod
     def with_create_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
         return cls.with_model_permissions('create')
 
     @classmethod
     def with_get_permissions(cls) -> Callable[[...], Coroutine[Any, Any, None]]:
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/crud_router.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,59 @@
 from collections.abc import Sequence
 from enum import Enum
-from typing import Callable, Any, Generic, TypeVar, Optional, Type
+from typing import Callable, Any, Generic, TypeVar, Optional, Type, Literal, TypedDict, Final, Union, List, Dict, Set
 
-from fastapi import Response, Request, APIRouter, Body, Path, Query, params, Depends, BackgroundTasks
+from fastapi import Response, Request, APIRouter, Body, Path, Query, Depends, BackgroundTasks
+from fastapi.datastructures import Default, DefaultPlaceholder
+from fastapi.encoders import SetIntStr, DictIntStrAny
 from fastapi.exceptions import RequestValidationError
+from fastapi.routing import APIRoute
+from fastapi.utils import generate_unique_id
 from pydantic.error_wrappers import ErrorWrapper
+from starlette.responses import JSONResponse
+from starlette.routing import BaseRoute
 
 from fastapi_all_out.code_responses import BaseCodes
 from fastapi_all_out.pydantic import CommaSeparatedOf, lower_camel, CamelModel
 from fastapi_all_out.lazy import get_codes, get_auth_backend
 from fastapi_all_out.responses import BgHTTPException
 from fastapi_all_out.routers import BaseRepository
 from .exceptions import ItemNotFound, ObjectErrors
 from .filters import BaseFilter
-from .utils import pagination_factory, PAGINATION, get_filters, sort_factory
+from .utils import \
+    pagination_factory, PAGINATION,\
+    filters_factory, FILTERS, \
+    sort_factory, SORT
 
 
-DISPLAY_FIELDS = tuple[str, ...]
-REPO = TypeVar('REPO', bound=BaseRepository)
-DEPENDENCIES = Optional[Sequence[params.Depends]]
-ROUTES_KWARGS = dict[str, bool | dict[str, Any]]
+CHECK_PERMS: Final[str] = 'check_perms'
+LOAD_USER: Final[str] = 'load_user'
+AUTH_REQUIRED: Final[str] = 'auth_required'
+LOAD_USER_OPTIONALLY: Final[str] = 'load_user_optionally'
+ACCESS_ALL: Final[str] = 'access_all'
+ACCESS = Literal['check_perms', 'load_user', 'auth_required', 'load_user_optionally', 'access_all']
 
+REPO = TypeVar('REPO', bound=BaseRepository)
+DEPENDENCIES = Optional[Sequence[Depends]]
+ROUTE_KWARGS = TypedDict('ROUTE_KWARGS', total=False, fields={
+    'dependencies': DEPENDENCIES,
+    'access': ACCESS
+})
+ROUTES_KWARGS = dict[str, ROUTE_KWARGS]
 Codes = get_codes()
 
 
 class CRUDRouter(Generic[REPO], APIRouter):
-    repo: Type[BaseRepository]
+    repo: Type[REPO]
     max_items_get_many_routes: Optional[int]
     max_items_delete_many_routes: Optional[int]
     filters: list[Type[BaseFilter]]
     available_sort: set[str]
     max_page_size: int | None
-    auto_routes_dependencies: DEPENDENCIES
+    tree_enabled: bool
 
     read_schema: Optional[Type[CamelModel]]
     read_many_schema: Optional[Type[CamelModel]]
     read_list_item_schema: Optional[Type[CamelModel]]
     create_schema: Optional[Type[CamelModel]]
     edit_schema: Optional[Type[CamelModel]]
 
@@ -51,17 +69,16 @@
             max_items_get_many: int = 100,
             max_items_delete_many: int = 100,
             prefix: str = None,
             tags: Optional[list[str | Enum]] = None,
             filters: list[Type[BaseFilter]] = None,
             available_sort: set[str] = None,
             max_page_size: int | None = 100,
-            auto_routes_dependencies: DEPENDENCIES = None,
             routes_kwargs: ROUTES_KWARGS = None,
-            add_tree_routes: bool = False,
+            tree_enabled: bool = False,
             read_only: bool = False,
             routes_only: set[str] = None,
             complete_auto_routes: bool = True,
             **kwargs,
     ) -> None:
         """
             :param max_items_get_many         отпределяет маскимальное количество записей, которые достаются по id
@@ -94,144 +111,325 @@
         self.read_list_item_schema = read_list_item_schema or self.read_many_schema
         self.create_schema = create_schema
         self.edit_schema = edit_schema
 
         self.max_items_get_many_routes = max_items_get_many
         self.max_items_delete_many_routes = max_items_delete_many
         self.read_only = read_only
+        self.tree_enabled = tree_enabled
 
-        self.auto_routes_dependencies = auto_routes_dependencies or []
         self.routes_kwargs = routes_kwargs or {}
 
         if routes_only:
             routes_names = routes_only
         else:
-            routes_names = self.default_routes_names()
-            if add_tree_routes:
-                routes_names = *routes_names, *self.tree_route_names()
-        self.routes_names = routes_names
+            routes_names = []
+            for rn in self.default_route_names():
+                if self.routes_kwargs.get(rn) is not False:
+                    routes_names.append(rn)
+        self.routes_names = tuple(routes_names)
 
         if filters is None:
             filters = []
         self.filters = filters
         self.available_sort = available_sort or self.repo.get_default_sort_fields()
         self.max_page_size = max_page_size
 
         if complete_auto_routes:
             self.complete_auto_routes()
 
     def complete_auto_routes(self) -> None:
         for route_name in self.routes_names:
-            route_data = self.routes_kwargs.get(route_name, True)
-            if route_data is False:
-                continue
-            self._register_route(route_name, (route_data if isinstance(route_data, dict) else {}))
+            getattr(self, f'_register_{route_name}')()
+
+    def get_dependencies(
+            self,
+            route_name: str,
+            access: str = ACCESS_ALL,
+            permissions: Sequence[str] = None,
+    ) -> DEPENDENCIES:
+        """
+        :param route_name: name of route (get_all, get_many, ..., create, delete_one, ...)
+        :param access: type of access.
+        :param permissions: names of permissions to check if access == 'check_perms.
+        :return: DEPENDENCIES
+        """
+        route_kwargs: ROUTE_KWARGS = {**self.routes_kwargs.get('_all', {}), **self.routes_kwargs.get(route_name, {})}
+        dependencies = route_kwargs.get('dependencies', ())
+        access = route_kwargs.get('access', access)
+        assert access in (CHECK_PERMS, LOAD_USER, LOAD_USER_OPTIONALLY, AUTH_REQUIRED, ACCESS_ALL)
+
+        if access == CHECK_PERMS:
+            if permissions:
+                check_perms_dep = Depends(self.repo.with_model_permissions(*permissions))
+            elif route_name in self.GET_names():
+                check_perms_dep = Depends(self.repo.with_model_permissions('get'))
+            elif route_name in self.CREATE_names():
+                check_perms_dep = Depends(self.repo.with_model_permissions('create'))
+            elif route_name in self.EDIT_names():
+                check_perms_dep = Depends(self.repo.with_model_permissions('edit'))
+            elif route_name in self.DELETE_names():
+                check_perms_dep = Depends(self.repo.with_model_permissions('delete'))
+            else:
+                raise Exception('If access is check_perms, permissions must be passed '
+                                'or route_name must be in GET_names, CREATE_names, EDIT_names or DELETE_names')
+            return *dependencies, check_perms_dep
+        elif access == LOAD_USER:
+            return *dependencies, Depends(get_auth_backend().load_user_dependency())
+        elif access == AUTH_REQUIRED:
+            return *dependencies, Depends(get_auth_backend().auth_required_dependency())
+        elif access == LOAD_USER_OPTIONALLY:
+            return *dependencies, Depends(get_auth_backend().load_user_optionally_dependency())
+        return *dependencies,
+
+    def get_read_schema(self) -> Type[CamelModel]:
+        return self.read_schema
+
+    def get_read_many_schema(self) -> Type[CamelModel]:
+        return self.read_many_schema
+
+    def get_read_list_item_schema(self) -> Type[CamelModel]:
+        return self.read_list_item_schema
+
+    def get_create_schema(self) -> Type[CamelModel]:
+        return self.create_schema
 
+    def get_edit_schema(self) -> Type[CamelModel]:
+        return self.edit_schema
+
+    def register_api_route(
+            self,
+            path: str,
+            endpoint: Callable[..., Any],
+            access: str = ACCESS_ALL,
+            permissions: Sequence[str] = None,
+            dependencies: DEPENDENCIES = None,
+
+            response_model: Any = Default(None),
+            status_code: Optional[int] = None,
+            tags: Optional[List[Union[str, Enum]]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            response_description: str = "Successful Response",
+            responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
+            deprecated: Optional[bool] = None,
+            methods: Optional[Union[Set[str], List[str]]] = None,
+            operation_id: Optional[str] = None,
+            response_model_include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+            response_model_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+            response_model_by_alias: bool = True,
+            response_model_exclude_unset: bool = False,
+            response_model_exclude_defaults: bool = False,
+            response_model_exclude_none: bool = False,
+            include_in_schema: bool = True,
+            response_class: Union[Type[Response], DefaultPlaceholder] = Default(JSONResponse),
+            name: Optional[str] = None,
+            route_class_override: Optional[Type[APIRoute]] = None,
+            callbacks: Optional[List[BaseRoute]] = None,
+            openapi_extra: Optional[Dict[str, Any]] = None,
+            generate_unique_id_function: Union[
+                Callable[[APIRoute], str], DefaultPlaceholder
+            ] = Default(generate_unique_id),
+    ) -> None:
+        name = name or endpoint.__name__
+        assert name in self.routes_names
+        self.add_api_route(
+            path,
+            endpoint,
+            dependencies=dependencies or self.get_dependencies(name, access, permissions=permissions),
+            response_model=response_model,
+            status_code=status_code,
+            tags=tags,
+            summary=summary,
+            description=description,
+            response_description=response_description,
+            responses=responses,
+            deprecated=deprecated,
+            methods=methods,
+            operation_id=operation_id,
+            response_model_include=response_model_include,
+            response_model_exclude=response_model_exclude,
+            response_model_by_alias=response_model_by_alias,
+            response_model_exclude_unset=response_model_exclude_unset,
+            response_model_exclude_defaults=response_model_exclude_defaults,
+            response_model_exclude_none=response_model_exclude_none,
+            include_in_schema=include_in_schema,
+            response_class=response_class,
+            name=name,
+            route_class_override=route_class_override,
+            callbacks=callbacks,
+            openapi_extra=openapi_extra,
+            generate_unique_id_function=generate_unique_id_function,
+        )
+
+    # get_all GET /all
     def _get_all_route(self) -> Callable[..., Any]:
         list_item_schema = self.get_read_list_item_schema()
 
-        async def route(
+        async def get_all(
                 background_tasks: BackgroundTasks,
                 request: Request,
                 response: Response,
                 pagination: PAGINATION = pagination_factory(self.max_page_size),
-                sort: list[str] = Depends(sort_factory(self.available_sort)),
-                applied_filters: list[BaseFilter] = Depends(get_filters(self.filters))
+                sort: SORT = Depends(sort_factory(self.available_sort)),
+                filters: FILTERS = Depends(filters_factory(self.filters))
         ):
-            raise_if_error_in_filters(applied_filters)
+            raise_if_error_in_filters(filters)
             skip, limit = pagination
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             result, total = await repository.get_all(
                 skip=skip,
                 limit=limit,
                 sort=sort,
-                filters=applied_filters,
+                filters=filters,
             )
             response.headers.append('X-Total-Count', str(total))
             return [list_item_schema.from_orm(r) for r in result]
 
-        return route
+        return get_all
 
+    def _register_get_all(self) -> None:
+        self.register_api_route(
+            path='/all',
+            endpoint=self._get_all_route(),
+            methods=["GET"],
+            response_model=list[self.get_read_list_item_schema()],
+            summary='Get all ' + self.repo.model.__name__,
+            status_code=200,
+            openapi_extra={'parameters': [f.query_openapi_desc() for f in self.filters]},
+            access=CHECK_PERMS,
+        )
+
+    # get_many GET /many
     def _get_many_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         max_items = self.max_items_get_many_routes
         read_many_schema = self.get_read_many_schema()
 
-        async def route(
+        async def get_many(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 item_ids: CommaSeparatedOf(pk_field_type, max_items=max_items, in_query=True) = Query(..., alias='ids')
         ):
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             results = await repository.get_many(item_ids)
             return [read_many_schema.from_orm(r) for r in results]
 
-        return route
+        return get_many
 
+    def _register_get_many(self) -> None:
+        self.register_api_route(
+            path='/many',
+            endpoint=self._get_many_route(),
+            methods=["GET"],
+            response_model=list[self.get_read_many_schema()],
+            summary='Get many ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS
+        )
+
+    # get_one GET /one/{item_id}
     def _get_one_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         read_schema = self.get_read_schema()
 
-        async def route(
+        async def get_one(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 item_id: pk_field_type = Path(...),
         ):
             try:
                 repository = self.repo(request=request, background_tasks=background_tasks, response=response)
                 item = await repository.get_one(item_id)
             except ItemNotFound:
                 raise self.not_found_error()
             return read_schema.from_orm(item)
 
-        return route
+        return get_one
+
+    def _register_get_one(self) -> None:
+        self.register_api_route(
+            path='/one/{item_id}',
+            endpoint=self._get_one_route(),
+            methods=["GET"],
+            response_model=self.get_read_schema(),
+            summary='Get one ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS,
+            responses=Codes.responses(self.not_found_error_instance()),
+        )
 
+    # get_tree_node GET /tree
     def _get_tree_node_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         get_list_item_schema = self.get_read_list_item_schema()
-        alias = lower_camel(self.repo.node_key)
 
-        async def route(
+        async def get_tree_node(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
-                node_id: Optional[pk_field_type] = Query(None, alias=alias)
+                node_id: Optional[pk_field_type] = Query(None, alias=lower_camel(self.repo.node_key))
         ):
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             return [get_list_item_schema.from_orm(item) for item in await repository.get_tree_node(node_id)]
 
-        return route
+        return get_tree_node
+
+    def _register_get_tree_node(self) -> None:
+        self.register_api_route(
+            path='/tree',
+            endpoint=self._get_tree_node_route(),
+            methods=["GET"],
+            response_model=list[self.get_read_list_item_schema()],
+            summary='Get tree node ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS
+        )
 
+    # create POST /create
     def _create_route(self) -> Callable[..., Any]:
         create_schema = self.get_create_schema()
         read_schema = self.get_read_schema()
 
-        async def route(
+        async def create(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 data: create_schema = Body(...)
         ):
             try:
                 instance = await self.repo(request=request, background_tasks=background_tasks, response=response)\
                     .create(data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise self.field_errors(e)
             return read_schema.from_orm(instance)
 
-        return route
+        return create
+
+    def _register_create(self) -> None:
+        self.register_api_route(
+            path='/create',
+            endpoint=self._create_route(),
+            methods=["POST"],
+            response_model=self.get_read_schema(),
+            summary='Create ' + self.repo.model.__name__,
+            status_code=201,
+            access=CHECK_PERMS,
+            responses=Codes.responses(self.field_errors_response_example()),
+        )
 
+    # edit PATCH /{item_id}
     def _edit_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         read_schema = self.get_read_schema()
         edit_schema = self.get_edit_schema()
 
-        async def route(
+        async def edit(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 item_id: pk_field_type = Path(...),
                 data: edit_schema = Body(...)
         ):
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
@@ -241,50 +439,89 @@
                 raise self.not_found_error()
             try:
                 instance = await repository.edit(instance, data.dict(exclude_unset=True))
             except ObjectErrors as e:
                 raise self.field_errors(e)
             return read_schema.from_orm(instance)
 
-        return route
+        return edit
+
+    def _register_edit(self) -> None:
+        self.register_api_route(
+            path='/{item_id}',
+            endpoint=self._edit_route(),
+            methods=["PATCH"],
+            response_model=self.get_read_schema(),
+            summary='Edit ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS,
+            responses=Codes.responses(
+                self.not_found_error_instance(),
+                self.field_errors_response_example()
+            )
+        )
 
+    # delete_many DELETE /many
     def _delete_many_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
         max_items = self.max_items_get_many_routes
 
-        async def route(
+        async def delete_many(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 item_ids: CommaSeparatedOf(pk_field_type, max_items=max_items, in_query=True) = Query(..., alias='ids')
         ):
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             deleted_items_count = await repository.delete_many(item_ids)
             return self.ok_response(count=deleted_items_count)
 
-        return route
+        return delete_many
+
+    def _register_delete_many(self) -> None:
+        self.register_api_route(
+            path='/many',
+            endpoint=self._delete_many_route(),
+            methods=["DELETE"],
+            summary='Delete many ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS,
+            responses=Codes.responses((self._ok_response_instance(), {'count': 30}), )
+        )
 
+    # delete_one DELETE /{item_id}
     def _delete_one_route(self) -> Callable[..., Any]:
         pk_field_type = self.repo.pk_field_type
 
-        async def route(
+        async def delete_one(
                 request: Request,
                 background_tasks: BackgroundTasks,
                 response: Response,
                 item_id: pk_field_type = Path(...)
         ):
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             try:
                 instance = await repository.get_one(item_id)
             except ItemNotFound:
                 raise self.not_found_error()
             await repository.delete_one(instance=instance)
             return self.ok_response(item=item_id)
 
-        return route
+        return delete_one
+
+    def _register_delete_one(self) -> None:
+        self.register_api_route(
+            path='/{item_id}',
+            endpoint=self._delete_one_route(),
+            methods=["DELETE"],
+            summary='Delete one ' + self.repo.model.__name__,
+            status_code=200,
+            access=CHECK_PERMS,
+            responses=Codes.responses((self._ok_response_instance(), {'item': 77}), )
+        )
 
     @classmethod
     def _ok_response_instance(cls) -> BaseCodes:
         return Codes.OK
 
     def ok_response(self, **kwargs) -> dict[str, Any]:
         if kwargs:
@@ -298,172 +535,41 @@
     def not_found_error(self) -> BgHTTPException:
         return self.not_found_error_instance().err()
 
     @classmethod
     def field_errors_instance(cls) -> BaseCodes:
         return Codes.fields_error
 
-    def field_errors_response_example(self) -> tuple[BaseCodes, dict[str, str]]:
+    def field_errors_response_example(self, example: dict[str, Any] = None) -> tuple[BaseCodes, dict[str, str]]:
         return (self.field_errors_instance(), {
-            'errors': 'Объект, который соответствует заполняемой модели, но вместо значений - ошибки'
+            'errors': example or 'Объект, который соответствует заполняемой модели, но вместо значений - ошибки'
         })
 
     def field_errors(self, object_errors: ObjectErrors) -> BgHTTPException:
         return self.field_errors_instance().err({'errors': object_errors.to_error()})
 
-    def default_routes_names(self) -> tuple[str, ...]:
+    def default_route_names(self) -> tuple[str, ...]:
         if self.read_only:
-            return 'get_all', 'get_many', 'get_one'
-        return 'get_all', 'get_many', 'get_one', 'create', 'edit', 'delete_many', 'delete_one'
+            return self.GET_names()
+        return *self.GET_names(), *self.CREATE_names(), *self.EDIT_names(), *self.DELETE_names(), *self.EXTRA_names()
 
-    @staticmethod
-    def tree_route_names() -> tuple[str, ...]:
-        return 'get_tree_node',
+    def GET_names(self) -> tuple[str, ...]:
+        names = 'get_all', 'get_many', 'get_one'
+        return (*names, 'get_tree_node') if self.tree_enabled else names
 
-    def all_route_names(self) -> tuple[str, ...]:
-        return *self.default_routes_names(), *self.tree_route_names()
+    def CREATE_names(self) -> tuple[str, ...]:
+        return 'create',
 
-    def _register_route(
-            self,
-            route_name: str,
-            route_kwargs: dict[str, Any],
-    ) -> None:
-        responses = {}
-        response_model = None
-        status = 200
-        openapi_extra = None
-        route_kwargs = {**self.routes_kwargs.get('all', {}), **route_kwargs}
-        match route_name:
-            case 'get_all':
-                path = '/all'
-                method = ["GET"]
-                response_model = list[self.get_read_list_item_schema()]
-                check_perms_dependency = Depends(self.repo.with_get_permissions())
-                openapi_extra = {'parameters': [f.query_openapi_desc() for f in self.filters]}
-            case 'get_many':
-                path = '/many'
-                method = ["GET"]
-                response_model = list[self.get_read_many_schema()]
-                check_perms_dependency = Depends(self.repo.with_get_permissions())
-            case 'get_one':
-                path = '/one/{item_id}'
-                method = ["GET"]
-                response_model = self.get_read_schema()
-                responses = Codes.responses(self.not_found_error_instance())
-                check_perms_dependency = Depends(self.repo.with_get_permissions())
-            case 'get_tree_node':
-                path = '/tree'
-                method = ["GET"]
-                response_model = list[self.get_read_list_item_schema()]
-                check_perms_dependency = Depends(self.repo.with_get_permissions())
-            case 'create':
-                path = '/create'
-                method = ["POST"]
-                response_model = self.get_read_schema()
-                responses = Codes.responses(self.field_errors_response_example())
-                status = 201
-                check_perms_dependency = Depends(self.repo.with_create_permissions())
-            case 'edit':
-                path = '/{item_id}'
-                method = ["PATCH"]
-                response_model = self.get_read_schema()
-                responses = Codes.responses(
-                    self.not_found_error_instance(),
-                    self.field_errors_response_example()
-                )
-                check_perms_dependency = Depends(self.repo.with_edit_permissions())
-            case 'delete_many':
-                path = '/many'
-                method = ["DELETE"]
-                # don`t need response model, responses has one with status 200
-                responses = Codes.responses((self._ok_response_instance(), {'count': 30}), )
-                check_perms_dependency = Depends(self.repo.with_delete_permissions())
-            case 'delete_one':
-                path = '/{item_id}'
-                method = ["DELETE"]
-                # don`t need response model, responses has one with status 200
-                responses = Codes.responses((self._ok_response_instance(), {'item': 77}), )
-                check_perms_dependency = Depends(self.repo.with_delete_permissions())
-            case _:
-                raise Exception(f'Unknown name of route: {route_name}.\n'
-                                f'Available are {", ".join(self.default_routes_names())}')
-        summary = f"{route_name.title().replace('_', ' ')} {self.repo.model.__name__}"
-
-        if route_kwargs.get('check_perms', True):
-            dependencies = [*self.auto_routes_dependencies, check_perms_dependency]
-        elif route_kwargs.get('auth_required', True):
-            dependencies = [*self.auto_routes_dependencies, Depends(get_auth_backend().auth_required())]
-        else:
-            dependencies = [*self.auto_routes_dependencies]
+    def EDIT_names(self) -> tuple[str, ...]:
+        return 'edit',
 
-        self.add_api_route(
-            path=path,
-            endpoint=getattr(self, f'_{route_name}_route')(),
-            methods=method,
-            response_model=response_model,
-            summary=summary,
-            status_code=status,
-            openapi_extra=openapi_extra,
-            **get_route_kwargs(route_kwargs, dependencies, responses),
-        )
+    def DELETE_names(self) -> tuple[str, ...]:
+        return 'delete_many', 'delete_one'
 
-    def get_read_schema(self) -> Type[CamelModel]:
-        return self.read_schema
-
-    def get_read_many_schema(self) -> Type[CamelModel]:
-        return self.read_many_schema
-
-    def get_read_list_item_schema(self) -> Type[CamelModel]:
-        return self.read_list_item_schema
-
-    def get_create_schema(self) -> Type[CamelModel]:
-        return self.create_schema
-
-    def get_edit_schema(self) -> Type[CamelModel]:
-        return self.edit_schema
-
-
-def get_route_kwargs(
-        route_data: dict[str, Any],
-        dependencies: DEPENDENCIES,
-        responses: dict[str, Any],
-) -> dict[str, Any]:
-    if isinstance(route_data, bool):
-        route_data = {}
-    else:
-        route_data = {**route_data}
-    route_data['dependencies'] = [*dependencies, *route_data.get('dependencies', [])] or None
-    route_data['responses'] = {**responses, **route_data.get('responses', {})} or None
-    for kwarg in tuple(route_data.keys()):
-        if kwarg not in available_api_route_kwargs:
-            del route_data[kwarg]
-    return route_data
+    def EXTRA_names(self) -> tuple[str, ...]:
+        return ()
 
 
 def raise_if_error_in_filters(filters: list[BaseFilter]) -> None:
     errors = [ErrorWrapper(f.error, loc=("filters", f.camel_source)) for f in filters if f.error is not None]
     if errors:
         raise RequestValidationError(errors)
-
-
-available_api_route_kwargs = [
-    'dependencies',
-    'responses',
-    'tags',
-    'description',
-    'response_description',
-    'deprecated',
-    'operation_id',
-    'response_model_include',
-    'response_model_exclude',
-    'response_model_by_alias',
-    'response_model_exclude_unset',
-    'response_model_exclude_defaults',
-    'response_model_exclude_none',
-    'include_in_schema',
-    'response_class',
-    'name',
-    'route_class_override',
-    'callbacks',
-    'openapi_extra',
-    'generate_unique_id_function',
-]
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     def to_error(self):
         return self.key
 
 
 NotUnique = AnyFieldError('not_unique')
 NotFoundFK = AnyFieldError('notFoundFK', False)
 FieldRequired = AnyFieldError('required_field')
+OldPasswordIsIncorrect = AnyFieldError('old_password_is_incorrect')
 
 
 class ListFieldError(FieldError):
     objects_map: dict[int, Union["ObjectErrors", "FieldError"]]
 
     def __init__(self,  *args):
         super().__init__(*args)
@@ -54,16 +55,17 @@
 
     def __str__(self):
         return str(self.to_error())
 
     def to_error(self):
         return {key: error.to_error() for key, error in self.errors.items()}
 
-    def add(self, field: str, error: Union[Type["FieldError"], "FieldError", "ObjectErrors"]):
+    def add(self, field: str, error: Union[Type["FieldError"], "FieldError", "ObjectErrors"]) -> Self:
         self.errors[field] = error
+        return self
 
     def merge(self, obj_error: "ObjectErrors") -> Self:
         self.errors.update(obj_error.errors)
         return self
 
     def __bool__(self):
         return not not self.errors
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,51 +7,53 @@
 
 if TYPE_CHECKING:
     from fastapi_all_out.routers.filters import BaseFilter
 
 
 ROUTE = bool | dict[str, Any]
 PAGINATION = tuple[Optional[int], Optional[int]]
+FILTERS = list["BaseFilter"]
+SORT = list[str]
 
 
 def pagination_factory(max_limit: Optional[int], default_limit: Optional[int] = 50) -> Any:
     """
-    Created the pagination dependency to be used in the router
+    Created the pagination dependency to be used in the CRUDRouter
     """
 
     if max_limit and default_limit > max_limit:
         default_limit = max_limit
 
     def pagination(
             skip: Optional[NonNegativeInt] = Query(None),
             limit: Optional[int] = Query(default_limit, ge=1, le=max_limit)
     ) -> PAGINATION:
         return skip, limit
 
     return Depends(pagination)
 
 
-def get_filters(filters: list[Type["BaseFilter"]]):
-    def wrapper(request: Request) -> list["BaseFilter"]:
+def filters_factory(available_filters: list[Type["BaseFilter"]]):
+    def filters(request: Request) -> FILTERS:
         qp = request.query_params
-        return [final_f for f in filters if (final_f := f.from_qs(qp))]
-    return wrapper
+        return [final_f for f in available_filters if (final_f := f.from_qs(qp))]
+    return filters
 
 
 def sort_factory(available: set[str]) -> Callable[[...], list[str]]:
     available_bidirectional: set[str] = set()
     for x in available:
         available_bidirectional.add(x)
         available_bidirectional.add('-' + x)
 
     def sort(fields: CommaSeparatedOf(str, wrapper=snake_case, in_query=True) = Query(
         None,
         alias='sort',
-        description=f'Пиши,поля,через,запятую. Доступно (+ эти же с минусами): {", ".join(available)}'
-    )) -> list[str]:
+        description=f'Write,fields,separated,by,commas. Available (also with "-" if descendant): {", ".join(available)}'
+    )) -> SORT:
         result: list[str] = []
         if fields:
             for field in fields:
                 if field in available_bidirectional:
                     result.append(field)
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.3.0/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.3.0/fastapi_all_out/templates/password_reset.html`

 * *Files 11% similar despite different names*

```diff
@@ -4,12 +4,12 @@
     <meta charset="UTF-8">
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <title>Goal2Be account activation</title>
 </head>
 <body>
-    <h1>Hello, {{ username }}</h1>
-    <h3>To activate your email enter this code <a href="{{ host }}/confirm?uuid={{ uuid }}&code={{ temp_code }}"><b>{{ temp_code }}</b></a></h3>
-    <p>Code is available in {{ duration }}</p>
+    <h1>Hello, {{ user.username }}</h1>
+    <h3>To reset your password tap <a href="{{ host }}/{{ endpoint }}?uuid={{ user.uuid }}&code={{ code }}"><b>this link</b></a></h3>
+    <p>Link is available in {{ duration_text }}</p>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 
 
-****** Hello, {{ username }} ******
-**** To activate your email enter this code {{_temp_code_}} ****
-Code is available in {{ duration }}
+****** Hello, {{ user.username }} ******
+**** To reset your password tap this_link ****
+Link is available in {{ duration_text }}
```

### Comparing `fastapi_all_out-0.2.8/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.3.0/fastapi_all_out/templates/activation.html`

 * *Files 27% similar despite different names*

```diff
@@ -4,12 +4,12 @@
     <meta charset="UTF-8">
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <title>Goal2Be account activation</title>
 </head>
 <body>
-    <h1>Hello, {{ username }}</h1>
-    <h3>To reset your password tap <a href="{{ host }}/password_reset?uuid={{ uuid }}&code={{ temp_code }}"><b>this link</b></a></h3>
-    <p>Link is available in {{ duration }}</p>
+    <h1>Hello, {{ user.username }}</h1>
+    <h3>To activate your email enter this code <a href="{{ host }}/{{ endpoint }}?uuid={{ user.uuid }}&code={{ code }}"><b>{{ code }}</b></a></h3>
+    <p>Code is available in {{ duration_text }}</p>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 
 
-****** Hello, {{ username }} ******
-**** To reset your password tap this_link ****
-Link is available in {{ duration }}
+****** Hello, {{ user.username }} ******
+**** To activate your email enter this code {{_code_}} ****
+Code is available in {{ duration_text }}
```

### Comparing `fastapi_all_out-0.2.8/LICENSE.md` & `fastapi_all_out-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.8/pyproject.toml` & `fastapi_all_out-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.2.8"
+version = "0.3.0"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
```

### Comparing `fastapi_all_out-0.2.8/PKG-INFO` & `fastapi_all_out-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.2.8
+Version: 0.3.0
 Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

