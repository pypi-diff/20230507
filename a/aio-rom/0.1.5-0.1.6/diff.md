# Comparing `tmp/aio-rom-0.1.5.tar.gz` & `tmp/aio_rom-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-rom-0.1.5.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aio-rom-0.1.5.tar` & `aio_rom-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,29 @@
--rw-r--r--   0        0        0     1071 2022-02-19 18:34:35.882046 aio-rom-0.1.5/LICENSE
--rw-r--r--   0        0        0     1280 2022-02-19 18:34:35.882046 aio-rom-0.1.5/README.md
--rw-r--r--   0        0        0      148 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/__init__.py
--rw-r--r--   0        0        0     7668 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/collections.py
--rw-r--r--   0        0        0      259 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/dataclasses.py
--rw-r--r--   0        0        0      154 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/exception.py
--rw-r--r--   0        0        0     3871 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/fields.py
--rw-r--r--   0        0        0     4979 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/model.py
--rw-r--r--   0        0        0        0 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/py.typed
--rw-r--r--   0        0        0     2475 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/session.py
--rw-r--r--   0        0        0     1727 2022-02-19 18:34:35.882046 aio-rom-0.1.5/aio_rom/types.py
--rw-r--r--   0        0        0      449 2022-02-19 18:34:35.886046 aio-rom-0.1.5/aio_rom/utils.py
--rw-r--r--   0        0        0      986 2022-02-19 18:34:35.886046 aio-rom-0.1.5/aio_rom/utils.pyi
--rw-r--r--   0        0        0     2594 2022-02-19 18:34:35.886046 aio-rom-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aio-rom-0.1.5/setup.py
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 aio-rom-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 aio_rom-0.1.6/dev-requirements.txt
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aio_rom-0.1.6/requirements.txt
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 aio_rom-0.1.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 aio_rom-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 aio_rom-0.1.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aio_rom-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/__init__.py
+-rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/collections.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/dataclasses.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/exception.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/fields.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/model.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/proxy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/py.typed
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/session.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/types.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/utils.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 aio_rom-0.1.6/aio_rom/utils.pyi
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/test_model.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/test_proxy.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/test_redis.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/test_redis_benchmark.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 aio_rom-0.1.6/tests/test_redis_collections.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 aio_rom-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aio_rom-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 aio_rom-0.1.6/README.md
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 aio_rom-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 aio_rom-0.1.6/PKG-INFO
```

### Comparing `aio-rom-0.1.5/LICENSE` & `aio_rom-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-rom-0.1.5/README.md` & `aio_rom-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aio-rom-0.1.5/aio_rom/collections.py` & `aio_rom-0.1.6/aio_rom/collections.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import typing
 from abc import ABCMeta, abstractmethod
 from collections import UserList
 from typing import (
     Any,
     AsyncIterable,
     AsyncIterator,
     ClassVar,
@@ -14,56 +15,62 @@
     Iterator,
     List,
     MutableSet,
     Type,
     TypeVar,
 )
 
-from aioredis.client import Pipeline, Redis
+from aio_rom.fields import deserialize, serialize
+from aio_rom.session import connection, transaction
+from aio_rom.types import IModel, Key, RedisValue, Serializable
 
-from .fields import deserialize, serialize
-from .session import connection, transaction
-from .types import IModel, Key, RedisValue, Serializable
+if typing.TYPE_CHECKING:
+    from redis.asyncio.client import Pipeline, Redis
 
 T = TypeVar("T", bound=Serializable)
+M = TypeVar("M", bound=IModel)
 
 _generic_types_cache: dict[tuple[type[Any], Any | tuple[Any, ...]], type[Any]] = {}
 GenericCollectionT = TypeVar("GenericCollectionT", bound="GenericCollection")
 
 
 class GenericCollection:
     def __class_getitem__(
         cls: type[GenericCollectionT],
         params: type[Any] | tuple[type[Any], ...],
         **kwargs: Any,
     ) -> type[GenericCollectionT]:
-
         cached = _generic_types_cache.get((cls, params))
         if cached is not None:
             return cached
 
         if not isinstance(params, tuple):
             params = (params,)
 
         cls_dict = dict(cls.__dict__)
         cls_dict["item_class"] = params[0]
+        slots = cls_dict.pop("__slots__", None)
         generic_collection = type(cls.__name__, (cls,), cls_dict)
+        if slots:
+            generic_collection.__slots__ = slots  # type: ignore[attr-defined]
         _generic_types_cache[(cls, params[0])] = generic_collection
         return generic_collection
 
 
 class RedisCollection(
     Generic[T],
     GenericCollection,
     Collection[T],
     IModel,
     AsyncIterable[T],
     Iterable[T],
     metaclass=ABCMeta,
 ):
+    __slots__ = ("_values",)
+
     item_class: ClassVar[type]
 
     def __init__(self, values: Collection[T] | None = None, id: Key | None = None):
         self.id = id  # type: ignore[assignment]
         self.values = values
 
     @property
@@ -78,15 +85,15 @@
         if not self.id:
             raise AttributeError("id must be set")
         return super().db_id()
 
     @abstractmethod
     async def save_redis_values(
         self,
-        tr: Pipeline,
+        tr: Pipeline[str],
         values: Collection[Any],
     ) -> None:
         pass
 
     async def save(self, *, optimistic: bool = False, cascade: bool = False) -> None:
         if not self.values:
             return
@@ -97,36 +104,43 @@
         watch = [self.db_id()] if optimistic else []
         async with transaction(*watch) as tr:
             await tr.delete(self.db_id())
             await self.save_redis_values(tr, [serialize(v) for v in self.values])
             await tr.sadd(self.prefix(), self.id)
             if cascade:
                 await asyncio.gather(
-                    *[
+                    *(
                         v.save(optimistic=optimistic)
                         for v in self.values
                         if isinstance(v, IModel)
-                    ]
+                    )
                 )
 
     @classmethod
     async def get(cls: Type[RedisCollection[T]], id: Key) -> RedisCollection[T]:
-        return cls(id=id)
+        async with connection() as redis:
+            values = []
+            for value in await cls.get_redis_values(redis, f"{cls.prefix()}:{str(id)}"):
+                deserialized = deserialize(cls.item_class, value)
+                if isinstance(deserialized, IModel):
+                    await deserialized.refresh()
+                    deserialized = getattr(deserialized, "__wrapped__", deserialized)
+                values.append(deserialized)
+
+        return cls(id=id, values=values)
 
     async def refresh(self) -> None:
-        async with connection() as redis:
-            self.values = await asyncio.gather(
-                *[
-                    deserialize(self.item_class, value)
-                    for value in await self.get_redis_values(redis)
-                ]
-            )
+        fresh = await type(self).get(self.id)
+        self.values = fresh.values
 
+    @classmethod
     @abstractmethod
-    async def get_redis_values(self, redis: Redis) -> Collection[RedisValue]:
+    async def get_redis_values(
+        cls, redis: Redis[str], id: Key
+    ) -> Collection[RedisValue]:
         pass
 
     async def delete(self, cascade: bool = False) -> None:
         if not self.id:
             raise AttributeError("id must be set")
 
         async with transaction() as tr:
@@ -142,15 +156,15 @@
 
     def __iter__(self) -> Iterator[T]:
         return iter(self.values or [])
 
     def __repr__(self) -> str:
         return repr(self.values)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return self.values == (
             other.values if isinstance(other, RedisCollection) else other
         )
 
     def __contains__(self, item: Any) -> bool:
         return self.values is not None and item in self.values
 
@@ -158,19 +172,22 @@
 class RedisSet(RedisCollection[T], MutableSet[T]):
     @RedisCollection.values.setter  # type: ignore[attr-defined,misc]
     def values(self, values: Collection[T] | None) -> None:
         super(RedisSet, type(self)).values.fset(  # type: ignore[attr-defined]
             self, set(values) if values else set()
         )
 
