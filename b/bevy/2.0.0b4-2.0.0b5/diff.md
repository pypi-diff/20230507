# Comparing `tmp/bevy-2.0.0b4.tar.gz` & `tmp/bevy-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bevy-2.0.0b4.tar", max compression
+gzip compressed data, was "bevy-2.0.0b5.tar", max compression
```

## Comparing `bevy-2.0.0b4.tar` & `bevy-2.0.0b5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-04-23 20:31:40.040469 bevy-2.0.0b4/LICENSE
--rw-r--r--   0        0        0     5859 2023-04-23 20:31:40.040469 bevy-2.0.0b4/README.md
--rw-r--r--   0        0        0      213 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/__init__.py
--rw-r--r--   0        0        0     1463 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/contextvar.py
--rw-r--r--   0        0        0     1692 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/injectors/classes.py
--rw-r--r--   0        0        0     2244 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/injectors/functions.py
--rw-r--r--   0        0        0     2717 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/options.py
--rw-r--r--   0        0        0      164 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/annotated_provider.py
--rw-r--r--   0        0        0     3488 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/base.py
--rw-r--r--   0        0        0     1143 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/providers/type_provider.py
--rw-r--r--   0        0        0     6003 2023-04-23 20:31:40.040469 bevy-2.0.0b4/bevy/repository.py
--rw-r--r--   0        0        0      866 2023-04-23 20:31:40.044469 bevy-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 16:20:11.686032 bevy-2.0.0b5/LICENSE
+-rw-r--r--   0        0        0     5859 2023-05-07 16:20:11.686032 bevy-2.0.0b5/README.md
+-rw-r--r--   0        0        0      213 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/__init__.py
+-rw-r--r--   0        0        0     1463 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/contextvar.py
+-rw-r--r--   0        0        0     1692 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/injectors/classes.py
+-rw-r--r--   0        0        0     2244 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/injectors/functions.py
+-rw-r--r--   0        0        0     2717 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/options.py
+-rw-r--r--   0        0        0      164 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/__init__.py
+-rw-r--r--   0        0        0     1631 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/annotated_provider.py
+-rw-r--r--   0        0        0     3423 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/provider.py
+-rw-r--r--   0        0        0     1153 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/providers/type_provider.py
+-rw-r--r--   0        0        0     6559 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/repository.py
+-rw-r--r--   0        0        0      296 2023-05-07 16:20:11.686032 bevy-2.0.0b5/bevy/repository_cache.py
+-rw-r--r--   0        0        0      866 2023-05-07 16:20:11.686032 bevy-2.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 bevy-2.0.0b5/PKG-INFO
```

### Comparing `bevy-2.0.0b4/LICENSE` & `bevy-2.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/README.md` & `bevy-2.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/bevy/contextvar.py` & `bevy-2.0.0b5/bevy/contextvar.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/bevy/injectors/classes.py` & `bevy-2.0.0b5/bevy/injectors/classes.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/bevy/injectors/functions.py` & `bevy-2.0.0b5/bevy/injectors/functions.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/bevy/options.py` & `bevy-2.0.0b5/bevy/options.py`

 * *Files identical despite different names*

### Comparing `bevy-2.0.0b4/bevy/providers/annotated_provider.py` & `bevy-2.0.0b5/bevy/providers/annotated_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     TypeAlias,
     TypeVar,
     get_args,
     get_origin,
 )
 
 from bevy.options import Option, Value, Null
-from bevy.providers.base import Provider
+from bevy.providers.provider import Provider
+from bevy.repository_cache import RepositoryCache as _RepositoryCache
 
 _T = TypeVar("_T")
 _A: TypeAlias = Annotated[Type[_T], Hashable]
 
 
 def get_type(annotated: _A) -> Option[_T]:
     """Get the type being annotated by a typing.Annotated instance."""
