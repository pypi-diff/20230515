# Comparing `tmp/python_equilibrium-0.1.0.tar.gz` & `tmp/python_equilibrium-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.1.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.2.0.tar", max compression
```

## Comparing `python_equilibrium-0.1.0.tar` & `python_equilibrium-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,31 @@
--rw-r--r--   0        0        0      988 2023-04-29 15:23:39.604150 python_equilibrium-0.1.0/LICENSE
--rw-r--r--   0        0        0     1636 2023-05-02 10:00:46.981797 python_equilibrium-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-02 09:59:58.191169 python_equilibrium-0.1.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0      729 2023-05-02 09:53:38.977837 python_equilibrium-0.1.0/src/equilibrium/core/AdmissionController.py
--rw-r--r--   0        0        0     9737 2023-05-01 01:52:48.052887 python_equilibrium-0.1.0/src/equilibrium/core/Context.py
--rw-r--r--   0        0        0     8257 2023-05-02 09:53:48.345574 python_equilibrium-0.1.0/src/equilibrium/core/CrudResourceController.py
--rw-r--r--   0        0        0    12898 2023-05-01 01:48:24.240327 python_equilibrium-0.1.0/src/equilibrium/core/JsonResourceStore.py
--rw-r--r--   0        0        0     8286 2023-04-30 13:59:56.647308 python_equilibrium-0.1.0/src/equilibrium/core/JsonResourceStore_test.py
--rw-r--r--   0        0        0      612 2023-04-30 17:48:34.717773 python_equilibrium-0.1.0/src/equilibrium/core/Namespace.py
--rw-r--r--   0        0        0    13094 2023-05-01 01:44:15.691346 python_equilibrium-0.1.0/src/equilibrium/core/Resource.py
--rw-r--r--   0        0        0      497 2023-05-01 16:47:21.311143 python_equilibrium-0.1.0/src/equilibrium/core/ResourceController.py
--rw-r--r--   0        0        0     4841 2023-04-30 14:02:14.843419 python_equilibrium-0.1.0/src/equilibrium/core/ResourceStore.py
--rw-r--r--   0        0        0     2194 2023-04-30 13:55:02.819576 python_equilibrium-0.1.0/src/equilibrium/core/Resource_test.py
--rw-r--r--   0        0        0     1473 2023-05-01 01:38:46.172670 python_equilibrium-0.1.0/src/equilibrium/core/Service.py
--rw-r--r--   0        0        0        0 2023-04-30 01:55:51.676435 python_equilibrium-0.1.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 python_equilibrium-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-04-29 15:23:39.604150 python_equilibrium-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1648 2023-05-15 12:17:20.303965 python_equilibrium-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-15 12:17:20.303965 python_equilibrium-0.2.0/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 01:55:51.676435 python_equilibrium-0.2.0/src/equilibrium/py.typed
+-rw-r--r--   0        0        0      741 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/AdmissionController.py
+-rw-r--r--   0        0        0     8497 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/CrudResourceController.py
+-rw-r--r--   0        0        0    12910 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore.py
+-rw-r--r--   0        0        0     8298 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      616 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/Namespace.py
+-rw-r--r--   0        0        0    13234 2023-05-12 17:39:48.381669 python_equilibrium-0.2.0/src/equilibrium/resource/Resource.py
+-rw-r--r--   0        0        0    15071 2023-05-12 17:39:31.274153 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceContext.py
+-rw-r--r--   0        0        0      500 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceController.py
+-rw-r--r--   0        0        0     4849 2023-05-12 13:32:26.554091 python_equilibrium-0.2.0/src/equilibrium/resource/ResourceStore.py
+-rw-r--r--   0        0        0     2198 2023-05-12 13:32:26.582090 python_equilibrium-0.2.0/src/equilibrium/resource/Resource_test.py
+-rw-r--r--   0        0        0     2088 2023-05-12 13:44:07.098245 python_equilibrium-0.2.0/src/equilibrium/resource/Service.py
+-rw-r--r--   0        0        0      786 2023-05-12 14:13:31.848076 python_equilibrium-0.2.0/src/equilibrium/resource/__init__.py
+-rw-r--r--   0        0        0     2031 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Cache.py
+-rw-r--r--   0        0        0     3161 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Executor.py
+-rw-r--r--   0        0        0      853 2023-05-12 20:59:56.505150 python_equilibrium-0.2.0/src/equilibrium/rules/HashSupport.py
+-rw-r--r--   0        0        0     5223 2023-05-12 21:00:21.736435 python_equilibrium-0.2.0/src/equilibrium/rules/Params.py
+-rw-r--r--   0        0        0      898 2023-05-12 19:42:53.092371 python_equilibrium-0.2.0/src/equilibrium/rules/Params_test.py
+-rw-r--r--   0        0        0     3699 2023-05-15 12:11:03.698682 python_equilibrium-0.2.0/src/equilibrium/rules/Rule.py
+-rw-r--r--   0        0        0      417 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/Rule_test.py
+-rw-r--r--   0        0        0     3111 2023-05-12 20:59:56.661146 python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine.py
+-rw-r--r--   0        0        0     2682 2023-05-12 19:45:46.695447 python_equilibrium-0.2.0/src/equilibrium/rules/RulesEngine_test.py
+-rw-r--r--   0        0        0     3054 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph.py
+-rw-r--r--   0        0        0     2639 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-05-12 14:30:48.998605 python_equilibrium-0.2.0/src/equilibrium/rules/Signature.py
+-rw-r--r--   0        0        0      689 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/__init__.py
+-rw-r--r--   0        0        0     1415 2023-05-12 19:29:51.170583 python_equilibrium-0.2.0/src/equilibrium/rules/errors.py
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_equilibrium-0.2.0/PKG-INFO
```

### Comparing `python_equilibrium-0.1.0/LICENSE` & `python_equilibrium-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.1.0/pyproject.toml` & `python_equilibrium-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
 
