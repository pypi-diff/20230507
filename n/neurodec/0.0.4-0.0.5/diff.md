# Comparing `tmp/neurodec-0.0.4.tar.gz` & `tmp/neurodec-0.0.5.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodec-0.0.4.tar", last modified: Tue Mar  7 10:15:39 2023, max compression
+gzip compressed data, was "neurodec-0.0.5.linux-x86_64.tar", last modified: Sun May  7 21:03:30 2023, max compression
```

## Comparing `neurodec-0.0.4.tar` & `neurodec-0.0.5.linux-x86_64.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.897556 neurodec-0.0.4/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      155 2023-03-07 10:15:39.897556 neurodec-0.0.4/PKG-INFO
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.894556 neurodec-0.0.4/neurodec/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)       36 2022-12-21 09:29:48.000000 neurodec-0.0.4/neurodec/__init__.py
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.895556 neurodec-0.0.4/neurodec/cli/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)       29 2021-05-06 08:44:00.000000 neurodec-0.0.4/neurodec/cli/__init__.py
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      148 2022-12-21 09:29:41.000000 neurodec-0.0.4/neurodec/cli/argparse.py
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.896556 neurodec-0.0.4/neurodec/mdt/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)    54516 2023-03-02 09:52:54.000000 neurodec-0.0.4/neurodec/mdt/__init__.py
--rw-r--r--   0 sdeslaur (656800) athena    (1190)     4828 2023-02-11 20:53:17.000000 neurodec-0.0.4/neurodec/mdt/auth.py
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.895556 neurodec-0.0.4/neurodec.egg-info/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      155 2023-03-07 10:15:39.000000 neurodec-0.0.4/neurodec.egg-info/PKG-INFO
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      301 2023-03-07 10:15:39.000000 neurodec-0.0.4/neurodec.egg-info/SOURCES.txt
--rw-r--r--   0 sdeslaur (656800) athena    (1190)        1 2023-03-07 10:15:39.000000 neurodec-0.0.4/neurodec.egg-info/dependency_links.txt
--rw-r--r--   0 sdeslaur (656800) athena    (1190)       46 2023-03-07 10:15:39.000000 neurodec-0.0.4/neurodec.egg-info/requires.txt
--rw-r--r--   0 sdeslaur (656800) athena    (1190)        9 2023-03-07 10:15:39.000000 neurodec-0.0.4/neurodec.egg-info/top_level.txt
-drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-03-07 10:15:39.897556 neurodec-0.0.4/scripts/
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      967 2021-05-06 08:29:58.000000 neurodec-0.0.4/scripts/neurodec
--rw-r--r--   0 sdeslaur (656800) athena    (1190)       38 2023-03-07 10:15:39.897556 neurodec-0.0.4/setup.cfg
--rw-r--r--   0 sdeslaur (656800) athena    (1190)      451 2023-03-07 10:10:21.000000 neurodec-0.0.4/setup.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.279389 ./
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.279389 ./usr/
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.577391 ./usr/local/
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.577391 ./usr/local/bin/
+-rwxr-xr-x   0 sdeslaur (656800) athena    (1190)      963 2023-05-07 21:03:30.000000 ./usr/local/bin/neurodec
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.279389 ./usr/local/lib/
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.279389 ./usr/local/lib/python3.11/
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.537390 ./usr/local/lib/python3.11/site-packages/
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      117 2023-05-07 19:20:15.000000 ./usr/local/lib/python3.11/site-packages/neurodec/__init__.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/__pycache__/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      423 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/cli/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)       29 2021-05-06 08:44:00.000000 ./usr/local/lib/python3.11/site-packages/neurodec/cli/__init__.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/cli/__pycache__/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      224 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/cli/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      472 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/cli/__pycache__/argparse.cpython-311.pyc
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      148 2021-05-06 08:48:39.000000 ./usr/local/lib/python3.11/site-packages/neurodec/cli/argparse.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)    74288 2023-05-07 19:20:15.000000 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/__init__.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.284388 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/__pycache__/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)    89427 2023-05-07 21:03:30.284388 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)     6334 2023-05-07 21:03:30.281388 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)     4828 2023-02-11 20:53:17.000000 ./usr/local/lib/python3.11/site-packages/neurodec/mdt/auth.py
+drwxr-xr-x   0 sdeslaur (656800) athena    (1190)        0 2023-05-07 21:03:30.537390 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      155 2023-05-07 21:03:30.367389 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)      301 2023-05-07 21:03:30.537390 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)        1 2023-05-07 21:03:30.390389 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)       59 2023-05-07 21:03:30.508390 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/requires.txt
+-rw-r--r--   0 sdeslaur (656800) athena    (1190)        9 2023-05-07 21:03:30.532390 ./usr/local/lib/python3.11/site-packages/neurodec-0.0.5-py3.11.egg-info/top_level.txt
```

### Comparing `neurodec-0.0.4/neurodec/mdt/__init__.py` & `./usr/local/lib/python3.11/site-packages/neurodec/mdt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 from enum import auto, IntEnum
 import logging