@@ -26,20 +27,22 @@
             return Null()
 
 
 class AnnotatedProvider(Provider[_A, _T]):
     """The annotated provider supports typing.Annotated annotations. It will attempt to instantiate the annotated type
     if it's not found in the cache."""
 
-    def factory(self, annotated: _A) -> Option[Callable[[], _T]]:
+    def factory(
+        self, key: _A, cache: _RepositoryCache[_A, _T]
+    ) -> Option[Callable[[], _T]]:
         """Get a callable for getting or constructing an instance of the annotated type. This will call the repository's
         get method looking up the un-annotated type, this will attempt to instantiate an instance of the type if no
         providers have an instance cached."""
-        match get_type(annotated):
+        match get_type(key):
             case Value(type_):
-                return Value(partial(self._repository.get, type_))
+                return Value(partial(cache.repository.get, type_))
             case Null(message):
                 return Null(message)
 
-    def supports(self, annotated: _A) -> bool:
+    def supports(self, key: _A, _) -> bool:
         """Checks if the given key is indeed a typing.Annotated wrapped type."""
-        return bool(get_type(annotated)) and get_origin(annotated) is Annotated
+        return bool(get_type(key)) and get_origin(key) is Annotated
```

### Comparing `bevy-2.0.0b4/bevy/providers/base.py` & `bevy-2.0.0b5/bevy/providers/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable, Generic, TypeVar
 
 from bevy.options import Option, Null, Value
+from bevy.repository_cache import RepositoryCache as _RepositoryCache
 
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 Factory = Callable[[], _V]
 
 
 class NotFound(Null):