-    async def get_redis_values(self, redis: Redis) -> Collection[RedisValue]:
-        return set(await redis.smembers(self.db_id()))
+    @classmethod
+    async def get_redis_values(
+        cls, redis: Redis[str], id: Key
+    ) -> Collection[RedisValue]:
+        return set(await redis.smembers(id))
 
     async def save_redis_values(
-        self, tr: Pipeline, values: Collection[RedisValue]
+        self, tr: Pipeline[str], values: Collection[RedisValue]
     ) -> None:
         await tr.sadd(self.db_id(), *values)
 
     async def async_add(
         self, value: T, optimistic: bool = False, cascade: bool = False
     ) -> None:
         async with connection() as conn:
@@ -189,43 +206,49 @@
     async def total_count(self) -> int:
         async with connection() as conn:
             return int(await conn.scard(self.db_id()))
 
     async def __aiter__(self) -> AsyncIterator[T]:
         async with connection() as conn:
             async for value in conn.sscan_iter(self.db_id()):
-                item = await deserialize(self.item_class, value)
+                item = deserialize(self.item_class, value)
+                if isinstance(item, IModel):
+                    await item.refresh()
+                    item = getattr(item, "__wrapped__", item)
                 self.add(item)
                 yield item
 
     def add(self, value: T) -> None:
         self.values.add(value)
 
     def discard(self, value: T) -> None:
         self.values.discard(value)
 
 
 class RedisList(RedisCollection[T], UserList):  # type: ignore[type-arg]
-    @property
-    def values(self) -> List[T]:
+    @property  # type: ignore[override]
+    def values(self) -> List[T] | None:
         return self.data
 
     @values.setter
     def values(self, values: Collection[T] | None) -> None:
         self.data = list(values) if values else []
 
-    async def get_redis_values(self, redis: Redis) -> Collection[RedisValue]:
-        return list(await redis.lrange(self.db_id(), 0, -1))
+    @classmethod
+    async def get_redis_values(
+        cls, redis: Redis[str], id: Key
+    ) -> Collection[RedisValue]:
+        return list(await redis.lrange(id, 0, -1))
 
     async def total_count(self) -> int:
         async with connection() as conn:
             return int(await conn.llen(self.db_id()))
 
     async def save_redis_values(
-        self, tr: Pipeline, values: Collection[RedisValue]
+        self, tr: Pipeline[str], values: Collection[RedisValue]
     ) -> None:
         await tr.rpush(self.db_id(), *values)
 
     async def async_append(
         self, value: T, optimistic: bool = False, cascade: bool = False
     ) -> None:
         async with connection() as conn:
@@ -234,10 +257,13 @@
                 await value.save(optimistic=optimistic)
         self.append(value)
 
     async def __aiter__(self) -> AsyncIterator[T]:
         async with connection() as conn:
             for index in range(0, await conn.llen(self.db_id())):
                 value = await conn.lindex(self.db_id(), index)
-                item = await deserialize(self.item_class, value)
-                self.insert(index, item)
+                item = deserialize(self.item_class, value)
+                if isinstance(item, IModel):
+                    await item.refresh()
+                    item = getattr(item, "__wrapped__", item)
+                self[index] = item
                 yield item
```

### Comparing `aio-rom-0.1.5/aio_rom/model.py` & `aio_rom-0.1.6/aio_rom/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,61 @@
 from __future__ import annotations
 
 import asyncio
 import logging