+
 import numpy as np
 from numpy.typing import ArrayLike
 import requests
+import rich
 import time
-from typing import Callable, Collection, Iterable, Optional, Tuple, Union
+from typing import Callable, Collection, List, Optional, Tuple, Union
 from werkzeug.datastructures import ImmutableMultiDict
 
 from .auth import get_credentials
 
 logger = logging.getLogger(__name__)
 
 _API_URL = "http://0.0.0.0:8001"
@@ -23,19 +25,19 @@
     NEW = 0
     PENDING = auto()
     PROCESSING = auto()
     READY = auto()
     ERROR = auto()
 
 
-class SurfaceType(IntEnum):
-    """The surface types which are used to build a volume conductor"""
+class TissueType(IntEnum):
+    """The types of tissues inside a volume conductor."""
 
-    OUTER_SKIN = 0
-    INNER_SKIN = 1
+    SKIN = 0
+    FAT = 1
     BONE = 2
     MUSCLE = 3
     ELECTRODE = 4
 
 
 class ElectrodeLayouts(IntEnum):
     """Possible orderings for grids of electrodes on the skin"""
@@ -48,15 +50,83 @@
 
 
 # Random seed to be used in new() calls when not explicitly given as parameter.
 DEFAULT_RANDOM_SEED = 0
 
 
 # Default radius to be used for fibers during generation.
-DEFAULT_FIBERS_RADIUS = 2.8e-5
+DEFAULT_FIBERS_RADIUS = 4e-5
+
+
+def get_version() -> Optional[str]:
+    """Returns the version of the Myoelectric Digital Twin
+
+    If a connection cannot be established with the MDT for any reason
+    (ConnectionError, Timeout, HTTPError, ...) this function returns
+    None.
+
+    """
+
+    try:
+        response = requests.get(f"{_API_URL}/", timeout=5)
+        return response.json()["mdt"] if response.ok else None
+    except requests.exceptions.RequestException:
+        return None
+
+
+def get_user() -> Optional[dict]:
+    """Returns the current user of the MDT
+
+    If the credentials are not valid, returns None. If the credentials are
+    valid and the MDT can be reached, returns a dictionary with the
+    user information.
+
+    """
+
+    try:
+        response = requests.get(f"{_API_URL}/users/0/", data=get_credentials(), timeout=5)
+        return response.json() if response.ok else None
+    except requests.exceptions.RequestException:
+        return None
+
+
+def is_connected() -> bool:
+    """Returns True if we can connect to the MDT, False otherwise"""
+    return get_version() is not None and get_user() is not None
+
+
+def print_connection_status():
+    """Pretty prints the connection status of the Myoelectric Digital Twin
+
+    Prints a message that indicates if a connection can be established and if
+    the credentials are valid. This is meant for interactive use. For programmatic
+    use, see is_connected.
+
+    """
+
+    # If we can get the version, the MDT is online and well.
+    version = get_version()
+    if version is None:
+        rich.print(
+            f"[bold red]Error[/bold red]: Could not connect to the [blue]Myoelectric Digital Twin[/blue]. "
+            f"Please check that the API URL ({_API_URL}) is correct. "
+            f"If the URL is correct and the error persists, the MDT may be offline.")
+        return
+    else:
+        rich.print(
+            f"The [blue]Myoelectric Digital Twin[/blue] version {version} is online.")
+
+    user = get_user()
+    if user is None:
+        rich.print(
+            f"[bold red]Error[/bold red]: Could not login to the [blue]Myoelectric Digital Twin[/blue]. "
+            f"Please verify that your credentials are correct.")
+    else:
+        rich.print(
+            f"You are connected as [green]{user['email']}[/green].")
 
 
 class MDTObject:
     """Base class for Neurodec Myoelectric Digital Twin classes"""
 
     _url_prefix: str = ""
 
@@ -92,20 +162,25 @@
         response = requests.get(f"{_API_URL}/{cls._url_prefix}/{id}/metadata", json={"credentials": get_credentials()})
         if not response.ok:
             raise ValueError("The metadata could not be retrieved.")
 
         return cls(response.json())
 
     @classmethod
