# Comparing `tmp/fudgeo-0.3.9-py3-none-any.whl.zip` & `tmp/fudgeo-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,19 @@
-Zip file size: 19764 bytes, number of entries: 12
--rw-r--r--  2.0 unx      117 b- defN 23-Mar-28 23:34 fudgeo/__init__.py
--rw-r--r--  2.0 unx     2457 b- defN 23-Mar-12 04:11 fudgeo/constant.py
+Zip file size: 24813 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      117 b- defN 23-May-06 22:44 fudgeo/__init__.py
+-rw-r--r--  2.0 unx     2538 b- defN 23-May-06 22:16 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
--rw-r--r--  2.0 unx    62026 b- defN 23-Mar-12 04:11 fudgeo/geometry.py
--rw-r--r--  2.0 unx    17613 b- defN 23-Mar-28 23:35 fudgeo/geopkg.py
--rw-r--r--  2.0 unx     2795 b- defN 23-Mar-12 04:11 fudgeo/geopkg.sql
--rw-r--r--  2.0 unx     7506 b- defN 23-Mar-28 18:25 fudgeo/sql.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     9095 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      901 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/RECORD
-12 files, 104854 bytes uncompressed, 18280 bytes compressed:  82.6%
+-rw-r--r--  2.0 unx    20081 b- defN 23-May-06 13:55 fudgeo/geopkg.py
+-rw-r--r--  2.0 unx     2673 b- defN 23-May-06 13:55 fudgeo/geopkg.sql
+-rw-r--r--  2.0 unx     7768 b- defN 23-May-06 13:55 fudgeo/sql.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-06 22:16 fudgeo/geometry/__init__.py
+-rw-r--r--  2.0 unx     3244 b- defN 23-May-06 22:31 fudgeo/geometry/base.py
+-rw-r--r--  2.0 unx    14233 b- defN 23-May-06 22:16 fudgeo/geometry/linestring.py
+-rw-r--r--  2.0 unx    16511 b- defN 23-May-06 22:16 fudgeo/geometry/point.py
+-rw-r--r--  2.0 unx    18766 b- defN 23-May-06 22:16 fudgeo/geometry/polygon.py
+-rw-r--r--  2.0 unx     6508 b- defN 23-May-06 22:16 fudgeo/geometry/util.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-06 22:44 fudgeo-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9095 b- defN 23-May-06 22:44 fudgeo-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 22:44 fudgeo-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-06 22:44 fudgeo-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1321 b- defN 23-May-06 22:44 fudgeo-0.4.0.dist-info/RECORD
+17 files, 106173 bytes uncompressed, 22681 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -3,35 +3,50 @@
 
 Filename: fudgeo/constant.py
 Comment: 
 
 Filename: fudgeo/enumeration.py
 Comment: 
 
-Filename: fudgeo/geometry.py
-Comment: 
-
 Filename: fudgeo/geopkg.py
 Comment: 
 
 Filename: fudgeo/geopkg.sql
 Comment: 
 
 Filename: fudgeo/sql.py
 Comment: 
 
-Filename: fudgeo-0.3.9.dist-info/LICENSE
+Filename: fudgeo/geometry/__init__.py
+Comment: 
+
+Filename: fudgeo/geometry/base.py
+Comment: 
+
+Filename: fudgeo/geometry/linestring.py
+Comment: 
+
+Filename: fudgeo/geometry/point.py
+Comment: 
+
+Filename: fudgeo/geometry/polygon.py
+Comment: 
+
+Filename: fudgeo/geometry/util.py
+Comment: 
+
+Filename: fudgeo-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.3.9.dist-info/METADATA
+Filename: fudgeo-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.3.9.dist-info/WHEEL
+Filename: fudgeo-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.3.9.dist-info/top_level.txt
+Filename: fudgeo-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.3.9.dist-info/RECORD
+Filename: fudgeo-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.3.9'
+__version__ = '0.4.0'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/constant.py