@@ -20,58 +21,50 @@
     offer any way to create new instances in the cache, so it shouldn't be considered a fully functional provider type.
     It is necessary for subclasses implement their own `factory` method to add support for this missing functionality.
 
     Every provider stores a reference to the repository it is attached to and a key/value cache for storing instances
     that it creates.
     """
 
-    def __init__(self, repository):
-        self._repository = repository
-        self._cache: dict[_K, _V] = {}
-
-    def create(self, key: _K) -> Option[_V]:
+    def create(self, key: _K, cache: _RepositoryCache[_K, _V]) -> Option[_V]:
         """Uses a factory function provided by the provider's factory method to get an instance that adheres to the type
         _V and that corresponds to the key. A Null option (NotSupported) is returned when no factory is available,
         otherwise a Value option containing the factory's return is returned.
         """
-        match self.factory(key):
-            case Value(factory) if self.supports(key):
-                self._cache[key] = factory()
-                return Value(self._cache[key])
+        match self.factory(key, cache):
+            case Value(factory) if self.supports(key, cache):
+                cache[key] = factory()
+                return Value(cache[key])
             case _:
                 return NotSupported(f"{type(self)!r} does not support {key!r}")
 
-    def factory(self, key: _K) -> Option[Factory]:
+    def factory(self, key: _K, cache: _RepositoryCache[_K, _V]) -> Option[Factory]:
         """The base provider returns a Null option as it does not support creating new instances that adhere to the type
         _V. This method should be overriden by base classes to create or lookup instances as appropriate that are
         returned as Value options.
         """
         return Null(f"{type(self)!r} does not support creating instances of {key!r}")
 
-    def find(self, key: _K) -> Option[_V]:
+    def find(self, key: _K, cache: _RepositoryCache[_K, _V]) -> Option[_V]:
         """Searches the cache for an instance that adheres to the type _V and that corresponds to the key. When a match
         is found, a Value option containing the instance is returned, otherwise a Null option (NotFound) is returned.
         """
         try:
-            return Value(self._cache[key])
+            return Value(cache[key])
         except KeyError as exception:
             return NotFound(f"{type(self)!r} has no instances cached for {key!r}")
 
-    def get_clone_factory(self) -> Callable[[], "Provider"]:
-        """Returns a callable that can be used to create an instance of the same type of provider."""
-        return type(self)
-
-    def set(self, key: _K, value: _V) -> Option[_V]:
+    def set(self, key: _K, value: _V, cache: _RepositoryCache[_K, _V]) -> Option[_V]:
         """Sets a value in the cache for the key only if the key is supported by the provider. A Null option
         (NotSupported) is returned when the key is not supported, otherwise a Value option containing the value placed
         in the cache is returned.
         """
-        if not self.supports(key):
+        if not self.supports(key, cache):
             return NotSupported(f"{type(self)!r} does not support {key!r}")
 
-        self._cache[key] = value
+        cache[key] = value
         return Value(value)
 
-    def supports(self, key: _K) -> bool:
+    def supports(self, key: _K, cache: _RepositoryCache[_K, _V]) -> bool:
         """Determines if the key is supported by the provider. Returns True if the `factory` method returns a Value
         option, False if it returned a Null option."""
-        return bool(self.factory(key))
+        return bool(self.factory(key, cache))
```

### Comparing `bevy-2.0.0b4/bevy/providers/type_provider.py` & `bevy-2.0.0b5/bevy/providers/type_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Callable, Type, TypeVar, Protocol, runtime_checkable
 
 from bevy.options import Option, Null, Value
-from bevy.providers.base import Provider
+from bevy.providers.provider import Provider
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
 class BevyConstructable(Protocol[_T]):
     @classmethod
     def __bevy_constructor__(cls: Type[_T], *args, **kwargs) -> _T:
         ...
 
 
 class TypeProvider(Provider[Type[_T], _T]):
     """The type provider supports any types and will attempt to instantiate them with no args."""
 
-    def factory(self, key: Type[_T]) -> Option[Callable[[], _T]]:
+    def factory(self, key: Type[_T], _) -> Option[Callable[[], _T]]:
         """Return a constructor callable for the key if it's a type. This will look for special dunder bevy constructor
         methods which will be preferred over the type callable."""
         match key:
             case BevyConstructable() as type_ if isinstance(type_, type):
                 return Value(type_.__bevy_constructor__)
             case type() as type_:
                 return Value(type_)
             case _:
                 return Null()
 
-    def supports(self, key: Type[_T]) -> bool:
+    def supports(self, key: Type[_T], _) -> bool:
         """Returns True only if the key is a type."""
         return isinstance(key, type)
```

### Comparing `bevy-2.0.0b4/bevy/repository.py` & `bevy-2.0.0b5/bevy/repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Generic, TypeVar, Type
 
 from bevy.contextvar import ContextVarDefaultFactory as _ContextVarDefaultFactory
 from bevy.options import Option, Value, Null
-from bevy.providers.base import Provider
+from bevy.providers.provider import Provider
+from bevy.repository_cache import RepositoryCache as _RepositoryCache
 
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 
 
 class _NullRepository(Generic[_K, _V]):
     """The Null Repository provides dead end null behavior. It is intended solely to simplify the propagation logic when
@@ -37,54 +38,61 @@
 class Repository(_NullRepository[_K, _V]):
     """The Bevy repository manages instance providers and caching the results that the providers create."""
 
     _bevy_repository: "_ContextVarDefaultFactory[Repository[_K, _V]]" = (
         _ContextVarDefaultFactory("bevy_context", default=lambda: Repository.factory())
     )
 
-    def __init__(self, parent: "Repository | None" = None):
+    def __init__(
+        self,
+        parent: "Repository | None" = None,
+        *,
+        providers: tuple[Provider[_K, _V]] = (),
+    ):
         self._parent = parent or _NullRepository()
-        self._providers: tuple[Provider[_K, _V]] = []
+        self._providers: dict[Provider[_K, _V], _RepositoryCache[_K, _V]] = {}
 