@@ -18,37 +18,36 @@
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/python-equilibrium"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 "databind.json" = "^4.2.5"
 pyyaml = "^6.0"
-"nr.proxy" = "^1.1.1"
 types-pyyaml = "^6.0.12.9"
+networkx = "^3.1"
+typeapi = "^1.4.2"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pytest = "*"
 pycln = "^2.1.3"
 pyterprise = "^0.0.15"
 rich = "^13.3.5"
+networkx-stubs = "^0.0.1"
 
 [tool.slap]
 typed = true
 
-[tool.slap.release]
-branch = "main"
-
 [tool.slap.test]
 check = "slap check"
 mypy = "dmypy run src/ examples/"
-pytest = "pytest src/ examples/ -vv"
+pytest = "pytest src/ -vv --doctest-modules"
 black = "black --check src/ examples/"
 isort = "isort --check-only src/ examples/"
 flake8 = "flake8 src/ examples/"
 pycln = "pycln src/ examples/ -c"
 
 [tool.slap.run]
 fmt = "pycln src/ examples/ && black src/ examples/ && isort src/ examples/"
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/AdmissionController.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/AdmissionController.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from typing import Any
 
-from equilibrium.core.Resource import Resource
-from equilibrium.core.ResourceStore import ResourceStore
-from equilibrium.core.Service import Service
+from equilibrium.resource.Resource import Resource
+from equilibrium.resource.ResourceStore import ResourceStore
+from equilibrium.resource.Service import Service
 
 __all__ = ["AdmissionController"]
 
 
 class AdmissionController(ABC):
     """Controller to allow or deny admission of resources to the system."""
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/Context.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/ResourceContext.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 from __future__ import annotations
 
 import atexit
 import logging
 from dataclasses import dataclass
+from enum import Enum
 from os import PathLike
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Any, TypeVar
+from typing import Any, TypeVar, overload
 
 import yaml
-from nr.proxy import proxy
 
-from equilibrium.core.AdmissionController import AdmissionController
-from equilibrium.core.JsonResourceStore import JsonResourceStore
-from equilibrium.core.Namespace import Namespace
-from equilibrium.core.Resource import GenericResource, Resource
-from equilibrium.core.ResourceController import ResourceController
-from equilibrium.core.ResourceStore import ResourceStore
-from equilibrium.core.Service import Service
+from equilibrium.resource.AdmissionController import AdmissionController
+from equilibrium.resource.JsonResourceStore import JsonResourceStore
+from equilibrium.resource.Namespace import Namespace
+from equilibrium.resource.Resource import GenericResource, Resource
+from equilibrium.resource.ResourceController import ResourceController
+from equilibrium.resource.ResourceStore import ResourceStore
+from equilibrium.resource.Service import Service
 
-__all__ = ["Context"]
+__all__ = ["ResourceContext"]
 T = TypeVar("T")
 logger = logging.getLogger(__name__)
+DEFAULT_NAMESPACE = "default"
 
 
-class Context:
+class NotSet(Enum):
+    Value = 1
+
+
+class ResourceContext:
     """
     The controller context is the main entry point for managing
 
     * Resource controllers
     * Resource types
     * Resources
     * Resource state
     * Resource events [ Todo ]
     """
 