-    def _new_request(cls, json=None):
+    def _new_request(cls, json=None, url_suffix=None):
         if json is None:
             json = {}
         json.update({"credentials": get_credentials()})
-        response = requests.post(f"{_API_URL}/{cls._url_prefix}", json=json)
+        request_url = f"{_API_URL}/{cls._url_prefix}"
+        if url_suffix is not None:
+            request_url += "/" + url_suffix
+        response = requests.post(request_url, json=json)
         if not response.ok:
+            if not is_connected():
+                print_connection_status()
             raise ValueError(f"The {cls.__name__} could not be created.")
 
         # Wait the status to be READY if requested.
         obj = cls(response.json())
         if wait:
             obj.wait()
 
@@ -220,44 +295,45 @@
 
         This function is not meant to be called directly by users. Use
         Surface.new instead.
 
         """
 
         super().__init__(dictionary)
-        self._type = SurfaceType(dictionary["type"])
+        self._type = TissueType(dictionary["type"])
         self._label = None
         self._vertices = None
         self._triangles = None
+        self._image_label = None
 
     def __str__(self):
         """String representation of a surface"""
         return f"Surface({self._id}, {str(self._status)}, {str(self._type)})"
 
     @property
-    def type(self) -> SurfaceType:
+    def type(self) -> TissueType:
         """Returns the type of the surface"""
         return self._type
 
     @classmethod
-    def new(cls, vertices: ArrayLike, triangles: ArrayLike, surface_type: SurfaceType, label: Optional[str] = None,
+    def new(cls, vertices: ArrayLike, triangles: ArrayLike, tissue_type: TissueType, label: Optional[str] = None,
             force_computation: bool = False) -> Surface:
         """Create a new surface
 
         Creates a new surface from raw data. This will initiate a call to the
         Neurodec Myoelectric Digital Twin (MDT) API that will save the surface,
         preprocess it, and return its metadata in the form of a dict.
 
         Args:
             vertices: A numpy array of float with a shape of (N, 3) that
                 contains the location of the vertices.
             triangles: A numpy array of unsigned integers with a shape of
                 (M, 3) that contains the indices of the vertices for each
                 triangle.
-            surface_type: The surface type, see neurodec.mdt.SurfaceType.
+            tissue_type: The tissue enclosed by this surface, see neurodec.mdt.TissueType.
             label: A human-readable name to easily identify the surface. If not given, the label will be autogenerated
                 from the surface type. Note that this label exists only locally and not in the database. This means that
                 if two Surface objects are created with different labels but with same vertices, triangles and types,
                 the result will be two instances that share the same id and status, despite having different labels.
             force_computation: Boolean flag that allows to bypass a status check. Normally, the API would check if an
                 object with the requested parameters was already present in the database. If this was the case, the API
                 would not request its computation and would simply return its identifier. By setting this flag to
@@ -292,82 +368,397 @@
                 "The triangle indices is equal to or exceed the number of vertices"
                 f" ({indices.max()} vs {len(vertices)})."
             )
 
         # Encode the vertices and triangles.
         data = {
             "force_computation": force_computation,
-            "type": surface_type.value,
+            "type": tissue_type.value,
         }
         data.update(_encode_array(vertices, "vertices"))
         data.update(_encode_array(triangles, "triangles"))
 
         surface = cls._new_request(json={"surface": data})
         surface._vertices = vertices
         surface._triangles = triangles
-        surface._label = label if label is not None else f"{surface_type.name.lower()}_{surface.id}"
+        surface._label = label if label is not None else f"{tissue_type.name.lower()}_{surface.id}"
         return surface
 
     @property
     def vertices(self):
+        """Retrieve the vertices of this Surface.
+
+        Return:
+            A NumPy array of float with a shape of (N, 3) that contains the location of the vertices.
+        """
+        if self._vertices is None:
+            self._retrieve_data()
+            self._vertices = _decode_array(self._data_json, "vertices")
         return self._vertices.copy()
 
     @property
     def triangles(self):
+        """Retrieve the triangles of this Surface.
+
+        Return:
+            A NumPy array of unsigned integers with a shape of (M, 3) that contains the indices of the vertices for each
+            triangle.
+        """
+        if self._triangles is None:
+            self._retrieve_data()
+            self._triangles = _decode_array(self._data_json, "triangles")
         return self._triangles.copy()
 
     @property
     def label(self) -> str:
-        """Returns the label of this Surface"""
+        """Returns the human-readable label of this Surface.
+
+        This is the human-readable label (a string) that was passed to Surface.new(). Do not confuse it with the
+        image_label property.
+
+        Returns:
+            The human-readable label of this Surface, if one was given during the Surface.new() call. If the surface was
+            extracted from a Tetrahedra instance, the label will be None.
+        """
         return self._label
 
+    @property
+    def image_label(self) -> Optional[int]:
+        """Returns the image label of this Surface.
+
+        Returns:
+            If this Surface was extracted from an Image, the label that identified it is returned. If this surface was
+            created using Surface.new(), then its image_label will be None.
+        """
+        return self._image_label
+
+
+class Image(MDTObject):
+    """A 3D image containing tissue information."""
+
+    _url_prefix: str = "images"
+
+    @classmethod
+    def new(
+            cls,
+            image: ArrayLike,
+            voxel_sizes: Union[Tuple[float, float, float], ArrayLike],
+            labels: dict,
+            ignore_labels: Optional[Collection[int]] = None,
+            skin_thickness: float = 2e-3,
+            force_computation: bool = False
+    ) -> Image:
+        """Create a new 3D image.
+
+        Create a new 3D image. Once received on the server, it is processed so that its spatial resolution is as uniform
+        as possible.
+
+        Args:
+            image: A NumPy array of integers with a shape of (A, B, C) that contains voxels whose values represent
+                labelled tissues. Each label should correspond to a specific component of the arm. See the argument
+                'labels' for more details.
+            voxel_sizes: A tuple or NumPy array that represents the spatial resolution of the image in the X, Y and Z
+                directions. This is used to associate the voxel at coordinates (i, j, k) to the point in space with
+                Cartesian coordinates (i*voxel_sizes[0], j*voxel_sizes[1], k*voxel_sizes[2]). If two of the values are
+                equal and the remaining one is larger, then the image is pre-processed to increase the resolution in the
+                coarsest direction.
+                .. Important:: The resolution has to be given in meters.
+            labels: Dictionary that specifies what each label in the image corresponds to, in terms of tissues. More
+                precisely, in each image one label should be used to identify skin, one for fat, a couple for the bones
+                (most likely, radius and ulna), several labels to identify the different muscles. Optionally, one or
+                more labels can be given to identify electrodes. Note that if electrodes are not part of an image, they
+                can still be added later using the Electrode class. Labels should be given as a dictionary with the
+                following keys and values:
+                - TissueType.SKIN: the label for the skin, as a positive integer;
+                - TissueType.FAT: the label for the fat, as a positive integer;
+                - TissueType.BONE: the labels for the bones, as a list of positive integers (can be empty);
+                - TissueType.MUSCLE: the labels for the muscles, as a list of positive integers;
+                - TissueType.ELECTRODE: the labels for the electrodes, as a list of positive integers (can be empty).
+                Labels must be unique. As an example, it is an error to have the label '42' both as skin label and as
+                part of the list of muscle labels. The label '0' is a special value that is used to represent empty
+                space and therefore cannot be used. Note that not all labels in the image need to be associated to a
+                tissue. As an example, while creating an MRI, some markers may have been placed on the skin to identify
+                reference locations. These markers are not part of the volume conductor and therefore their label can be
+                ignored while extracting the tetrahedral mesh. In practice, all voxels in the image whose label does not
+                appear in the `labels` variables are ignored and treated as if they represented void space (label '0').
+                For each of these, a warning is issued to prevent issues related to forgotten labels, unless they are
+                explicitly included in the `ignore_labels` variable.
+            ignore_labels: List of labels that appear in the image, but not in `labels`, and that can be safely ignored
+                without issuing a warning. By default, this list is empty, meaning that a warning is issued for every
+                missing label.
+            skin_thickness: After increasing the resolution of the image, the skin is re-computed so that it wraps
+                around the arm with the specified thickness (2mm by default).
+            force_computation: Boolean flag that allows to bypass a status check. Normally, the API would check if an
+                object with the requested parameters was already present in the database. If this was the case, the API
+                would not request its computation and would simply return its identifier. By setting this flag to
+                `True`, the user can bypass this logic and force the computation of the resource even if it existed
+                already. The main reason is to allow starting a calculation again in case of unexpected errors.
+
+        Returns:
+            The new image. If another image with the same parameters already exits, that one will be returned instead
+            of creating a new image.
+        """
+
+        # Make sure that the inputs are interpreted as NumPy arrays.
+        image = np.asarray(image, dtype=int)
+        voxel_sizes = np.asarray(voxel_sizes)
+
+        # Check that the input is a 3D image.
+        if image.ndim != 3:
+            raise ValueError(f"Input 'image' must be an array of integers with 3 dimensions. It has {image.ndim} "
+                             f"dimension(s) instead.")
+
+        # Check that the voxel is a NumPy array with 3 elements.
+        if voxel_sizes.shape != (3, ):
+            raise ValueError(f"Input 'voxel_sizes' must be an array with shape (3,) (single dimension of length 3). "
+                             f"It has instead the shape {voxel_sizes.shape}.")
+
+        largest_resolution = np.max(voxel_sizes)
+        if largest_resolution >= 1e-2:
+            logger.warning(f"The largest image resolution is {largest_resolution}, which appears to be quite large for "
+                           f"an anatomical image. Remember that lengths are all in meters, meaning that the larges "
+                           f"resolution is interpreted as {largest_resolution}m. If the intended unit was different and"
+                           f" you meant for example {largest_resolution}mm, consider rescaling 'voxel_sizes' by the "
+                           f"appropriate factor.")
+
+        # Initialize 'ignore_labels' if it was not given by the user.
+        if ignore_labels is None:
+            ignore_labels = []
+
+        # Check that all mandatory labels are present.
+        mandatory_tissues = [TissueType.SKIN, TissueType.FAT, TissueType.BONE, TissueType.MUSCLE]
+        for tissue in mandatory_tissues:
+            if tissue not in labels:
+                raise ValueError(f"Missing tissue '{tissue.name}' in 'labels'.")
+
+        # Complete the labels with optional ones.
+        non_list_tissues = [TissueType.SKIN, TissueType.FAT]
+        list_tissues = [TissueType.BONE, TissueType.MUSCLE, TissueType.ELECTRODE]
+        tissues = non_list_tissues + list_tissues
+        labels = {tissue: labels.get(tissue, []) for tissue in tissues}
+        labels_lists = [[labels[t]] for t in non_list_tissues] + [labels[t] for t in list_tissues]
+
+        for i in range(len(tissues) - 1):
+            # Make sure that labels are all positive integers.
+            for label in labels_lists[i]:
+                if not isinstance(label, (int, np.integer)) or label < 1:
+                    raise ValueError(
+                        f"Label for '{tissues[i].name}' tissue is invalid: expected positive integer, got "
+                        f"'{label}'.")
+
+            # Make sure there are no label repetitions.
+            if len(set(labels_lists[i])) != len(labels_lists[i]):
+                raise ValueError(f"Invalid labels for tissue '{tissues[i].name}': all values must be unique. Got: "
+                                 f"{labels_lists[i]}")
+            for j in range(i + 1, len(tissues)):
+                if any(label in labels_lists[j] for label in labels_lists[i]):
+                    raise ValueError(
+                        f"Invalid labels: '{tissues[i].name}' and '{tissues[j].name}' share at least one "
+                        f"label. {tissues[i].name}: {labels_lists[i]}, {tissues[j].name}: "
+                        f"{labels_lists[j]}.")
+
+        # Check that all values in the image are associated with a label. If not, issue warnings as needed.
+        all_labels = sum(labels_lists, [0])
+        unique_labels = np.unique(image)
+        for image_label in unique_labels:
+            if image_label not in all_labels and image_label not in ignore_labels:
+                logger.warning(
+                    f"Image label '{image_label}' does not has not been given tissue information. If this is"
+                    f" intentional, consider adding '{image_label}' to the argument 'ignore_labels'.")
+
+        # Also, make sure that the labels to ignore are valid, meaning that they all exist in the image and none of them
+        # appear in the 'labels' dictionary.
+        non_existing_labels = [label for label in ignore_labels if label not in unique_labels]
+        if len(non_existing_labels) > 0:
+            raise ValueError(
+                f"The labels {non_existing_labels} were part of 'ignore_labels', but they are not present "
+                f"in the original image.")
+
+        non_ignorable_labels = [label for label in ignore_labels if label in all_labels]
+        if len(non_ignorable_labels) > 0:
+            raise ValueError(
+                f"The labels {non_ignorable_labels} were part of 'ignore_labels', but they are present in "
+                f"the 'labels' dictionary.")
+
+        # Encode the parameters.
+        data = {
+            "force_computation": force_computation,
+            "labels": labels,
+            "skin_thickness": skin_thickness,
+        }
+        data.update(_encode_array(image, "image"))
+        data.update(_encode_array(voxel_sizes, "voxel_sizes"))
+
+        # Send the image to the server and keep track of its metadata.
+        image_metadata = cls._new_request(json=data)
+        return image_metadata
+
+
+class Tetrahedra(MDTObject):
+    """A labelled tetrahedral mesh."""
+
+    _url_prefix: str = "tetrahedra"
+    _surfaces: Optional[Collection[Surface]] = None
+
+    @classmethod
+    def from_image(
+            cls,
+            image: Image,
+            sizes: float = 1e-3,
+            distance: float = 1e-3,
+            force_computation: bool = False
+    ) -> Tetrahedra:
+        """Create a labelled tetrahedral mesh from a set of voxels.
+
+        Args:
+            image: The labelled 3D image from which the tetrahedral mesh should be extracted.
+            sizes: This parameter controls the size of surface facets. Each surface facet has a surface Delaunay ball
+                which is a ball circumscribing the surface facet and centered on the surface patch.
+            distance: This parameter controls the approximation error of boundary and subdivision surfaces. It provides
+                an upper bound for the distance between the circumcenter of a surface facet and the center of a surface
+                Delaunay ball of this facet.
+            force_computation: Boolean flag that allows to bypass a status check. Normally, the API would check if an
+                object with the requested parameters was already present in the database. If this was the case, the API
+                would not request its computation and would simply return its identifier. By setting this flag to
+                `True`, the user can bypass this logic and force the computation of the resource even if it existed
+                already. The main reason is to allow starting a calculation again in case of unexpected errors.
+        Returns:
+            The metadata of the new tetrahedra. If another object with the same parameters already exits, that one will
+            be returned instead of building a new one.
+        """
+        data = {
+            "force_computation": force_computation,
+            "image_id": image.id,
+            "sizes": sizes,
+            "distance": distance,
+        }
+        return cls._new_request(json=data, url_suffix="from_image")
+
+    @classmethod
+    def from_surfaces(
+            cls,
+            surfaces: Collection[Surface],
+            sizes: float = 1e-3,
+            distance: float = 1e-3,
+            force_computation: bool = False
+    ) -> Tetrahedra:
+        """Create a labelled tetrahedral mesh from a set of surfaces.
+
+        Args:
+            surfaces: The surface meshes from which the tetrahedral mesh should be built. There must be exactly one
+                surface of type TissueType.SKIN, one of type TissueType.SKIN and at least one of type TissueType.MUSCLE.
+            sizes: This parameter controls the size of surface facets. Each surface facet has a surface Delaunay ball
+                which is a ball circumscribing the surface facet and centered on the surface patch.
+            distance: This parameter controls the approximation error of boundary and subdivision surfaces. It provides
+                an upper bound for the distance between the circumcenter of a surface facet and the center of a surface
+                Delaunay ball of this facet.
+            force_computation: Boolean flag that allows to bypass a status check. Normally, the API would check if an
+                object with the requested parameters was already present in the database. If this was the case, the API
+                would not request its computation and would simply return its identifier. By setting this flag to
+                `True`, the user can bypass this logic and force the computation of the resource even if it existed
+                already. The main reason is to allow starting a calculation again in case of unexpected errors.
+        Returns:
+            The metadata of the new tetrahedra. If another object with the same parameters already exits, that one will
+            be returned instead of building a new one.
+        """
+        data = {
+            "force_computation": force_computation,
+            "surfaces": [s.id for s in surfaces],
+            "sizes": sizes,
+            "distance": distance,
+        }
+        return cls._new_request(json=data, url_suffix="from_surfaces")
+
+    @property
+    def surfaces(self):
+        if self._surfaces is None:
+            self._retrieve_data()
+            self._surfaces = []
+            for id, label in self._data_json["surfaces_data"]:
+                s = Surface._get_metadata(id)
+                s._image_label = label
+                self._surfaces.append(s)
+
+        return self._surfaces
+
+    def _surfaces_of_type(self, tissue_type):
+        surfaces = [s for s in self.surfaces if s.type == tissue_type]
+        if len(surfaces) == 0:
+            logger.warning(f"Could not find any surface of type '{tissue_type.name}' associated to this Tetrahedra "
+                           f"instance.")
+        return surfaces
 