-from collections.abc import Iterable
-from operator import attrgetter
-from typing import Any, AsyncIterator, Awaitable, ClassVar, Type, TypeVar
-
-from .exception import ModelNotFoundException
-from .fields import Field, deserialize, fields, serialize_dict
-from .session import connection, transaction
-from .types import IModel, Key, RedisValue
+from typing import Any, AsyncIterator, Awaitable, ClassVar, Mapping, Type, TypeVar
+
+from aio_rom.exception import ModelNotFoundException
+from aio_rom.fields import deserialize, fields, serialize
+from aio_rom.session import connection, transaction
+from aio_rom.types import IModel, Key, RedisValue
 
 _logger = logging.getLogger(__name__)
 
 M = TypeVar("M", bound="Model")
 
 
 class Model(IModel):
     NotFoundException: ClassVar[Type[ModelNotFoundException]]
 
     @classmethod
     async def get(cls: type[M], id: Key) -> M:
         key = f"{cls.prefix()}:{str(id)}"
         async with connection() as conn:
-            db_item: dict[str, RedisValue] = await conn.hgetall(key)
+            db_item: Mapping[str, RedisValue] = await conn.hgetall(key)
 
         if not db_item:
             raise cls.NotFoundException(f"{key} not found")
 
-        model_fields = [
-            f for field_name, f in fields(cls).items() if field_name in db_item
-        ]
-
-        async def deserialize_field(field: Field, value: RedisValue) -> Any:
-            value = await deserialize(field.type, value)
-            if isinstance(value, IModel) and field.eager:
+        deserialized = {}
+        for f in [f for f in fields(cls).values() if f.name in db_item]:
+            value = deserialize(f.field_type, db_item[f.name])
+            if f.eager and isinstance(value, IModel):
                 await value.refresh()
-            return value
+                value = getattr(value, "__wrapped__", value)
+            deserialized[f.name] = value
 
-        deserialized = await asyncio.gather(
-            *(deserialize_field(f, db_item[f.name]) for f in model_fields)
-        )
-
-        return cls(**dict(zip(map(attrgetter("name"), model_fields), deserialized)))
+        return cls(**deserialized)
 
     @classmethod
     async def scan(cls: type[M], **kwargs: str | None | int | None) -> AsyncIterator[M]:
         async with connection() as conn:
-            found = set()
-            async for key in conn.sscan_iter(cls.prefix(), **kwargs):  # type: ignore[arg-type] # noqa
-                if key not in found:
-                    value = await cls.get(key)
-                    if value:
-                        yield value
-                        found.add(key)
-                    else:
-                        _logger.warning(f"{cls.__name__} Key: {key} orphaned")
+            async for key in conn.sscan_iter(
+                cls.prefix(), **kwargs  # type: ignore[arg-type]
+            ):
+                try:
+                    yield await cls.get(key)
+                except cls.NotFoundException:
+                    _logger.warning(f"{cls.__name__} Key: {key} orphaned")
 
     @classmethod
-    async def all(cls: type[M]) -> Iterable[M]:
+    async def all(cls: type[M]) -> list[M]:
         async with connection() as conn:
             keys = await conn.smembers(cls.prefix())
-            return await asyncio.gather(*[cls.get(key) for key in keys])
+            return list(await asyncio.gather(*[cls.get(key) for key in keys]))
 
     @classmethod
     async def total_count(cls) -> int:
         async with connection() as conn:
             return int(await conn.scard(cls.prefix()))
 
     async def save(self, *, optimistic: bool = False, cascade: bool = False) -> None:
@@ -73,45 +63,43 @@
         async with transaction(*watch) as tr:
             await self.update(optimistic=optimistic)
             await tr.sadd(self.prefix(), self.id)
 
     async def update(self, optimistic: bool = False, **changes: Any) -> None:
         model_fields = fields(self)
         for name, value in changes.items():
-            setattr(self, name, value)
+            if name in model_fields:
+                setattr(self, name, value)
 
-        values = {
-            field_name: getattr(self, field_name)
+        values = [
+            (field_name, getattr(self, field_name))
             for field_name, f in model_fields.items()
             if (not changes or field_name in changes)
-        }
+        ]
 