-    resources: ResourceStore
+    store: ResourceStore
+    services: ServiceRegistry
+    controllers: ControllerRegistry
+    resource_types: ResourceTypeRegistry
+    resources: ResourceRegistry
 
     @dataclass
     class InMemoryBackend:
         """Constructor for creating a context with an in-memory backend."""
 
         max_lock_duration: float | None = 5.0
 
@@ -47,171 +56,335 @@
     class JsonBackend:
         """Constructor for creating a context with a JSON backend."""
 
         directory: PathLike[str] | str
         max_lock_duration: float | None = 5.0
 
     @classmethod
-    def create(cls, backend: InMemoryBackend | JsonBackend) -> Context:
+    def create(cls, backend: InMemoryBackend | JsonBackend) -> ResourceContext:
         match backend:
             case cls.InMemoryBackend(max_lock_duration):
                 # TODO(@NiklasRosenstein): Actually implement an in-memory backend.
                 tempdir = TemporaryDirectory()
                 logger.debug("using temporary directory for in-memory backend: %r", tempdir.name)
                 atexit.register(tempdir.cleanup)
                 return cls(JsonResourceStore(Path(tempdir.name), max_lock_duration))
             case cls.JsonBackend(directory, max_lock_duration):
                 logger.debug("using JSON backend: %r", directory)
                 return cls(JsonResourceStore(Path(directory), max_lock_duration))
             case _:
                 raise TypeError(f"invalid backend type {backend!r}")
 
-    def __init__(self, store: ResourceStore, default_namespace_name: str = "default") -> None:
+    def __init__(self, store: ResourceStore, default_namespace: str = DEFAULT_NAMESPACE) -> None:
+        self.store = store
+        self.services = ServiceRegistry(store)
+        self.controllers = ControllerRegistry(self.store, self.services)
+        self.resource_types = ResourceTypeRegistry()
+        self.resource_types.register(Namespace)
+        self.resources = ResourceRegistry(store, self.resource_types, self.controllers, default_namespace)
+
+    def load_manifest(self, path: PathLike[str] | str) -> list[GenericResource]:
+        """
+        Loads a YAML file containing resource manifests into the store.
+        """
+
+        resources = []
+        with Path(path).open() as fp:
+            for payload in yaml.safe_load_all(fp):
+                resource = Resource.of(payload)
+                resources.append(self.resources.put(resource))
+        return resources
+
+
+class ControllerRegistry:
+    def __init__(self, resources: ResourceStore, services: ServiceRegistry) -> None:
+        self._resources = resources
+        self._services = services
         self._resource_controllers: list[ResourceController] = []
         self._admission_controllers: list[AdmissionController] = []
-        self._resource_types: dict[str, dict[str, type[Resource.Spec]]] = {}
-        self._default_namespace_name = default_namespace_name
-        self._services: dict[Resource.Type, dict[Service.Id, Service]] = {}
-        self.resources = store
-        self.register_resource_type(Namespace)
 
-    def register_resource_type(self, resource_type: type[Resource.Spec]) -> None:
-        self._resource_types.setdefault(resource_type.API_VERSION, {})[resource_type.KIND] = resource_type
-
-    def register_controller(self, controller: ResourceController | AdmissionController) -> None:
-        controller.resources = proxy(lambda: self.resources)  # type: ignore[assignment]
-        controller.services = _ContextServiceProvider(self)
+    def register(self, controller: ResourceController | AdmissionController) -> None:
+        assert isinstance(controller, (ResourceController, AdmissionController))
+        controller.resources = self._resources
+        controller.services = self._services
         if isinstance(controller, AdmissionController):
             self._admission_controllers.append(controller)
         if isinstance(controller, ResourceController):
             self._resource_controllers.append(controller)
 
-    def register_service(self, resource_type: Resource.Type, service: Service) -> None:
+    def admit(self, resource: Resource[Any]) -> Resource[Any]:
+        uri = resource.uri
+        # Pass resource through admission controllers.
+        for controller in self._admission_controllers:
+            try:
+                new_resource = controller.admit_resource(resource)
+            except Exception as e:
+                raise Resource.AdmissionFailed(resource.uri, e) from e
+            if new_resource.uri != uri:
+                raise RuntimeError(f"Admission controller mutated resource URI (controller: {controller!r})")
+            if type(new_resource.spec) != type(resource.spec):  # noqa: E721
+                raise RuntimeError(f"Admission controller mutated resource spec type (controller: {controller!r})")
+            resource = new_resource
+        return resource
+
+    def reconcile(self) -> None:
+        for controller in self._resource_controllers:
+            logger.debug(f"Reconciling {controller!r}")
+            controller.reconcile()
+
+
+class ResourceTypeRegistry:
+    def __init__(self) -> None:
+        self._resource_types: dict[str, dict[str, type[Resource.Spec]]] = {}
+
+    def __contains__(self, resource_type: Resource.Type) -> bool:
+        if resource_type.apiVersion not in self._resource_types:
+            return False
+        return resource_type.kind in self._resource_types[resource_type.apiVersion]
+
+    def register(self, spec_type: type[Resource.Spec]) -> None:
+        self._resource_types.setdefault(spec_type.API_VERSION, {})[spec_type.KIND] = spec_type
+
+    def get(self, resource_type: Resource.Type) -> type[Resource.Spec] | None:
+        return self._resource_types.get(resource_type.apiVersion, {}).get(resource_type.kind)
+
+
+class ServiceRegistry(Service.Provider):
+    def __init__(self, resources: ResourceStore) -> None:
+        self._resources = resources
+        self._services: dict[Resource.Type, dict[Service.Id, Service]] = {}
+
+    def register(self, resource_type: Resource.Type | type[Resource.Spec], service: Service) -> None:
         """
         Register a service to the controller for the given resource type.
         """
 
