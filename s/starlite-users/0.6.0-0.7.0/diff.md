# Comparing `tmp/starlite_users-0.6.0.tar.gz` & `tmp/starlite_users-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlite_users-0.6.0.tar", max compression
+gzip compressed data, was "starlite_users-0.7.0.tar", max compression
```

## Comparing `starlite_users-0.6.0.tar` & `starlite_users-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-03-26 16:53:28.475615 starlite_users-0.6.0/LICENSE
--rw-r--r--   0        0        0      809 2023-03-26 16:53:28.475615 starlite_users-0.6.0/README.md
--rw-r--r--   0        0        0     4317 2023-03-26 16:53:28.475615 starlite_users-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-03-26 16:53:28.475615 starlite_users-0.6.0/starlite_users/__init__.py
--rw-r--r--   0        0        0     1522 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/guid.py
--rw-r--r--   0        0        0     1517 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/mixins.py
--rw-r--r--   0        0        0     8141 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/repository.py
--rw-r--r--   0        0        0    11160 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/config.py
--rw-r--r--   0        0        0     2660 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/dependencies.py
--rw-r--r--   0        0        0     2830 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/exceptions.py
--rw-r--r--   0        0        0     5046 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/generics.py
--rw-r--r--   0        0        0     1485 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/guards.py
--rw-r--r--   0        0        0     8578 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/main.py
--rw-r--r--   0        0        0     1350 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/password.py
--rw-r--r--   0        0        0    13984 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/route_handlers.py
--rw-r--r--   0        0        0     2356 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/schema.py
--rw-r--r--   0        0        0    15311 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/service.py
--rw-r--r--   0        0        0     3354 2023-03-26 16:53:28.479615 starlite_users-0.6.0/starlite_users/user_handlers.py
--rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-15 08:50:32.380055 starlite_users-0.7.0/LICENSE
+-rw-r--r--   0        0        0      809 2023-05-15 08:50:32.380055 starlite_users-0.7.0/README.md
+-rw-r--r--   0        0        0     4317 2023-05-15 08:50:32.384055 starlite_users-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/__init__.py
+-rw-r--r--   0        0        0     1522 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/guid.py
+-rw-r--r--   0        0        0     1517 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0     8141 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/repository.py
+-rw-r--r--   0        0        0    13032 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/config.py
+-rw-r--r--   0        0        0     2660 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/dependencies.py
+-rw-r--r--   0        0        0     2830 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/exceptions.py
+-rw-r--r--   0        0        0     5046 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/generics.py
+-rw-r--r--   0        0        0     1485 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/guards.py
+-rw-r--r--   0        0        0     6734 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/main.py
+-rw-r--r--   0        0        0     1350 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/password.py
+-rw-r--r--   0        0        0    14243 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/route_handlers.py
+-rw-r--r--   0        0        0     2356 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/schema.py
+-rw-r--r--   0        0        0    15727 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/service.py
+-rw-r--r--   0        0        0     3354 2023-05-15 08:50:32.384055 starlite_users-0.7.0/starlite_users/user_handlers.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 starlite_users-0.7.0/PKG-INFO
```

### Comparing `starlite_users-0.6.0/LICENSE` & `starlite_users-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/README.md` & `starlite_users-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/pyproject.toml` & `starlite_users-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starlite-users"
-version = "0.6.0"
+version = "0.7.0"
 description = "Authentication and user management for Starlite"
 authors = ["Michael Bosch <michael@lonelyviking.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "starlite_users"}]
 
 [tool.poetry.dependencies]
```

### Comparing `starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/guid.py` & `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/guid.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/mixins.py` & `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/adapter/sqlalchemy/repository.py` & `starlite_users-0.7.0/starlite_users/adapter/sqlalchemy/repository.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/config.py` & `starlite_users-0.7.0/starlite_users/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Generic, Literal
 
 from pydantic import SecretStr
+from starlite.contrib.jwt import JWTAuth, JWTCookieAuth
 from starlite.exceptions import ImproperlyConfiguredException
+from starlite.security.session_auth import SessionAuth
 
 from starlite_users.adapter.sqlalchemy.mixins import (
     SQLAlchemyRoleMixin,
     UserModelType,
 )
 from starlite_users.adapter.sqlalchemy.repository import SQLAlchemyUserRepository
 from starlite_users.schema import (
     BaseRoleCreateDTO,
     BaseRoleReadDTO,
     BaseRoleUpdateDTO,
     BaseUserCreateDTO,
     BaseUserReadDTO,
     BaseUserUpdateDTO,
 )
+from starlite_users.user_handlers import (
+    get_jwt_retrieve_user_handler,
+    get_session_retrieve_user_handler,
+)
 
 __all__ = [
     "AuthHandlerConfig",
     "CurrentUserHandlerConfig",
     "PasswordResetHandlerConfig",
     "RegisterHandlerConfig",
     "RoleManagementHandlerConfig",
@@ -172,15 +178,15 @@
     user_repository_class: type[SQLAlchemyUserRepository] = SQLAlchemyUserRepository
     """The user repository class to use."""
     auth_exclude_paths: list[str] = field(default_factory=lambda: ["/schema"])
     """Paths to be excluded from authentication checks."""
     hash_schemes: list[str] = field(default_factory=lambda: ["argon2"])
     """Schemes to use for password encryption.
 
-    Defaults to `['argon2']`
+    Defaults to `["argon2"]`
     """
     session_backend_config: BaseBackendConfig | None = None
     """Optional backend configuration for session based authentication.
 
     Notes:
         - Required if `auth_backend` is set to `session`.
     """
@@ -247,14 +253,15 @@
     """
     verification_handler_config: VerificationHandlerConfig | None = None
     """Optional user verification route handler configuration. If set, registers the route handler(s) on the app.
 
     Note:
         - At least one route handler config must be set.
     """
+    _auth_config: JWTAuth | JWTCookieAuth | SessionAuth | None = None
 
     def __post_init__(self) -> None:
         """Validate the configuration.
 
         - A session backend must be configured if `auth_backend` is set to `'session'`.
         - At least one route handler must be configured.
         - `role_model`, `role_create_dto`, `role_read_dto` and `role_update_dto` are required fields if `role_management_handler_config` is configured.
@@ -276,7 +283,45 @@
             self.secret = SecretStr(self.secret)
         if len(self.secret) not in [16, 24, 32]:
             raise ImproperlyConfiguredException("secret must be 16, 24 or 32 characters")
         if all(getattr(self, config) is None for config in handler_configs):
             raise ImproperlyConfiguredException("at least one route handler must be configured")
         if self.role_management_handler_config and self.role_model is SQLAlchemyRoleMixin:
             raise ImproperlyConfiguredException("role_model must be set when role_management_handler_config is set")
+
+        self._auth_config = self._get_auth_config()
+
+    @property
+    def auth_config(self) -> JWTAuth | JWTCookieAuth | SessionAuth:
+        return self._auth_config or self._get_auth_config()
+
+    def _get_auth_config(self) -> JWTAuth | JWTCookieAuth | SessionAuth:
+        if self.auth_backend == "session":
+            return SessionAuth(
+                retrieve_user_handler=get_session_retrieve_user_handler(
+                    user_model=self.user_model,
+                    role_model=self.role_model,
+                    user_repository_class=self.user_repository_class,
+                ),
+                session_backend_config=self.session_backend_config,  # type: ignore
+                exclude=self.auth_exclude_paths,
+            )
+        if self.auth_backend == "jwt":
+            return JWTAuth(
+                retrieve_user_handler=get_jwt_retrieve_user_handler(
+                    user_model=self.user_model,
+                    role_model=self.role_model,
+                    user_repository_class=self.user_repository_class,
+                ),
+                token_secret=self.secret.get_secret_value(),
+                exclude=self.auth_exclude_paths,
+            )
+
+        return JWTCookieAuth(
+            retrieve_user_handler=get_jwt_retrieve_user_handler(
+                user_model=self.user_model,
+                role_model=self.role_model,
+                user_repository_class=self.user_repository_class,
+            ),
+            token_secret=self.secret.get_secret_value(),
+            exclude=self.auth_exclude_paths,
+        )
```

### Comparing `starlite_users-0.6.0/starlite_users/dependencies.py` & `starlite_users-0.7.0/starlite_users/dependencies.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/exceptions.py` & `starlite_users-0.7.0/starlite_users/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/generics.py` & `starlite_users-0.7.0/starlite_users/generics.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/guards.py` & `starlite_users-0.7.0/starlite_users/guards.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/main.py` & `starlite_users-0.7.0/starlite_users/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
-from starlite import HTTPRouteHandler, OpenAPIConfig, Request, Response, Router
-from starlite.contrib.jwt import JWTAuth, JWTCookieAuth
-from starlite.security.session_auth import SessionAuth
-
 from starlite_users.dependencies import get_service_dependency
 from starlite_users.exceptions import (
     RepositoryException,
     TokenException,
     repository_exception_handler,
     token_exception_handler,
 )
@@ -18,24 +14,23 @@
     get_current_user_handler,
     get_password_reset_handler,
     get_registration_handler,
     get_role_management_handler,
     get_user_management_handler,
     get_verification_handler,
 )
-from starlite_users.user_handlers import (
-    get_jwt_retrieve_user_handler,
-    get_session_retrieve_user_handler,
-)
 
 __all__ = ["StarliteUsers"]
 
 
 if TYPE_CHECKING:
+    from starlite import HTTPRouteHandler, Request, Response, Router
     from starlite.config import AppConfig
+    from starlite.contrib.jwt import JWTAuth, JWTCookieAuth
+    from starlite.security.session_auth import SessionAuth
 
     from starlite_users.config import StarliteUsersConfig
 
 
 class StarliteUsers:
     """A Starlite extension for authentication, authorization and user management."""
 
@@ -45,65 +40,28 @@
 
     def on_app_init(self, app_config: "AppConfig") -> "AppConfig":
         """Register routers, auth strategies etc on the Starlite app.
 
         Args:
             app_config: An instance of [AppConfig][starlite.config.AppConfig]
         """
-        auth_backend = self._get_auth_backend()
+        auth_backend = self._config.auth_config
         route_handlers = self._get_route_handlers(auth_backend)
 
-        app_config.openapi_config = OpenAPIConfig(
-            title="Security API",  # TODO: make configurable
-            version="0.1.0",  # TODO: make configurable
-        )
-        # will always be true
         app_config = auth_backend.on_app_init(app_config)
         app_config.route_handlers.extend(route_handlers)
 
         exception_handlers: dict[type[Exception], Callable[[Request, Any], Response]] = {
             TokenException: token_exception_handler,
             RepositoryException: repository_exception_handler,
         }
         app_config.exception_handlers.update(exception_handlers)  # type: ignore[arg-type]
 
         return app_config
 
-    def _get_auth_backend(self) -> JWTAuth | JWTCookieAuth | SessionAuth:
-        if self._config.auth_backend == "session":
-            return SessionAuth(
-                retrieve_user_handler=get_session_retrieve_user_handler(
-                    user_model=self._config.user_model,
-                    role_model=self._config.role_model,
-                    user_repository_class=self._config.user_repository_class,
-                ),
-                session_backend_config=self._config.session_backend_config,  # type: ignore
-                exclude=self._config.auth_exclude_paths,
-            )
-        if self._config.auth_backend == "jwt":
-            return JWTAuth(
-                retrieve_user_handler=get_jwt_retrieve_user_handler(
-                    user_model=self._config.user_model,
-                    role_model=self._config.role_model,
-                    user_repository_class=self._config.user_repository_class,
-                ),
-                token_secret=self._config.secret.get_secret_value(),
-                exclude=self._config.auth_exclude_paths,
-            )
-
-        return JWTCookieAuth(
-            retrieve_user_handler=get_jwt_retrieve_user_handler(
-                user_model=self._config.user_model,
-                role_model=self._config.role_model,
-                user_repository_class=self._config.user_repository_class,
-            ),
-            token_secret=self._config.secret.get_secret_value(),
-            exclude=self._config.auth_exclude_paths,
-        )
-
     def _get_route_handlers(
         self, auth_backend: JWTAuth | JWTCookieAuth | SessionAuth
     ) -> Sequence[HTTPRouteHandler | Router]:
         """Parse the route handler configs to get Routers."""
 
         handlers: list[HTTPRouteHandler | Router] = []
         service_dependency_provider = get_service_dependency(
```

### Comparing `starlite_users-0.6.0/starlite_users/password.py` & `starlite_users-0.7.0/starlite_users/password.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/route_handlers.py` & `starlite_users-0.7.0/starlite_users/route_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Type, Union
-from uuid import UUID  # noqa: TCH003
+from uuid import UUID
 
 from starlite import (
     HTTPRouteHandler,
     Provide,
     Request,
     Response,
     Router,
     delete,
     get,
     patch,
     post,
     put,
 )
 from starlite.contrib.jwt import JWTAuth, JWTCookieAuth
-from starlite.exceptions import ImproperlyConfiguredException, NotAuthorizedException
+from starlite.exceptions import ImproperlyConfiguredException, NotAuthorizedException, PermissionDeniedException
 from starlite.security.session_auth.auth import SessionAuth
 
 from starlite_users.adapter.sqlalchemy.mixins import UserModelType
 from starlite_users.schema import (
     ForgotPasswordSchema,
     ResetPasswordSchema,
     RoleCreateDTOType,
@@ -122,29 +122,35 @@
         """Authenticate a user."""
         if not isinstance(auth_backend, SessionAuth):
             raise ImproperlyConfiguredException("session login can only be used with SesssionAuth")
 
         user = await service.authenticate(data)
         if user is None:
             request.clear_session()
-            raise NotAuthorizedException()
+            raise NotAuthorizedException(detail="login failed, invalid input")
 
-        request.set_session({"user_id": user.id})  # TODO: move and make configurable
+        if user.is_verified is False:
+            raise PermissionDeniedException(detail="not verified")
+
+        request.set_session({"user_id": user.id})
         return user_read_dto.from_orm(user)
 
     @post(login_path, dependencies={"service": Provide(service_dependency)}, exclude_from_auth=True, tags=tags)
     async def login_jwt(data: UserAuthSchema, service: BaseUserService) -> Response[user_read_dto]:  # type: ignore
         """Authenticate a user."""
 
         if not isinstance(auth_backend, (JWTAuth, JWTCookieAuth)):
             raise ImproperlyConfiguredException("jwt login can only be used with JWTAuth")
 
         user = await service.authenticate(data)
         if user is None:
-            raise NotAuthorizedException()
+            raise NotAuthorizedException(detail="login failed, invalid input")
+
+        if user.is_verified is False:
+            raise PermissionDeniedException(detail="not verified")
 
         user_dto = user_read_dto.from_orm(user)
         return auth_backend.login(identifier=str(user.id), response_body=user_dto)
 
     @post(logout_path, tags=tags)
     async def logout(request: Request) -> None:
         """Log an authenticated user out."""
```

### Comparing `starlite_users-0.6.0/starlite_users/schema.py` & `starlite_users-0.7.0/starlite_users/schema.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/starlite_users/service.py` & `starlite_users-0.7.0/starlite_users/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         user_dict = data.dict(exclude={"password"})
         user_dict["password_hash"] = self.password_manager.hash(data.password)
         if not process_unsafe_fields:
             user_dict["is_verified"] = False
             user_dict["is_active"] = True
 
-        return await self.repository.add_user(self.user_model(**user_dict))
+        return await self.repository.add_user(self.user_model(**user_dict))  # pyright: ignore
 
     async def register(self, data: UserCreateDTOType) -> UserModelType | None:
         """Register a new user and optionally run custom business logic.
 
         Args:
             data: User creation data transfer object.
         """
@@ -147,25 +147,34 @@
 
     async def authenticate(self, data: UserAuthSchema) -> UserModelType | None:
         """Authenticate a user.
 
         Args:
             data: User authentication data transfer object.
         """
-        if not await self.pre_login_hook(data):
-            return None
-
-        user = await self.repository.get_user_by(email=data.email)
+        # avoid early returns to mitigate timing attacks.
+        # check if user supplied logic should allow authentication, but only
+        # supply the result later.
+        should_proceed = await self.pre_login_hook(data)
 
-        verified, new_password_hash = self.password_manager.verify_and_update(data.password, user.password_hash)
-        if not verified:
+        try:
+            user = await self.repository.get_user_by(email=data.email)
+        except RepositoryNotFoundException:
+            self.password_manager.hash(data.password)
             return None
+
+        password_verified, new_password_hash = self.password_manager.verify_and_update(
+            data.password, user.password_hash
+        )
         if new_password_hash is not None:
             user = await self.repository._update(user, {"password_hash": new_password_hash})
 
+        if not password_verified or not should_proceed:
+            return None
+
         await self.post_login_hook(user)
 
         return user
 
     def generate_token(self, user_id: "UUID", aud: str) -> str:
         """Generate a limited time valid JWT.
 
@@ -211,15 +220,15 @@
         """
         token = self._decode_and_verify_token(encoded_token, context="verify")
 
         user_id = token.sub
         try:
             user = await self.repository.update_user(user_id, {"is_verified": True})
         except RepositoryNotFoundException as e:
-            raise InvalidTokenException from e
+            raise InvalidTokenException("token is invalid") from e
 
         await self.post_verification_hook(user)
 
         return user
 
     async def initiate_password_reset(self, email: str) -> None:
         """Initiate the password reset flow.
@@ -262,15 +271,15 @@
             await self.repository.update_user(user_id, {"password_hash": self.password_manager.hash(password)})
         except RepositoryNotFoundException as e:
             raise InvalidTokenException from e
 
     async def pre_login_hook(self, data: UserAuthSchema) -> bool:  # pylint: disable=W0613
         """Execute custom logic to run custom business logic prior to authenticating a user.
 
-        Useful for authorization checks against external sources,
+        Useful for authentication checks against external sources,
         eg. current membership validity or blacklists, etc
         Must return `False` or raise a custom exception to cancel authentication.
 
         Args:
             data: Authentication data transfer object.
 
         Returns:
@@ -379,15 +388,15 @@
         """Add a new role to the database.
 
         Args:
             data: A role creation data transfer object.
         """
         if self.role_model is None or not issubclass(self.role_model, SQLAlchemyRoleMixin):
             raise ImproperlyConfiguredException("StarliteUsersConfig.role_model must subclass SQLAlchemyRoleMixin")
-        return await self.repository.add_role(self.role_model(**data.dict()))
+        return await self.repository.add_role(self.role_model(**data.dict()))  # pyright: ignore
 
     async def update_role(self, id_: "UUID", data: RoleUpdateDTOType) -> RoleModelType:
         """Update a role in the database.
 
         Args:
             id_: UUID corresponding to the role primary key.
             data: A role update data transfer object.
```

### Comparing `starlite_users-0.6.0/starlite_users/user_handlers.py` & `starlite_users-0.7.0/starlite_users/user_handlers.py`

 * *Files identical despite different names*

### Comparing `starlite_users-0.6.0/PKG-INFO` & `starlite_users-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlite-users
-Version: 0.6.0
+Version: 0.7.0
 Summary: Authentication and user management for Starlite
 License: MIT
 Author: Michael Bosch
 Author-email: michael@lonelyviking.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