-def default_conductivities() -> dict[str, ArrayLike]:
+    @property
+    def skin(self):
+        """Retrieve the skin surface of this mesh.
+
+        Returns:
+            A Surface object representing the skin of the mesh. If this Tetrahedra object was created from an Image, the
+            surface is extracted from the mesh once the image is processed. If the object was created from a set of
+            surfaces, this surface is the same that was given as input.
+        """
+        skins = self._surfaces_of_type(TissueType.SKIN)
+        if len(skins) != 1:
+            raise RuntimeError(f"Every Tetrahedra instance must have exactly one skin surface, however {len(skins)} "
+                               f"were found.")
+        return skins[0]
+
+    @property
+    def muscles(self):
+        """Retrieve the muscle surfaces of this mesh.
+
+        Returns:
+            A list of Surface objects representing the muscles of the mesh. If this Tetrahedra object was created from
+            an Image, the surfaces are extracted from the mesh once the image is processed. If the object was created
+            from a set of surfaces, these surfaces are the same that were given as input.
+        """
+        return self._surfaces_of_type(TissueType.MUSCLE)
+
+
+def default_conductivities() -> dict[TissueType, ArrayLike]:
     """Create a dictionary containing default conductivities for each tissue type.
 
     Returns:
-        A dictionary in the form {tissue: conductivity} where tissue is one of the strings "skin", "fat", "bone",
-        "muscle" or "electrode" and conductivity is either a scalar (isotropic tissue) or the principal components
-        (anisotropic tissue).
+        A dictionary in the form {tissue: conductivity} where tissue is one of the values of the TissueType
+        enumeration, and conductivity is either a scalar (isotropic tissue) or the principal components (anisotropic
+        tissue).
     """
     return {
-        "skin": 0.17,
-        "fat": 5.73e-2,
-        "bone": 8.2e-2,
-        "muscle": [0.5, 0.1, 0.1],
-        "electrode": 2.0
+        TissueType.SKIN: 0.17,
+        TissueType.FAT: 5.73e-2,
+        TissueType.BONE: 8.2e-2,
+        TissueType.MUSCLE: [0.5, 0.1, 0.1],
+        TissueType.ELECTRODE: 2.0
     }
 
 
 class Conductor(MDTObject):
     """A volume conductor"""
 
     _url_prefix: str = "conductor"
 
     @classmethod
     def new(
         cls,
-        surfaces: Iterable[Surface],
+        tetrahedra: Tetrahedra,
         skin_conductivity: float = 0.17,
         fat_conductivity: float = 5.73e-2,
         bone_conductivity: float = 8.2e-2,
         muscle_conductivity: Optional[Union[float, ArrayLike]] = None,
         electrode_conductivity: float = 2.0,
         force_computation: bool = False
     ) -> Conductor:
         """Create a new volume conductor
 
         Creates a new volume conductor from surfaces. This will initiate a call
         to the Neurodec Myoelectric Digital Twin (MDT) API that will build
         the conductor and return its metadata in the form of a dict.
 
         Args:
-            surfaces: The surfaces used to define the volume conductor. Must
-                contain at least one OUTER_SKIN surface and one INNER_SKIN
-                surface.
+            tetrahedra: The labelled tetrahedral mesh used to define the volume conductor.
             skin_conductivity: Conductivity of skin tissue. This tissue is assumed to be isotropic and therefore only
                 one value is required to define the conductivity tensor.
             fat_conductivity: Conductivity of fat tissue. This tissue is assumed to be isotropic and therefore only one
                 value is required to define the conductivity tensor.
             bone_conductivity: Conductivity of bone tissue. This tissue is assumed to be isotropic and therefore only
                 one value is required to define the conductivity tensor.
             muscle_conductivity: Principal conductivity components of muscle tissue. This tissue is assumed to be
@@ -379,61 +770,56 @@
                 - A 2-dimensional vector in the form (C1, C2). In this case, a third value is added to complete the
                   principal components as (C1, C2, C2).
                 - A 3-dimensional vector in the form (C1, C2, C3). The vector is passed as-is to the API. However, a
                   warning is issued if C2 != C3.
                 - None: the default values (0.5, 0.1, 0.1) are used for the principal components.
             electrode_conductivity: Conductivity of electrode material. This material is assumed to be isotropic and
                 therefore only one value is required to define the conductivity tensor.
-
-                - A scalar (isotropic tissue).
-                - A vector containing the 3 principal components of the conductivity tensor. This is allowed only for
-                  the MUSCLE tissue type.
             force_computation: Boolean flag that allows to bypass a status check. Normally, the API would check if an
                 object with the requested parameters was already present in the database. If this was the case, the API
                 would not request its computation and would simply return its identifier. By setting this flag to
                 `True`, the user can bypass this logic and force the computation of the resource even if it existed
                 already. The main reason is to allow starting a calculation again in case of unexpected errors.
 
         Returns:
             The metadata of the new conductor. If another conductor with the
             same parameters already exits, that one will be returned instead of
             building a new one.
-
         """
         # If muscle conductivities are not given, use the default ones. If they are given, make sure they become a list
         # in the form [c1, c2, c3].
         if muscle_conductivity is None:
             muscle_conductivity = [0.5, 0.1, 0.1]
         elif np.isscalar(muscle_conductivity):
             muscle_conductivity = [muscle_conductivity] * 3
         else:
             muscle_conductivity = np.asarray(muscle_conductivity)
             if muscle_conductivity.shape == (2,):
                 c1, c2 = muscle_conductivity
                 muscle_conductivity = [c1, c2, c2]