-        service.resources = proxy(lambda: self.resources)  # type: ignore[assignment]
-        service.services = _ContextServiceProvider(self)
+        if isinstance(resource_type, type):
+            resource_type = resource_type.TYPE
+
+        service.resources = self._resources
+        service.services = self
         services = self._services.setdefault(resource_type, {})
         if service.SERVICE_ID in services:
             raise ValueError(
                 f"Service '{service.SERVICE_ID}' is already registered for resource type {resource_type!r}"
             )
         services[service.SERVICE_ID] = service
 
-    def get_service(self, resource_type: Resource.Type, service_type: type[Service.T]) -> Service.T | None:
+    @overload
+    def get(
+        self,
+        resource_type: Resource.Type | type[Resource.Spec],
+        service_type: type[Service.T],
+    ) -> Service.T:
+        ...
+
+    @overload
+    def get(
+        self,
+        resource_type: Resource.Type | type[Resource.Spec],
+        service_type: type[Service.T],
+        default: T,
+    ) -> Service.T | T:
+        ...
+
+    def get(
+        self,
+        resource_type: Resource.Type | type[Resource.Spec],
+        service_type: type[Service.T],
+        default: T | NotSet = NotSet.Value,
+    ) -> Service.T | T:
         """
-        Find a service registered for the given resource type and service type.
+        Obtain a service for the given resource type. If the service is not registered, None is returned.
         """
 
+        if isinstance(resource_type, type):
+            resource_type = resource_type.TYPE
+
         services = self._services.get(resource_type)
         service = services.get(service_type.SERVICE_ID) if services else None
         if service is not None and not isinstance(service, service_type):
             raise RuntimeError(f"Service '{service_type.SERVICE_ID}' is not of type {service_type!r}")
+        if service is None:
+            if default is NotSet.Value:
+                raise KeyError(
+                    f"Service '{service_type.SERVICE_ID}' is not registered for resource type {resource_type!r}"
+                )
+            return default
         return service
 
-    def put_resource(self, resource: Resource[Any]) -> Resource[Any]:
+
+class ResourceRegistry:
+    """
+    A high-level interface to the resource store, which can controls resource admission.
+    """
+
+    def __init__(
+        self,
+        store: ResourceStore,
+        resource_types: ResourceTypeRegistry,
+        controllers: ControllerRegistry,
+        default_namespace: str,
+    ) -> None:
+        self._store = store
+        self._resource_types = resource_types
+        self._controllers = controllers
+        self._default_namespace = default_namespace
+
+    @overload
+    def get(self, uri: Resource.URI) -> GenericResource:
+        ...
+
+    @overload
+    def get(self, uri: Resource.URI, default: T) -> GenericResource | T:
+        ...
+
+    def get(self, uri: Resource.URI, default: T | NotSet = NotSet.Value) -> GenericResource | T:
+        """
+        Get a resource by full URI.
+        """
+
+        with self._store.enter(self._store.LockRequest.from_uri(uri)) as lock:
+            result = self._store.get(lock, uri)
+        if result is None:
+            if default is NotSet.Value:
+                raise Resource.NotFound(uri)
+            return default
+        return result
+
+    def put(self, resource: Resource[Any], stateful: bool = False) -> Resource[Any]:
         """
         Put a resource into the resource store. This will trigger the admission controllers. Any admission controller
         may complain about the resource, mutate it and raise an exception if necessary. This exception will propagate
-        to the caller of #put_resource().
+        to the caller of #put().
 
-        Note that this method does not permit a resource which has state. This method can only be used to update a
-        resource's metadata and spec. The state will be inherited from the existing resource, if it exists.
+        Note that this method does not permit a resource which has state unless the *stateful* flag is set to True.
+        This method should only be used to update a resource's metadata and spec. The state will be inherited from
+        existing resource, if it exists.
+
+        If the *stateful* flag is set to True, the state of the resource will be committed to the resource store.
+        Note that this also means that if the specified *resource* has no state, but the store currently does store
+        a state for the resource, that state will be deleted.
         """
 