-        model_dict = serialize_dict(
-            {
-                k: v
-                for k, v in values.items()
-                if not (model_fields[k].optional and v is None)
-            }
-        )
-        watch = [self.db_id()] if optimistic else []
+        model_dict = {
+            k: serialize(v)
+            for k, v in values
+            if not (model_fields[k].optional and v is None)
+        }
         operations: list[Awaitable[None]] = [
             value.save(optimistic=optimistic, cascade=model_fields[field_name].cascade)
-            for field_name, value in values.items()
+            for field_name, value in values
             if isinstance(value, IModel)
         ]
         keys_to_delete = [k for k, v in model_dict.items() if v is None]
-        async with transaction(*watch) as tr:
+        update_mapping = {k: v for k, v in model_dict.items() if v is not None}
+        async with transaction(*([self.db_id()] if optimistic else [])) as tr:
             if keys_to_delete:
                 operations.append(tr.hdel(self.db_id(), *keys_to_delete))
-            update_mapping = {k: v for k, v in model_dict.items() if v is not None}
             if update_mapping:
                 operations.append(
                     tr.hset(
                         self.db_id(),
-                        mapping=update_mapping,
+                        mapping=update_mapping,  # type: ignore[arg-type]
                     )
                 )
             if operations:
                 await asyncio.gather(*operations)
 
     async def delete(self, _: bool = False) -> None:
         key = self.db_id()
@@ -124,11 +112,10 @@
     async def refresh(self: M) -> None:
         fresh = await type(self).get(self.id)
         for name, field in fields(self).items():
             if not field.transient:
                 setattr(self, name, getattr(fresh, name))
 
     def __setattr__(self, key: str, value: Any) -> None:
-        model_fields = fields(self)
         if isinstance(value, IModel) and not value.id:
-            value.id = f"{self.db_id()}:{model_fields[key].name}"
+            value.id = f"{self.db_id()}:{key}"
         super().__setattr__(key, value)
```

### Comparing `aio-rom-0.1.5/aio_rom/session.py` & `aio_rom-0.1.6/aio_rom/session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
 from contextvars import ContextVar
 from typing import TYPE_CHECKING, Any, AsyncIterator
 
-from aioredis import ConnectionPool, Redis
-from aioredis.client import Pipeline
+from redis.asyncio import Redis
 
 if TYPE_CHECKING:
+    from redis.asyncio.client import Pipeline
+
     from aio_rom.types import Key
 
-POOL: ContextVar[ConnectionPool | None] = ContextVar("pool", default=None)
-CONNECTION: ContextVar[Redis | None] = ContextVar("connection", default=None)
-TRANSACTION: ContextVar[Pipeline | None] = ContextVar("transaction", default=None)
+REDIS_CLIENT: ContextVar[Redis[str] | None] = ContextVar("redis_client", default=None)
+CONNECTION: ContextVar[Redis[str] | None] = ContextVar("connection", default=None)
+TRANSACTION: ContextVar[Pipeline[str] | None] = ContextVar("transaction", default=None)
 
 config: dict[str, Any] = {}
 
 
 def configure(address: str | None = None, *args: Any, **kwargs: Any) -> None:
     global config
     config["address"] = address
     config["args"] = args
     config["kwargs"] = kwargs
 
 
 @asynccontextmanager
-async def redis_pool(
+async def redis_client(
     address: str | None = None, **kwargs: Any
-) -> AsyncIterator[ConnectionPool]:
-    pool = POOL.get()
-    if pool:
-        yield pool
+) -> AsyncIterator[Redis[str]]:
+    client: Redis[str] | None = REDIS_CLIENT.get()
+    if client:
+        yield client
         return