```diff
@@ -69,13 +69,14 @@
     (True, False): WKB_POINT_Z_PRE,
     (False, True): WKB_POINT_M_PRE,
     (True, True): WKB_POINT_ZM_PRE,
 }
 
 
 HEADER_OFFSET: int = 8
-ENVELOPE_OFFSET: Dict[int, int] = {0: 0, 1: 32, 2: 48, 3: 48, 4: 64}
-ENVELOPE_OFFSET = {k: v + HEADER_OFFSET for k, v in ENVELOPE_OFFSET.items()}
+ENVELOPE_LENGTH: Dict[int, int] = {0: 0, 1: 32, 2: 48, 3: 48, 4: 64}
+ENVELOPE_COUNT: Dict[int, int] = {k: v // 8 for k, v in ENVELOPE_LENGTH.items()}
+ENVELOPE_OFFSET = {k: v + HEADER_OFFSET for k, v in ENVELOPE_LENGTH.items()}
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geopkg.py

```diff
@@ -4,45 +4,58 @@
 """
 
 
 from datetime import datetime, timedelta, timezone
 from math import nan
 from os import PathLike
 from pathlib import Path
+from re import IGNORECASE, compile as recompile
 from sqlite3 import (
-    Connection, Cursor, PARSE_COLNAMES, PARSE_DECLTYPES, connect,
-    register_adapter, register_converter)
-from typing import Dict, List, Optional, Tuple, Type, Union
+    Connection, Cursor, DatabaseError, OperationalError, PARSE_COLNAMES,
+    PARSE_DECLTYPES, connect, register_adapter, register_converter)
+from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 
 from fudgeo.enumeration import (
     DataType, GPKGFlavors, GeometryType, SQLFieldType)
 from fudgeo.geometry import (
     Point, PointZ, PointM, PointZM, MultiPoint, MultiPointZ, MultiPointM,
     MultiPointZM, LineString, LineStringZ, LineStringM, LineStringZM,
     MultiLineString, MultiLineStringZ, MultiLineStringM, MultiLineStringZM,
     Polygon, PolygonZ, PolygonM, PolygonZM, MultiPolygon, MultiPolygonZ,
     MultiPolygonM, MultiPolygonZM)
 from fudgeo.sql import (
-    CHECK_SRS_EXISTS, CREATE_FEATURE_TABLE, CREATE_TABLE, DEFAULT_EPSG_RECS,
-    DEFAULT_ESRI_RECS, GPKG_OGR_CONTENTS_DELETE_TRIGGER,
-    GPKG_OGR_CONTENTS_INSERT_TRIGGER, INSERT_GPKG_CONTENTS_SHORT,
-    INSERT_GPKG_GEOM_COL, INSERT_GPKG_OGR_CONTENTS, INSERT_GPKG_SRS, KEYWORDS,
-    REMOVE_FEATURE_CLASS, REMOVE_TABLE, SELECT_EXTENT, SELECT_GEOMETRY_COLUMN,
-    SELECT_GEOMETRY_TYPE, SELECT_HAS_ZM, SELECT_SRS, SELECT_TABLES_BY_TYPE,
-    TABLE_EXISTS, UPDATE_EXTENT)
+    CHECK_SRS_EXISTS, CREATE_FEATURE_TABLE, CREATE_OGR_CONTENTS, CREATE_TABLE,
+    DEFAULT_EPSG_RECS, DEFAULT_ESRI_RECS, DELETE_OGR_CONTENTS,
+    GPKG_OGR_CONTENTS_DELETE_TRIGGER, GPKG_OGR_CONTENTS_INSERT_TRIGGER,
+    HAS_OGR_CONTENTS, INSERT_GPKG_CONTENTS_SHORT, INSERT_GPKG_GEOM_COL,
+    INSERT_GPKG_OGR_CONTENTS, INSERT_GPKG_SRS, KEYWORDS, REMOVE_FEATURE_CLASS,
+    REMOVE_TABLE, SELECT_EXTENT, SELECT_GEOMETRY_COLUMN, SELECT_GEOMETRY_TYPE,
+    SELECT_HAS_ZM, SELECT_SRS, SELECT_TABLES_BY_TYPE, TABLE_EXISTS,
+    UPDATE_EXTENT)
 
 
 FIELDS = Union[Tuple['Field', ...], List['Field']]
+NAME_MATCHER: Callable = recompile(r'^[A-Z]\w*$', IGNORECASE).match
 
 
 COMMA_SPACE = ', '
 GPKG_EXT = '.gpkg'
 SHAPE = 'SHAPE'
 
 
+def _escape_name(name: str) -> str:
+    """
+    Escape Name
+    """
+    if name.upper() in KEYWORDS or not NAME_MATCHER(name):
+        name = f'"{name}"'
+    return name
+# End _escape_name function
+
+
 def _now() -> str:
     """
     Formatted Now
     """
     return datetime.now().strftime('%Y-%m-%dT%H:%M:%S.%fZ')
 # End _now method
 
@@ -123,14 +136,21 @@
         Initialize the GeoPackage class
         """
         super().__init__()
         self._path: Path = Path(path)
         self._conn: Optional[Connection] = None
     # End init built-in
 