-        # Validate that the resource type is registered.
-        if resource.apiVersion not in self._resource_types:
-            raise ValueError(f"Unknown resource type: {resource.apiVersion}/{resource.kind}")
-        if resource.kind not in self._resource_types[resource.apiVersion]:
-            raise ValueError(f"Unknown resource type: {resource.apiVersion}/{resource.kind}")
-
-        if resource.state is not None:
+        if not stateful and resource.state is not None:
             raise ValueError("Cannot put a resource with state into the resource store")
 
-        uri = resource.uri
-        resource_spec = self._resource_types[resource.apiVersion][resource.kind]
+        resource_spec = self._resource_types.get(resource.type)
+        if resource_spec is None:
+            raise ValueError(f"Unknown resource type: {resource.apiVersion}/{resource.kind}")
 
         # Ensure that we have the resource in its deserialized (i.e. non-generic) form.
+        uri = resource.uri
         resource = resource.into(resource_spec)
 
-        with self.resources.enter(self.resources.LockRequest.from_uri(uri)) as lock:
-            # Validate the resource spec.
-            try:
-                resource.spec.validate()
-            except Exception as e:
-                raise Resource.ValidationFailed(resource.uri, e) from e
-
-            # Give the resource the default namespace.
-            if uri.namespace is None and resource_spec.NAMESPACED:
-                resource.metadata = resource.metadata.with_namespace(self._default_namespace_name)
-                uri = resource.uri
-            resource_spec.check_uri(resource.uri, do_raise=True)
-
-            # Pass resource through admission controllers.
-            for controller in self._admission_controllers:
-                try:
-                    new_resource = controller.admit_resource(resource)
-                except Exception as e:
-                    raise Resource.AdmissionFailed(resource.uri, e) from e
-                if new_resource.uri != uri:
-                    raise RuntimeError(f"Admission controller mutated resource URI (controller: {controller!r})")
-                if type(new_resource.spec) != type(resource.spec):  # noqa: E721
-                    raise RuntimeError(f"Admission controller mutated resource spec type (controller: {controller!r})")
-                resource = resource
-
-            # Inherit the state of an existing resource, if it exists.
-            existing_resource = self.resources.get(lock, uri)
-            resource.state = existing_resource.state if existing_resource else None
+        # Validate the resource spec.
+        try:
+            resource.spec.validate()
+        except Exception as e:
+            raise Resource.ValidationFailed(resource.uri, e) from e
+
+        # Give the resource the default namespace.
+        if uri.namespace is None and resource_spec.NAMESPACED:
+            resource.metadata = resource.metadata.with_namespace(self._default_namespace)
+            uri = resource.uri
+        resource_spec.check_uri(resource.uri, do_raise=True)
+
+        # Check for admission errors.
+        resource = self._controllers.admit(resource)
+
+        with self._store.enter(self._store.LockRequest.from_uri(uri)) as lock:
+            if not stateful:
+                # Inherit the state of an existing resource, if it exists.
+                existing_resource = self._store.get(lock, uri)
+                resource.state = existing_resource.state if existing_resource else None
 
             logger.debug("Putting resource '%s'.", uri)
-            self.resources.put(lock, resource.into_generic())
+            self._store.put(lock, resource.into_generic())
 
         return resource
 
-    def delete_resource(self, uri: Resource.URI, *, do_raise: bool = True, force: bool = False) -> bool:
+    def delete(self, uri: Resource.URI, *, do_raise: bool = True, force: bool = False) -> bool:
         """
         Mark a resource as deleted. A controller must take care of actually removing it from the system.
         If *force* is True, the resource will be removed from the store immediately. If the resource is not found,
         a #Resource.NotFound error will be raised.
 
         If *do_raise* is False, this method will return False if the resource was not found.
         """
 
-        with self.resources.enter(self.resources.LockRequest.from_uri(uri)) as lock:
-            resource = self.resources.get(lock, uri)
+        with self._store.enter(self._store.LockRequest.from_uri(uri)) as lock:
+            resource = self._store.get(lock, uri)
             if resource is None:
                 logger.info("Could not delete Resource '%s', not found.", uri)
                 if do_raise:
                     raise Resource.NotFound(uri)
                 return False
             if force:
                 logger.info("Force deleting resource '%s'.", uri)