-    pool = ConnectionPool.from_url(
+    client = Redis.from_url(
         address if address else config.get("address", "redis://localhost"),
         encoding="utf-8",
         decode_responses=True,
         **kwargs if kwargs else config.get("kwargs", {}),
     )
-    t = POOL.set(pool)
+    if not client:
+        raise ValueError("Failed to initialize Redis client")
+    t = REDIS_CLIENT.set(client)
     try:
-        yield pool
+        yield client
     finally:
-        await pool.disconnect()
-        POOL.reset(t)
+        await client.close()
+        REDIS_CLIENT.reset(t)
 
 
 @asynccontextmanager
-async def connection(address: str | None = None, **kwargs: Any) -> AsyncIterator[Redis]:
+async def connection(
+    address: str | None = None, **kwargs: Any
+) -> AsyncIterator[Redis[str]]:
     connection = CONNECTION.get()
     if connection:
         yield connection
         return
 
-    async with redis_pool(address, **kwargs) as pool:
-        async with Redis(single_connection_client=True, connection_pool=pool) as redis:
-            t = CONNECTION.set(redis)
-            try:
-                yield redis
-            finally:
-                CONNECTION.reset(t)
+    async with redis_client(address, **kwargs) as pool:
+        redis = await pool.client()
+        t = CONNECTION.set(redis)
+        try:
+            yield redis
+        finally:
+            CONNECTION.reset(t)
+            await redis.close(close_connection_pool=True)
 
 
 @asynccontextmanager
-async def transaction(*watches: Key) -> AsyncIterator[Pipeline]:
+async def transaction(*watches: Key) -> AsyncIterator[Pipeline[str]]:
     transaction = TRANSACTION.get()
     if transaction:
         yield transaction
         return
 
-    async with connection() as conn:
-        async with conn.pipeline() as tr:
-            keys = [str(key) if isinstance(key, int) else key for key in watches]
-            if keys:
-                await tr.watch(*keys)
-            tr.multi()  # type: ignore[no-untyped-call]
-            t = TRANSACTION.set(tr)
+    async with connection() as conn, conn.pipeline(transaction=True) as tr:
+        if watches:
+            await tr.watch(*watches)
+        tr.multi()
+        t = TRANSACTION.set(tr)
+        try:
+            yield tr
+        finally:
             try:
-                yield tr
+                await tr.execute()
             finally:
-                try:
-                    await tr.execute()
-                finally:
-                    TRANSACTION.reset(t)
+                TRANSACTION.reset(t)
```

### Comparing `aio-rom-0.1.5/aio_rom/types.py` & `aio_rom-0.1.6/aio_rom/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
-from abc import ABC
+from abc import ABC, abstractmethod
 from typing import Any, ClassVar, Optional, Type, TypeVar, Union
 
-from aioredis.client import FieldT, KeyT
+from redis.typing import FieldT, KeyT
+from typing_extensions import TypeAlias
 
 from aio_rom.exception import ModelNotFoundException
 from aio_rom.session import connection
 
-Key = KeyT
 T = TypeVar("T", bound="IModel")
 
 
 class IModel(ABC):
+    __slots__ = ("id",)
+
     NotFoundException: ClassVar[Type[ModelNotFoundException]]
     id: Key
 
     @classmethod
     def prefix(cls) -> str:
         return f"{cls.__name__.lower()}"
 
     def __init_subclass__(cls: type[T], **kwargs: Any) -> None:
         cls.NotFoundException = type("NotFoundException", (ModelNotFoundException,), {})
 
     def db_id(self) -> str:
         return f"{self.prefix()}:{str(self.id)}"
 
+    @abstractmethod
     async def save(self, *, optimistic: bool = False, cascade: bool = False) -> None:
         ...
 
     @classmethod
+    @abstractmethod
     async def get(cls: type[T], id: Key) -> T:
         ...
 
     @classmethod
     async def persisted(cls: type[T], id: int) -> bool:
         async with connection() as conn:
             return bool(await conn.exists(f"{cls.prefix()}:{id}"))
@@ -41,24 +45,30 @@
     @classmethod
     async def delete_all(cls: type[T]) -> None:
         key_prefix = cls.prefix()
         async with connection() as conn:
             keys = await conn.keys(f"{key_prefix}:*")
             await conn.delete(key_prefix, *keys)
 
+    @abstractmethod
     async def total_count(self) -> int:
         ...
 
+    @abstractmethod
     async def delete(self, cascade: bool = False) -> None:
         ...
 
     async def exists(self) -> bool:
         async with connection() as conn:
             return bool(await conn.exists(self.db_id()))
 
-    async def refresh(self: T) -> None:
+    @abstractmethod
+    async def refresh(self) -> None:
         ...
 
 
-RedisValue = FieldT
+Key: TypeAlias = KeyT
+RedisValue: TypeAlias = FieldT
 Serializable = Union[RedisValue, IModel]
 Serialized = Optional[RedisValue]
+
+__all__ = ["IModel", "Key", "RedisValue", "Serializable", "Serialized"]
```

### Comparing `aio-rom-0.1.5/aio_rom/utils.pyi` & `aio_rom-0.1.6/aio_rom/utils.pyi`

 * *Files identical despite different names*

### Comparing `aio-rom-0.1.5/pyproject.toml` & `aio_rom-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-[tool.poetry]
+[project]
 name = "aio-rom"
-version = "0"
+dynamic = ["version"]
 description = "asyncio based Redis object mapper"
-authors = ["Federico Jaite <fede_654_87@hotmail.com>"]
+authors = [{ name = "fedej", email = "fede_654_87@hotmail.com" }]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "aio_rom"}]
-repository = "https://github.com/fedej/aio-rom"
+requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -18,99 +17,117 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Database :: Front-Ends",
 ]