+    def __repr__(self) -> str:
+        """
+        String Representation
+        """
+        return f'GeoPackage(path={self._path!r})'
+    # End repr built-in
+
     @property
     def path(self) -> Path:
         """
         Path
         """
         return self._path
     # End path property
@@ -148,15 +168,16 @@
             register_converter('timestamp', _convert_datetime)
             register_converter('datetime', _convert_datetime)
         return self._conn
     # End connection property
 
     @classmethod
     def create(cls, path: Union[PathLike, str],
-               flavor: str = GPKGFlavors.esri) -> 'GeoPackage':
+               flavor: str = GPKGFlavors.esri,
+               ogr_contents: bool = True) -> 'GeoPackage':
         """
         Create a new GeoPackage
         """
         path = Path(path).with_suffix(GPKG_EXT)
         if path.is_file():
             raise ValueError(f'GeoPackage already exists: {path}')
         if not path.parent.is_dir():
@@ -165,14 +186,16 @@
             defaults = DEFAULT_ESRI_RECS
         else:
             defaults = DEFAULT_EPSG_RECS
         with connect(str(path), isolation_level='EXCLUSIVE') as conn:
             with Path(__file__).parent.joinpath('geopkg.sql').open() as fin:
                 conn.executescript(fin.read())
             conn.executemany(INSERT_GPKG_SRS, defaults)
+            if ogr_contents:
+                conn.execute(CREATE_OGR_CONTENTS)
         return cls(path)
     # End create method
 
     def check_srs_exists(self, srs_id: int) -> bool:
         """
         Check if a SpatialReferenceSystem already exists in the table.
         This is done purely by srs id because that is all ESRI looks at.
@@ -267,20 +290,28 @@
         """
         super().__init__()
         self.geopackage: GeoPackage = geopackage
         self.name: str = name
     # End init built-in
 
     @property