-                self.resources.delete(lock, uri)
+                self._store.delete(lock, uri)
             elif resource.deletion_marker is None:
                 logger.info("Marking resource '%s' as deleted.", uri)
                 resource.deletion_marker = Resource.DeletionMarker()
+                self._store.put(lock, resource)
             else:
                 logger.info("Resource '%s' is already marked as deleted.", uri)
             return True
 
-    def load_manifest(self, path: PathLike[str] | str) -> list[GenericResource]:
-        resources = []
-        with Path(path).open() as fp:
-            for payload in yaml.safe_load_all(fp):
-                resource = Resource.of(payload)
-                resources.append(self.put_resource(resource))
-        return resources
-
-    def reconcile_once(self) -> None:
-        for controller in self._resource_controllers:
-            logger.debug(f"Reconciling {controller!r}")
-            controller.reconcile_once()
+    def search(
+        self,
+        *,
+        apiVersion: str | None = None,
+        kind: str | None = None,
+        namespace: str | None = "",
+        name: str | None = None,
+        labels: dict[str, str] | None = None,
+    ) -> list[Resource.URI]:
+        """
+        Search for resources of the given type. If *namespace* is `""`, all namespaces and unnamespaced resources will
+        be searched. If *namespace* is `None`, only unnamespaced resources will be searched. If *name* is given, only
+        resources with that name will be returned.
+        """
 
+        with self._store.enter(self._store.LockRequest(apiVersion, kind, namespace, name)) as lock:
+            return list(
+                self._store.search(
+                    lock,
+                    self._store.SearchRequest(
+                        apiVersion,
+                        kind,
+                        namespace,
+                        name,
+                        labels,
+                    ),
+                )
+            )
 
-class _ContextServiceProvider(Service.Provider):
-    def __init__(self, context: Context) -> None:
-        self._context = context
+    def list(
+        self,
+        spec_type: type[Resource.T_Spec],
+        *,
+        namespace: str | None = "",
+        name: str | None = None,
+        labels: dict[str, str] | None = None,
+    ) -> list[Resource[Resource.T_Spec]]:
+        """
+        Combines #search() and #get() to return a list of resources of the given type.
+        """
 
-    def get(self, resource_type: Resource.Type, service_type: type[Service.T]) -> Service.T | None:
-        return self._context.get_service(resource_type, service_type)
+        with self._store.enter(self._store.LockRequest(spec_type.API_VERSION, spec_type.KIND, namespace, name)) as lock:
+            uris = self._store.search(
+                lock,
+                self._store.SearchRequest(
+                    spec_type.API_VERSION,
+                    spec_type.KIND,
+                    namespace,
+                    name,
+                    labels,
+                ),
+            )
+            result = []
+            for uri in uris:
+                resource = self._store.get(lock, uri)
+                if resource is not None:
+                    result.append(resource.into(spec_type))
+        return result
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/CrudResourceController.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/CrudResourceController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from abc import abstractmethod
 from enum import Enum
 from logging import Logger
 from typing import Any, ClassVar, Generic
 