-            elif len(muscle_conductivity) == (3,):
+            elif muscle_conductivity.shape == (3,):
                 c1, c2, c3 = muscle_conductivity
                 if not np.allclose(c2, c3):
                     logger.warning(f"Received 3 muscle conductivities, with c2 != c3. {c2=}, {c3=}.")
                 muscle_conductivity = [c1, c2, c3]
             else:
                 raise RuntimeError(f"Principal conductivity components for a muscle must be given as either a scalar or"
                                    f" an array with 2 or 3 components. An array with shape {muscle_conductivity.shape} "
                                    f"was received.")
 
-        # Encode the surfaces.
+        # Encode the input data.
         json = {
             "force_computation": force_computation,
-            "surfaces": [s.id for s in surfaces],
+            "tetrahedra": tetrahedra.id,
             "conductivities": {
-                "skin": skin_conductivity,
-                "fat": fat_conductivity,
-                "bone": bone_conductivity,
-                "muscle": muscle_conductivity,
-                "electrode": electrode_conductivity
+                TissueType.SKIN: skin_conductivity,
+                TissueType.FAT: fat_conductivity,
+                TissueType.BONE: bone_conductivity,
+                TissueType.MUSCLE: muscle_conductivity,
+                TissueType.ELECTRODE: electrode_conductivity
             }
         }
 
         return cls._new_request(json=json)
 
 
 class Electrode(MDTObject):