+    def escaped_name(self) -> str:
+        """
+        Escaped Name
+        """
+        return _escape_name(self.name)
+    # End escaped_name property
+
+    @property
     def fields(self) -> List['Field']:
         """
         Fields
         """
         cursor = self.geopackage.connection.execute(
-            f"""PRAGMA table_info({self.name})""")
+            f"""PRAGMA table_info({self.escaped_name})""")
         return [Field(name=name, data_type=type_)
                 for _, name, type_, _, _, _ in cursor.fetchall()]
     # End fields property
 
     @property
     def field_names(self) -> List[str]:
         """
@@ -291,81 +322,110 @@
 # End BaseTable class
 
 
 class Table(BaseTable):
     """
     GeoPackage Table
     """
+    def __repr__(self) -> str:
+        """
+        String Representation
+        """
+        return f'Table(geopackage={self.geopackage!r}, name={self.name!r})'
+    # End repr built-in
+
     @classmethod
     def create(cls, geopackage: GeoPackage, name: str, fields: FIELDS,
                description: str = '', overwrite: bool = False) -> 'Table':
         """
         Create a regular non-spatial table in the geopackage
         """
         cols = f', {", ".join(repr(f) for f in fields)}' if fields else ''
         with geopackage.connection as conn:
+            escaped_name = _escape_name(name)
+            has_ogr_contents = _has_ogr_contents(conn)
             if overwrite:
-                conn.executescript(REMOVE_TABLE.format(name))
-            conn.execute(CREATE_TABLE.format(name=name, other_fields=cols))
+                conn.executescript(REMOVE_TABLE.format(name, escaped_name))
+                if has_ogr_contents:
+                    conn.execute(DELETE_OGR_CONTENTS.format(name))
+            conn.execute(CREATE_TABLE.format(
+                name=escaped_name, other_fields=cols))
             conn.execute(INSERT_GPKG_CONTENTS_SHORT, (
                 name, DataType.attributes, name, description, _now(), None))
-            conn.execute(INSERT_GPKG_OGR_CONTENTS, (name, 0))
-            conn.execute(GPKG_OGR_CONTENTS_INSERT_TRIGGER.format(name))
-            conn.execute(GPKG_OGR_CONTENTS_DELETE_TRIGGER.format(name))
+            if has_ogr_contents:
+                _add_ogr_contents(conn, name=name, escaped_name=escaped_name)
         return cls(geopackage=geopackage, name=name)
-    # End create_table method
+    # End create method
 
     def drop(self) -> None:
         """
         Drop table from Geopackage
         """
         with self.geopackage.connection as conn:
-            conn.executescript(REMOVE_TABLE.format(self.name))
+            conn.executescript(
+                REMOVE_TABLE.format(self.name, self.escaped_name))
+            if _has_ogr_contents(conn):
+                conn.execute(DELETE_OGR_CONTENTS.format(self.name))
     # End drop method
 # End Table class
 
 
 class FeatureClass(BaseTable):
     """
     GeoPackage Feature Class
     """
+    def __repr__(self) -> str:
+        """
+        String Representation
+        """
+        return (f'FeatureClass(geopackage={self.geopackage!r}, '
+                f'name={self.name!r})')
+    # End repr built-in
+
     @classmethod
     def create(cls, geopackage: GeoPackage, name: str, shape_type: str,
                srs: 'SpatialReferenceSystem', z_enabled: bool = False,
                m_enabled: bool = False, fields: FIELDS = (),
                description: str = '',
                overwrite: bool = False) -> 'FeatureClass':
         """
         Create Feature Class
         """
         cols = f', {", ".join(repr(f) for f in fields)}' if fields else ''
         with geopackage.connection as conn:
+            escaped_name = _escape_name(name)
+            has_ogr_contents = _has_ogr_contents(conn)
             if overwrite:
-                conn.executescript(REMOVE_FEATURE_CLASS.format(name))
+                conn.executescript(
+                    REMOVE_FEATURE_CLASS.format(name, escaped_name))
+                if has_ogr_contents:
+                    conn.execute(DELETE_OGR_CONTENTS.format(name))
             conn.execute(CREATE_FEATURE_TABLE.format(
-                name=name, feature_type=shape_type, other_fields=cols))
+                name=escaped_name, feature_type=shape_type, other_fields=cols))
             if not geopackage.check_srs_exists(srs.srs_id):
                 conn.execute(INSERT_GPKG_SRS, srs.as_record())
             conn.execute(INSERT_GPKG_GEOM_COL,
                          (name, SHAPE, shape_type, srs.srs_id,
                           int(z_enabled), int(m_enabled)))
             conn.execute(INSERT_GPKG_CONTENTS_SHORT, (
                 name, DataType.features, name, description, _now(), srs.srs_id))
-            conn.execute(INSERT_GPKG_OGR_CONTENTS, (name, 0))
-            conn.execute(GPKG_OGR_CONTENTS_INSERT_TRIGGER.format(name))
-            conn.execute(GPKG_OGR_CONTENTS_DELETE_TRIGGER.format(name))
+            if has_ogr_contents:
+                _add_ogr_contents(conn, name=name, escaped_name=escaped_name)
         return cls(geopackage=geopackage, name=name)
     # End create method
 
     def drop(self) -> None:
         """
         Drop feature class from Geopackage
         """
         with self.geopackage.connection as conn:
-            conn.executescript(REMOVE_FEATURE_CLASS.format(self.name))
+            conn.executescript(
+                REMOVE_FEATURE_CLASS.format(self.name, self.escaped_name))
+            if _has_ogr_contents(conn):
+                conn.execute(DELETE_OGR_CONTENTS.format(self.name))
     # End drop method
 
     @staticmethod
     def _check_result(cursor: Cursor) -> Optional[str]:
         """
         Check Result
         """
@@ -512,27 +572,46 @@
     # End init built-in
 
     @property
     def escaped_name(self) -> str:
         """
         Escaped Name, only adds quotes if needed
         """
-        name = self.name
-        if name.upper() in KEYWORDS:
-            name = f'"{name}"'
-        return name
+        return _escape_name(self.name)
     # End escaped_name property
 
     def __repr__(self) -> str:
         """
         String representation
         """
         types = SQLFieldType.blob, SQLFieldType.text
         if self.size and self.data_type in types:
             return f'{self.escaped_name} {self.data_type}{self.size}'
         return f'{self.escaped_name} {self.data_type}'
     # End repr built-in
 # End Field class
 
 
+def _has_ogr_contents(conn: 'Connection') -> bool:
+    """
+    Has gpkg_ogr_contents table
+    """
+    try:
+        cursor = conn.execute(HAS_OGR_CONTENTS)
+    except (DatabaseError, OperationalError):
+        return False
+    return bool(cursor.fetchone())
+# End _has_ogr_contents function
+
+
+def _add_ogr_contents(conn: Connection, name: str, escaped_name: str) -> None:
+    """
+    Add OGR Contents Table Entry and Triggers
+    """
+    conn.execute(INSERT_GPKG_OGR_CONTENTS, (name, 0))
+    conn.execute(GPKG_OGR_CONTENTS_INSERT_TRIGGER.format(name, escaped_name))
+    conn.execute(GPKG_OGR_CONTENTS_DELETE_TRIGGER.format(name, escaped_name))
+# End _add_ogr_contents function
+
+
 if __name__ == '__main__':
     pass
```

## fudgeo/geopkg.sql

```diff
@@ -74,13 +74,7 @@
     table_name     TEXT,
     column_name    TEXT,
     extension_name TEXT NOT NULL,
     definition     TEXT NOT NULL,
     scope          TEXT NOT NULL,
     CONSTRAINT ge_tce UNIQUE (table_name, column_name, extension_name)
 );
-
-
-CREATE TABLE gpkg_ogr_contents (
-    table_name    TEXT NOT NULL PRIMARY KEY,
-    feature_count INTEGER DEFAULT NULL
-);
```

## fudgeo/sql.py

```diff
@@ -38,44 +38,61 @@
 
 
 INSERT_GPKG_OGR_CONTENTS: str = """
     INSERT INTO gpkg_ogr_contents (table_name, feature_count) VALUES (?, ?)
 """
 
 
-REMOVE_FEATURE_CLASS: str = """
+CREATE_OGR_CONTENTS: str = """
+    CREATE TABLE gpkg_ogr_contents (
+        table_name    TEXT NOT NULL PRIMARY KEY,
+        feature_count INTEGER DEFAULT NULL
+    );
+"""
+
+
+HAS_OGR_CONTENTS: str = """
+    SELECT name FROM sqlite_master 
+    WHERE type = 'table' AND name = 'gpkg_ogr_contents'
+"""
+
+
+DELETE_OGR_CONTENTS: str = """
     DELETE FROM gpkg_ogr_contents WHERE lower(table_name) = lower('{0}');
+"""
+
+
+REMOVE_FEATURE_CLASS: str = """
     DELETE FROM gpkg_contents WHERE lower(table_name) = lower('{0}');
     DELETE FROM gpkg_geometry_columns WHERE lower(table_name) = lower('{0}');
     DROP TRIGGER IF EXISTS trigger_insert_feature_count_{0};
     DROP TRIGGER IF EXISTS trigger_delete_feature_count_{0};
-    DROP TABLE IF EXISTS {0};
+    DROP TABLE IF EXISTS {1};
 """
 
 
 REMOVE_TABLE: str = """
-    DELETE FROM gpkg_ogr_contents WHERE lower(table_name) = lower('{0}');
     DELETE FROM gpkg_contents WHERE lower(table_name) = lower('{0}');
     DROP TRIGGER IF EXISTS trigger_insert_feature_count_{0};
     DROP TRIGGER IF EXISTS trigger_delete_feature_count_{0};
-    DROP TABLE IF EXISTS {0};
+    DROP TABLE IF EXISTS {1};
 """
 
 
 GPKG_OGR_CONTENTS_INSERT_TRIGGER: str = """
     CREATE TRIGGER trigger_insert_feature_count_{0}
-    AFTER INSERT ON {0}
+    AFTER INSERT ON {1}
     BEGIN UPDATE gpkg_ogr_contents SET feature_count = feature_count + 1 
           WHERE lower(table_name) = lower('{0}'); END;
 """
 
 
 GPKG_OGR_CONTENTS_DELETE_TRIGGER: str = """
     CREATE TRIGGER trigger_delete_feature_count_{0}
-    AFTER DELETE ON {0}
+    AFTER DELETE ON {1}
     BEGIN UPDATE gpkg_ogr_contents SET feature_count = feature_count - 1 
           WHERE lower(table_name) = lower('{0}'); END;
 """
 
 
 INSERT_GPKG_GEOM_COL: str = """
     INSERT INTO gpkg_geometry_columns (
```

## Comparing `fudgeo-0.3.9.dist-info/LICENSE` & `fudgeo-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.3.9.dist-info/METADATA` & `fudgeo-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.3.9
+Version: 0.4.0
 Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