-include = ["aio_rom/py.typed"]
+dependencies = [
+    "typing-extensions>=4.4.0,<5.0",
+    "redis>=4.3.4,<4.6.0",
+    "wrapt>=1.14.1",
+]
+
+[project.urls]
+"Source" = "https://github.com/fedej/aio-rom"
 
-[tool.poetry.dependencies]
-python = "^3.7"
-aioredis = "2.0.1"
-typing-extensions = ">=4.0.1,<5.0"
-
-[tool.poetry.dev-dependencies]
-black = "^22.1"
-flake8 = "^4.0.1"
-mypy = "^0.931"
-pytest = "^6.2.5"
-pytest-benchmark = "^3.4.1"
-isort = "^5.9.3"
-bandit = "^1.7.2"
-flake8-bugbear = "^22.1.11"
-flake8-comprehensions = "^3.8.0"
+[project.optional-dependencies]
+dev = [
+    "bandit",
+    "black",
+    "flake8",
+    "flake8-bugbear",
+    "flake8-comprehensions",
+    "isort",
+    "mypy",
+    "pytest",
+    "pytest-asyncio",
+    "pytest-benchmark"
+]
 
-[tool.poetry-version-plugin]
-source = "git-tag"
+[tool.hatch.version]
+source = "vcs"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.run]
 relative_files = true