@@ -532,15 +918,15 @@
             force_computation: bool = False
     ) -> ElectrodeBracelet:
         """Generate a bracelet of electrodes on the given surface.
 
         A bracelet is a series of electrodes arranged in multiple rings that should wrap around the given surface.
 
         Args:
-            skin: A Surface object with type OUTER_SKIN where the electrodes will be placed.
+            skin: A Surface object with type SKIN where the electrodes will be placed.
             radius: Radius of an electrode. The same value is used for all electrodes in the bracelet.
             first_electrode_location: A numpy array containing 3D coordinates of the first electrode of the first ring.
                 Does not have to be precisely on the skin mesh - the point will be projected onto it.
             rings_normal: A numpy array containing the direction of the normal vector defining the bracelet section planes.
                 Note, that all the rings have the same normal vector.
             n_rings: The number of electrode rings in the bracelet. If larger than 1, the initial bracelet plan is shifted
                 in the direction of the normal vector for a distance distance_between_rings.
@@ -585,15 +971,15 @@
             layout: ElectrodeLayouts,
             smooth_surface: bool = True,
             force_computation: bool = False
     ) -> ElectrodeGrid:
         """Generate a grid of electrodes on the given surface.
 
         Args:
-            skin: A Surface object with type OUTER_SKIN where the electrodes will be placed.
+            skin: A Surface object with type SKIN where the electrodes will be placed.
             radius: Radius of an electrode. The same value is used for all electrodes in the bracelet.
             corners: A NumPy array with shape (4, 3) representing the 3D corners of a rectangular patch of skin that
                 should contain a grid of electrodes. The four corners are to be given in the order top-left (grid[0]),
                 top-right (grid[1]), bottom-left (grid[2]), bottom-right (grid[3]). The points do not need to define an
                 actual rectangle, but rather an approximation of it. In addition, they do not have to be precisely on
                 the skin mesh.
             shape: A NumPy array with shape (2,), containing the rows and columns (respectively as first and second
```

### Comparing `neurodec-0.0.4/neurodec/mdt/auth.py` & `./usr/local/lib/python3.11/site-packages/neurodec/mdt/auth.py`

 * *Files identical despite different names*

### Comparing `neurodec-0.0.4/scripts/neurodec` & `./usr/local/bin/neurodec`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/python
 
 import argparse
 import pkgutil
 
 import neurodec.cli
 import neurodec.cli.commands
```