-from equilibrium.core.AdmissionController import AdmissionController
-from equilibrium.core.Resource import Resource
-from equilibrium.core.ResourceController import ResourceController
-from equilibrium.core.ResourceStore import ResourceStore
+from equilibrium.resource.AdmissionController import AdmissionController
+from equilibrium.resource.Resource import Resource
+from equilibrium.resource.ResourceController import ResourceController
+from equilibrium.resource.ResourceStore import ResourceStore
 
 __all__ = ["CrudResourceController"]
 
 
 class CrudResourceController(ResourceController, AdmissionController, Generic[Resource.T_Spec, Resource.T_State]):
     """
     A base class for resource controllers that follow a CRUD pattern and may also control admittance.
@@ -96,15 +96,19 @@
                     raise RuntimeError(
                         f"{type(self).__name__}.read() is expected to return an object of type "
                         f"{self.state_type.__name__} or Status.Deleted, got {type(response).__name__} instead."
                     )
                 else:
                     current_state = response
 
-            if current_state is None:
+            if current_state is None and resource.deletion_marker:
+                log.debug(
+                    "Resource '%s' is marked for deletion and has no current state, skipping reconciliation.", uri
+                )
+            elif current_state is None:
                 if resource.state is None:
                     log.debug("Resource '%s' is new, creating it.", uri)
                 else:
                     log.debug("Resource '%s' was lost, creating it.", uri)
 
                 current_state = self.create(resource)
                 if not isinstance(current_state, self.state_type):
@@ -143,15 +147,15 @@
                 self.resources.put(lock, resource.into_generic())
 
         except Exception:
             log.exception("An unhandled exception occurred reconciling a resource.")
 
     # ResourceController
 
-    def reconcile_once(self) -> None:
+    def reconcile(self) -> None:
         self.log = self._get_logger(None)
 
         namespaces = self.resources.namespaces()
         self.log.info(
             "Reconciling resources of type '%s' (namespaces: %r)",
             self.spec_type.TYPE,
             {ns.metadata.name for ns in namespaces},
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/JsonResourceStore.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from threading import Condition, get_ident as get_thread_id
 from time import perf_counter
 from typing import Any, Callable, Iterable, Iterator, TypeAlias
 from uuid import uuid4
 
 import databind.json
 
-from equilibrium.core.Namespace import Namespace
-from equilibrium.core.Resource import GenericResource, Resource, match_labels
-from equilibrium.core.ResourceStore import ResourceStore
+from equilibrium.resource.Namespace import Namespace
+from equilibrium.resource.Resource import GenericResource, Resource, match_labels
+from equilibrium.resource.ResourceStore import ResourceStore
 
 logger = getLogger(__name__)
 
 __all__ = ["JsonResourceStore"]
 
 
 class JsonResourceStore(ResourceStore):
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/JsonResourceStore_test.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/JsonResourceStore_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import tempfile
 from pathlib import Path
 from threading import Thread
 from typing import Iterator
 
 import pytest
 
-from equilibrium.core.JsonResourceStore import JsonResourceStore
-from equilibrium.core.Namespace import Namespace
-from equilibrium.core.Resource import Resource
+from equilibrium.resource.JsonResourceStore import JsonResourceStore
+from equilibrium.resource.Namespace import Namespace
+from equilibrium.resource.Resource import Resource
 
 LockID = JsonResourceStore.LockID
 
 
 @pytest.fixture
 def tempdir() -> Iterator[Path]:
     with tempfile.TemporaryDirectory() as tmpdir:
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/Namespace.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/Namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The namespace resource is builtin by default.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from equilibrium.core.Resource import Resource
+from equilibrium.resource.Resource import Resource
 
 __all__ = ["Namespace"]
 
 
 @dataclass
 class Namespace(Resource.Spec, apiVersion="v1", kind="Namespace", namespaced=False):
     @staticmethod
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/Resource.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/Resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass, field, replace
 from datetime import datetime, timezone
+from functools import total_ordering
 from typing import Any, ClassVar, Generic, Literal, Mapping, Protocol, Type as _Type, TypeVar, cast, overload
 
 import databind.json
 from databind.json.settings import JsonConverter
 from typing_extensions import Self  # 3.11+
 
 __all__ = ["Resource", "match_labels", "validate_api_version", "validate_identifier"]
@@ -50,18 +51,18 @@
     @dataclass
     class AdmissionFailed(Error):
         uri: Resource.URI
         exc: Exception
 
     class Spec(Dataclass):
         __dataclass_fields__: Mapping[str, Any]
-        API_VERSION: ClassVar[str] = ""
-        KIND: ClassVar[str] = ""
-        NAMESPACED: ClassVar[bool] = False
-        TYPE: ClassVar[Resource.Type] = None  # type: ignore[assignment]
+        API_VERSION: ClassVar[str]
+        KIND: ClassVar[str]
+        NAMESPACED: ClassVar[bool]
+        TYPE: ClassVar[Resource.Type]
 
         def __init_subclass__(cls, apiVersion: str, kind: str, namespaced: bool = True) -> None:
             cls.API_VERSION = apiVersion
             cls.KIND = kind
             cls.NAMESPACED = namespaced
             cls.TYPE = Resource.Type(apiVersion, kind)
             return super().__init_subclass__()
@@ -121,14 +122,15 @@
 
     T_Spec = TypeVar("T_Spec", bound="Resource.Spec")
     T_State = TypeVar("T_State", bound="Resource.State")
     GenericSpec = dict[str, Any]
     GenericState = dict[str, Any]
 
     @JsonConverter.using_classmethods(serialize="__str__", deserialize="of")
+    @total_ordering
     @dataclass(frozen=True)
     class URI:
         apiVersion: str
         kind: str
         namespace: str | None
         name: str
 
@@ -139,23 +141,29 @@
                 validate_identifier(self.namespace, "namespace")
             validate_identifier(self.name, "name")
 
         def __str__(self) -> str:
             if self.namespace is not None:
                 return f"{self.apiVersion}/{self.kind}/{self.namespace}/{self.name}"
             else:
-                return f"{self.apiVersion}/{self.kind}/{self.name}"
+                return f"{self.apiVersion}/{self.kind}//{self.name}"
+
+        def __lt__(self, other: Any) -> bool:
+            if type(other) == Resource.URI:
+                return str(self) < str(other)
+            else:
+                return NotImplemented
 
         @staticmethod
         def of(s: str) -> Resource.URI:
             parts = s.split("/")
             try:
                 apiVersion = "/".join(parts[:-3])
                 kind = parts[-3]
-                namespace = parts[-2]
+                namespace = parts[-2] or None
                 name = parts[-1]
             except IndexError:
                 raise ValueError(f"invalid Resource.URI: {s!r}")
             return Resource.URI(apiVersion, kind, namespace, name)
 
         @property
         def type(self) -> Resource.Type:
@@ -253,15 +261,15 @@
     state: GenericState | None = None
 
     def __post_init__(self) -> None:
         validate_api_version(self.apiVersion, "apiVersion")
         validate_identifier(self.kind, "kind")
 
     def __repr__(self) -> str:
-        return f"Resource(apiVersion={self.apiVersion!r}, kind={self.kind!r}, metadata={self.metadata!r})"
+        return f"Resource('{self.uri}')"
 
     @property
     def type(self) -> Type:
         return Resource.Type(self.apiVersion, self.kind)
 
     @property
     def locator(self) -> Locator:
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/ResourceStore.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/ResourceStore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import Iterator, NewType
 
-from equilibrium.core.Namespace import Namespace
-from equilibrium.core.Resource import GenericResource, Resource
+from equilibrium.resource.Namespace import Namespace
+from equilibrium.resource.Resource import GenericResource, Resource
 
 __all__ = ["ResourceStore"]
 
 
 class ResourceStore(ABC):
     """Provides an API for storing and loading resources."""
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/Resource_test.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/Resource_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Any
 
 import pytest
 
-from equilibrium.core.Resource import Resource
+from equilibrium.resource.Resource import Resource
 
 
 def test__Resource_URI__validates_apiVersion() -> None:
     Resource.URI("v1", "MyResource", "default", "my-resource")
     Resource.URI("example.com/v1", "MyResource", "default", "my-resource")
     with pytest.raises(ValueError):
         Resource.URI("example_com/v1", "MyResource", "default", "my-resource")
```

### Comparing `python_equilibrium-0.1.0/src/equilibrium/core/Service.py` & `python_equilibrium-0.2.0/src/equilibrium/resource/Service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, ClassVar, NewType, TypeVar
 
-from equilibrium.core.Resource import Resource
-from equilibrium.core.ResourceStore import ResourceStore
+from equilibrium.resource.Resource import Resource
+from equilibrium.resource.ResourceStore import ResourceStore
 
 
 def validate_service_id(s: str) -> None:
     try:
         Resource.Type.of(s)
     except ValueError:
         raise ValueError(f"Invalid serviceId: {s!r}")
@@ -22,22 +22,33 @@
 
     Id = NewType("Id", str)
     T = TypeVar("T", bound="Service")
 
     #: A globally unique identifier of the service type. The identifier is used to retrieve the service from the
     #: context. This must begin with an apiVersion and end with a kind, separated by a slash. The apiVersion and kind
     #: must be valid DNS subdomains.
-    SERVICE_ID: ClassVar[Id] = Id("")
+    SERVICE_ID: ClassVar[Id]
 
     #: Assigned to the service upon registration to the context.
     resources: ResourceStore
     services: Service.Provider
 
     class Provider(ABC):
         @abstractmethod
         def get(self, resource_type: Resource.Type, service_type: type[Service.T]) -> Service.T | None:
             ...
 
-    def __init_subclass__(cls, serviceId: str, **kwargs: Any) -> None:
-        validate_service_id(serviceId)
-        cls.SERVICE_ID = cls.Id(serviceId)
+    def __init_subclass__(cls, serviceId: str | None = None, **kwargs: Any) -> None:
+        # Check if any of the base classes is a subclass of the service. In this case, the `serviceId` is inherited
+        # and must not be redefined.
+        if any(issubclass(x, Service) and x is not Service for x in cls.__bases__):
+            if serviceId is not None:
+                raise RuntimeError("Service implementation must not redefine serviceId")
+            assert hasattr(cls, "SERVICE_ID"), "Service parent class should have a serviceId defined."
+
+        else:
+            if serviceId is None:
+                raise RuntimeError("Service subclass must define serviceId")
+            validate_service_id(serviceId)
+            cls.SERVICE_ID = cls.Id(serviceId)
+
         return super().__init_subclass__(**kwargs)
```

### Comparing `python_equilibrium-0.1.0/PKG-INFO` & `python_equilibrium-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: databind.json (>=4.2.5,<5.0.0)
-Requires-Dist: nr.proxy (>=1.1.1,<2.0.0)
+Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: typeapi (>=1.4.2,<2.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-equilibrium/issues
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-equilibrium
```