+branch = true
+source_pkgs = ["aio_rom", "tests"]
+
+[tool.coverage.paths]
+aio_rom = ["aio_rom"]
+tests = ["tests"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "no cov",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+]
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
+[tool.hatch.envs.default]
+dependencies = [
+    "asynctest;python_version<'3.8'",
+    "pytest",
+    "pytest-asyncio",
+    "pytest-benchmark",
+    "pytest-cov",
+]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-minversion = 3.7
-isolated_build = true
-envlist =
-    clean
-    style
-    mypy
-    py{37,38,39,310},pypy3
-skip_missing_interpreters = true
-
-[gh-actions]
-python =
-    3.7: clean, py37, style
-    3.8: clean, py38, mypy
-    3.9: clean, py39
-    3.10: clean, py310
-    pypy-3: clean, pypy3
-
-[testenv]
-deps =
-    asynctest; python_version < "3.8"
-    pytest
-    pytest-cov
-    pytest-benchmark
-passenv = CI
-extras = mypy
-setenv = MYPY_TEST_PREFIX = tests
-commands = pytest --cov=aio_rom --cov-append --cov-report=term-missing --cov-branch --cov-report=xml
-
-[testenv:pypy3]
-extras =
-setenv =
-commands = {[testenv]commands} --ignore-glob='*mypy*.py'
-
-[testenv:style]
-deps =
-    black
-    flake8
-    flake8-bugbear
-    flake8-comprehensions
-    bandit
-    isort
-commands =
-    black --check .
-    flake8 --max-line-length=88 --ignore=E203,W503,B950 --select=E,W,F,C9,N8,B,B9,C4 .
-    bandit -r aio_rom
-    isort --check-only .
-
-[testenv:mypy]
-deps =
-    mypy
-    pytest
-commands = mypy --install-types --non-interactive --strict aio_rom tests
-
-[testenv:clean]
-deps = coverage[toml]
-skip_install = true
-commands = coverage erase
-"""
+[tool.hatch.envs.default.scripts]
+no-cov = "pytest --no-cov {args:tests}"
+cov = "pytest --cov --cov-report=term-missing --cov-config=pyproject.toml {args:tests}"
+
+[[tool.hatch.envs.test.matrix]]
+python = ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"]
+
+[tool.hatch.envs.coverage]
+detached = true
+dependencies = [
+    "coverage[toml]",
+    "lxml",
+]
+[tool.hatch.envs.coverage.scripts]
+combine = "coverage combine {args}"
+report-xml = "coverage xml"
+
+[tool.hatch.envs.lint]
+detached = true
+dependencies = [
+    "bandit",
+    "black",
+    "flake8",
+    "flake8-bugbear",
+    "flake8-comprehensions",
+    "isort",
+    "mypy",
+    "pytest",
+]
+
+[tool.hatch.envs.lint.scripts]
+fmt = [
+    "black {args:.}",
+    "isort {args:.}",
+]
+style = [
+    "black --check {args:.}",
+    "isort --check-only {args:.}",
+]
+lint = [
+    "flake8 --max-line-length=88 --ignore=E203,W503,B950 --select=E,W,F,C9,N8,B,B9,C4 {args:aio_rom tests}",
+    "bandit -r {args:aio_rom}",
+]
+typing = "mypy --install-types --ignore-missing-imports --non-interactive --strict {args:.}"
+all = [
+    "style",
+    "lint",
+    "typing"
+]
```

### Comparing `aio-rom-0.1.5/PKG-INFO` & `aio_rom-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: aio-rom
-Version: 0.1.5
+Version: 0.1.6
 Summary: asyncio based Redis object mapper
-Home-page: https://github.com/fedej/aio-rom
-License: MIT
-Author: Federico Jaite
-Author-email: fede_654_87@hotmail.com
-Requires-Python: >=3.7,<4.0
+Project-URL: Source, https://github.com/fedej/aio-rom
+Author-email: fedej <fede_654_87@hotmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database :: Front-Ends
-Requires-Dist: aioredis (==2.0.1)
-Requires-Dist: typing-extensions (>=4.0.1,<5.0)
-Project-URL: Repository, https://github.com/fedej/aio-rom
+Requires-Python: >=3.7
+Requires-Dist: redis<4.6.0,>=4.3.4
+Requires-Dist: typing-extensions<5.0,>=4.4.0
+Requires-Dist: wrapt>=1.14.1
+Provides-Extra: dev
+Requires-Dist: bandit; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: flake8-bugbear; extra == 'dev'
+Requires-Dist: flake8-comprehensions; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
+Requires-Dist: pytest-benchmark; extra == 'dev'
 Description-Content-Type: text/markdown
 
 Python Redis Object Mapper
 ======================
 
 asyncio based Redis object mapper
 
@@ -89,8 +95,7 @@
 1. Tests
 
 ## Limitations
 1. `configure` must be called before other calls to Redis can succeed, no defaults to localhost atm.
 1. You cannot use `from __future__ import annotations` in the same file you define your models. See https://bugs.python.org/issue39442
 1. TODO Supported datatypes
 1. Probably more ...
-
```