-    def add_providers(self, *providers: Type[Provider[_K, _V]]):
-        """Creates providers and adds them to the repository. These providers will be used to lookup and create
-        instances that will be stored and returned by the repository."""
-        self._providers = (
-            *(provider(self) for provider in providers),
-            *self._providers,
+        self.add_providers(*providers)
+
+    def add_providers(self, *providers: Provider[_K, _V]):
+        """Adds providers to the repository. These providers will be used to lookup and create instances that will be
+        stored and returned by the repository."""
+        self._providers.update(
+            (provider, _RepositoryCache(self))
+            for provider in providers
+            if provider not in self._providers
         )
 
     def branch(self) -> "Repository[_K, _V]":
-        branch = type(self)(self)
-
-        providers = (provider.get_clone_factory() for provider in self._providers)
-        branch.add_providers(*providers)
-
-        return branch
+        """Creates a new repository that inherits the providers from the current repository. Dependencies not found on
+        the new repository can be propagated to the branched parent repository. This allows the branch repository to
+        inherit dependencies from the parent repository and protects the parent from changes to the branch.
+        """
+        return type(self)(parent=self, providers=(*self._providers,))
 
     def create(self, key: _K) -> Option[_V]:
         """Attempts to create an instance that adheres to the type _V and that corresponds to the key by looking for a
         provider that supports the key. Returns a Null option when no provider is found for the key, otherwise returns a
         Value option containing the instance created by the provider."""
-        for provider in self._providers:
-            match provider.create(key):
+        for provider, repo in self._providers.items():
+            match provider.create(key, repo):
                 case Value(result):
                     return Value(result)
 
         return Null(f"No providers supported the {key!r}")
 
     def find(self, key: _K, *, allow_propagation: bool = True) -> Option[_V]:
         """Searches all providers for a cached instance that adheres to the type _V and that corresponds to the key.
         A Value option containing the matching instance is returned, when no match is found a Null option is returned.
 
         When `allow_propagation` is set to True (default) this will search any parent repositories for matching cached
         values.
         """
-        for provider in self._providers:
-            match provider.find(key):
+        for provider, repo in self._providers.items():
+            match provider.find(key, repo):
                 case Value() as result:
                     return result
 
         if allow_propagation:
             match self._parent.find(key):
                 case Value() as result:
                     return result
@@ -113,27 +121,27 @@
                 return result
             case Null():
                 return self.create(key).value_or(default)
 
     def set(self, key: _K, value: _V) -> Option[_V]:
         """Attempts to cache a value. A Null option is returned when no providers support the key, otherwise a Value
         option containing the value that was placed in the cache is returned."""
-        for provider in self._providers:
-            match provider.set(key, value):
+        for provider, repo in self._providers.items():
+            match provider.set(key, value, repo):
                 case Value(cached_value):
                     return Value(cached_value)
 
         return Null()
 
     @classmethod
     def factory(cls) -> "Repository[_K, _V]":
         from bevy.providers import AnnotatedProvider, TypeProvider
 
         repository = cls()
-        repository.add_providers(AnnotatedProvider, TypeProvider)
+        repository.add_providers(AnnotatedProvider(), TypeProvider())
         return repository
 
     @classmethod
     def get_repository(cls: "Type[Repository[_K, _V]]") -> "Repository[_K, _V]":
         """Retrieves the repository instance that is assigned to the current context."""
         return cls._bevy_repository.get()
```

### Comparing `bevy-2.0.0b4/pyproject.toml` & `bevy-2.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Bevy"
-version = "2.0.0b4"
+version = "2.0.0b5"
 description = "Python Dependency Inversion made simple so you can focus on creating amazing code."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ZechCodes/Bevy"
 repository = "https://github.com/ZechCodes/Bevy"
 documentation = "https://github.com/ZechCodes/Bevy/blob/master/README.md"
```

### Comparing `bevy-2.0.0b4/PKG-INFO` & `bevy-2.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bevy
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: Python Dependency Inversion made simple so you can focus on creating amazing code.
 Home-page: https://github.com/ZechCodes/Bevy
 License: MIT
 Keywords: dependency,injection,annotations,types
 Author: Zech Zimmerman
 Author-email: hi@zech.codes
 Requires-Python: >=3.10,<4.0
```

