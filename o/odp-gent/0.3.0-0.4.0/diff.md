# Comparing `tmp/odp_gent-0.3.0.tar.gz` & `tmp/odp_gent-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_gent-0.3.0.tar", max compression
+gzip compressed data, was "odp_gent-0.4.0.tar", max compression
```

## Comparing `odp_gent-0.3.0.tar` & `odp_gent-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-03-08 00:16:46.348398 odp_gent-0.3.0/LICENSE
--rw-r--r--   0        0        0     9345 2023-03-08 00:16:46.348398 odp_gent-0.3.0/README.md
--rw-r--r--   0        0        0      319 2023-03-08 00:16:46.348398 odp_gent-0.3.0/odp_gent/__init__.py
--rw-r--r--   0        0        0      260 2023-03-08 00:16:46.348398 odp_gent-0.3.0/odp_gent/exceptions.py
--rw-r--r--   0        0        0     3877 2023-03-08 00:16:46.352398 odp_gent-0.3.0/odp_gent/models.py
--rw-r--r--   0        0        0     5193 2023-03-08 00:16:46.352398 odp_gent-0.3.0/odp_gent/odp_gent.py
--rw-r--r--   0        0        0        0 2023-03-08 00:16:46.352398 odp_gent-0.3.0/odp_gent/py.typed
--rw-r--r--   0        0        0     3827 2023-03-08 00:17:02.920586 odp_gent-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10884 1970-01-01 00:00:00.000000 odp_gent-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-07 13:38:18.833757 odp_gent-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7549 2023-05-07 13:38:18.837757 odp_gent-0.4.0/README.md
+-rw-r--r--   0        0        0      369 2023-05-07 13:38:18.837757 odp_gent-0.4.0/odp_gent/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-07 13:38:18.837757 odp_gent-0.4.0/odp_gent/exceptions.py
+-rw-r--r--   0        0        0     6795 2023-05-07 13:38:18.837757 odp_gent-0.4.0/odp_gent/models.py
+-rw-r--r--   0        0        0     6535 2023-05-07 13:38:18.837757 odp_gent-0.4.0/odp_gent/odp_gent.py
+-rw-r--r--   0        0        0        0 2023-05-07 13:38:18.837757 odp_gent-0.4.0/odp_gent/py.typed
+-rw-r--r--   0        0        0     3880 2023-05-07 13:38:32.630091 odp_gent-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 odp_gent-0.4.0/PKG-INFO
```

### Comparing `odp_gent-0.3.0/LICENSE` & `odp_gent-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odp_gent-0.3.0/README.md` & `odp_gent-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -33,68 +33,20 @@
 pip install odp-gent
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- Parking garages occupancy (12 locations)
-- Park and Ride occupancy (5 locations)
+- [Parking garages occupancy][garages] (12 locations)
+- [Park and Ride occupancy][parkandride] (5 locations)
+- [BlueBike rental locations][bluebike] (6 locations)
+- [Partago vehicle locations][partago] (116 locations)
 
-<details>
-    <summary>Click here to get more details</summary>
-
-### Parking garages
-
-Parameters:
-
-- **limit** (default: 10) - How many results you want to retrieve.
-
-| Variable | Type | Description |
-| :------- | :--- | :---------- |
-| `garage_id` | string | The id of the garage |
-| `name` | string | The name of the garage |
-| `parking_type` | string | The type of parking |
-| `url` | string | The url with more information about the garage |
-| `is_open` | boolean | Whether the garage is open or not |
-| `free_parking` | boolean | Whether there is free parking or not |
-| `temporary_closed` | boolean | Whether the garage is temporarily closed or not |
-| `free_space` | integer | The amount of free parking spaces |
-| `total_capacity` | integer | The total capacity of the garage |
-| `availability_pct` | float | The percentage of free parking spaces |
-| `occupancy_pct` | integer | The percentage of occupied parking spaces |
-| `longitude` | float | The longitude of the garage |
-| `latitude` | float | The latitude of the garage |
-| `updated_at` | datetime | The last time the data was updated |
-
-### Park and Ride
-
-Parameters:
-
-- **limit** (default: 10) - How many results you want to retrieve.
-- **gentse_feesten** - Whether a park and ride location is used for the [Gentse Feesten](https://gentsefeesten.stad.gent).
-
-| Variable | Type | Description |
-| :------- | :--- | :---------- |
-| `spot_id` | string | The id of the park and ride |
-| `name` | string | The name of the park and ride |
-| `parking_type` | string | The type of parking |
-| `url` | string | The url with more information about the park and ride |
-| `is_open` | boolean | Whether the park and ride is open or not |
-| `free_parking` | boolean | Whether there is free parking or not |
-| `temporary_closed` | boolean | Whether the park and ride is temporarily closed or not |
-| `gentse_feesten` | boolean | Whether the park and ride is used for the [Gentse Feesten](https://gentsefeesten.stad.gent) |
-| `free_space` | integer | The amount of free parking spaces |
-| `total_capacity` | integer | The total capacity of the park and ride |
-| `availability_pct` | float | The percentage of free parking spaces |
-| `occupancy_pct` | integer | The percentage of occupied parking spaces |
-| `longitude` | float | The longitude of the park and ride |
-| `latitude` | float | The latitude of the park and ride |
-| `updated_at` | datetime | The last time the data was updated |
-</details>
+Find here [more information](examples) about the different variables and parameters per dataset with this python package.
 
 ## Example
 
 ```python
 import asyncio
 
 from odp_gent import ODPGent
@@ -200,14 +152,19 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [api]: https://data.stad.gent/explore
 [nipkaart]: https://www.nipkaart.nl
 
+[garages]: https://data.stad.gent/explore/dataset/bezetting-parkeergarages-real-time/information
+[parkandride]: https://data.stad.gent/explore/dataset/real-time-bezetting-pr-gent/information
+[bluebike]: https://data.stad.gent/explore/?disjunctive.keyword&disjunctive.theme&sort=modified&q=bluebike
+[partago]: https://data.stad.gent/explore/dataset/real-time-locaties-deelwagen-partago/information
+
 <!-- MARKDOWN LINKS & IMAGES -->
 [build-shield]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/tests.yaml/badge.svg
 [build-url]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-odp-gent.svg
 [commits-url]: https://github.com/klaasnicolaas/python-odp-gent/commits/main
```

### Comparing `odp_gent-0.3.0/odp_gent/odp_gent.py` & `odp_gent-0.4.0/odp_gent/odp_gent.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import async_timeout
 from aiohttp import ClientError, ClientSession
 from aiohttp.hdrs import METH_GET
 from yarl import URL
 
 from .exceptions import ODPGentConnectionError, ODPGentError
-from .models import Garage, ParkAndRide
+from .models import BlueBike, Garage, ParkAndRide, Partago
 
 
 @dataclass
 class ODPGent:
     """Main class for handling data fetchting from Open Data Platform of Gent."""
 
     request_timeout: float = 10.0
@@ -75,22 +75,18 @@
                     params=params,
                     headers=headers,
                     ssl=True,
                 )
                 response.raise_for_status()
         except asyncio.TimeoutError as exception:
             msg = "Timeout occurred while connecting to the Open Data Platform API."
-            raise ODPGentConnectionError(
-                msg,
-            ) from exception
+            raise ODPGentConnectionError(msg) from exception
         except (ClientError, socket.gaierror) as exception:
             msg = "Error occurred while communicating with Open Data Platform API."
-            raise ODPGentConnectionError(
-                msg,
-            ) from exception
+            raise ODPGentConnectionError(msg) from exception
 
         content_type = response.headers.get("Content-Type", "")
         if "application/json" not in content_type:
             text = await response.text()
             msg = "Unexpected content type response from the Open Data Platform API"
             raise ODPGentError(
                 msg,
@@ -150,14 +146,58 @@
             params=params,
         )
 
         for item in locations["records"]:
             results.append(ParkAndRide.from_dict(item))
         return results
 
+    async def bluebikes(self) -> list[BlueBike]:
+        """Get list of data from BlueBike locations.
+
+        Returns
+        -------
+            A list of BlueBike objects.
+        """
+        results: list[BlueBike] = []
+
+        # Data is spread over multiple datasets
+        datasets: list[str] = [
+            "blue-bike-deelfietsen-gent-sint-pieters-st-denijslaan",
+            "blue-bike-deelfietsen-merelbeke-drongen-wondelgem",
+            "blue-bike-deelfietsen-gent-sint-pieters-m-hendrikaplein",
+            "blue-bike-deelfietsen-gent-dampoort",
+        ]
+
+        for dataset in datasets:
+            locations = await self._request(
+                "search/",
+                params={"dataset": dataset},
+            )
+
+            for item in locations["records"]:
+                results.append(BlueBike.from_dict(item))
+        return results
+
+    async def partago_vehicles(self, limit: int = 10) -> list[Partago]:
+        """Get list of data from Partago vehicles.
+
+        Returns
+        -------
+            A list of Partago objects.
+        """
+        results: list[Partago] = []
+        vehicles = await self._request(
+            "search/",
+            params={"dataset": "real-time-locaties-deelwagen-partago", "rows": limit},
+        )
+
+        for item in vehicles["records"]:
+            results.append(Partago.from_dict(item))
+        return results
+
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> ODPGent:
         """Async enter.
```

### Comparing `odp_gent-0.3.0/pyproject.toml` & `odp_gent-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp-gent"
-version = "0.3.0"
+version = "0.4.0"
 description = "Asynchronous Python client providing Open Data information of Gent"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-odp-gent"
 repository = "https://github.com/klaasnicolaas/python-odp-gent"
@@ -26,35 +26,37 @@
     { include = "odp_gent" }
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
+pytz = "^2023.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-odp-gent/issues"
 Changelog = "https://github.com/klaasnicolaas/python-odp-gent/releases"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.243,<0.0.255"
+ruff = ">=0.0.243,<0.0.265"
 aresponses = "^2.1.6"
 black = ">=22.10,<24.0"
 blacken-docs = "^1.13.0"
 codespell = "^2.2.2"
 coverage = {version = ">=7.2,<8.0", extras = ["toml"]}
-mypy = ">=1.0,<1.1"
+mypy = ">=1.0,<1.3"
 pre-commit = "^3.1.1"
 pre-commit-hooks = "^4.4.0"
 pylint = "^2.16.4"
 pytest = "^7.2.2"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
 yamllint = "^1.29.0"
 covdefaults = "^2.3.0"
+types-pytz = "^2023.3.0.0"
 
 [tool.black]
 target-version = ['py39']
 
 [tool.coverage.paths]
 source = ["odp_gent"]
```

### Comparing `odp_gent-0.3.0/PKG-INFO` & `odp_gent-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-gent
-Version: 0.3.0
+Version: 0.4.0
 Summary: Asynchronous Python client providing Open Data information of Gent
 Home-page: https://github.com/klaasnicolaas/python-odp-gent
 License: MIT
 Keywords: open,data,platform,parking,gent,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Klaas Schoute
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: yarl (>=1.6.0)
 Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-odp-gent/issues
 Project-URL: Changelog, https://github.com/klaasnicolaas/python-odp-gent/releases
 Project-URL: Documentation, https://github.com/klaasnicolaas/python-odp-gent
 Project-URL: Repository, https://github.com/klaasnicolaas/python-odp-gent
 Description-Content-Type: text/markdown
 
@@ -67,68 +68,20 @@
 pip install odp-gent
 ```
 
 ## Datasets
 
 You can read the following datasets with this package:
 
-- Parking garages occupancy (12 locations)
-- Park and Ride occupancy (5 locations)
+- [Parking garages occupancy][garages] (12 locations)
+- [Park and Ride occupancy][parkandride] (5 locations)
+- [BlueBike rental locations][bluebike] (6 locations)
+- [Partago vehicle locations][partago] (116 locations)
 
-<details>
-    <summary>Click here to get more details</summary>
-
-### Parking garages
-
-Parameters:
-
-- **limit** (default: 10) - How many results you want to retrieve.
-
-| Variable | Type | Description |
-| :------- | :--- | :---------- |
-| `garage_id` | string | The id of the garage |
-| `name` | string | The name of the garage |
-| `parking_type` | string | The type of parking |
-| `url` | string | The url with more information about the garage |
-| `is_open` | boolean | Whether the garage is open or not |
-| `free_parking` | boolean | Whether there is free parking or not |
-| `temporary_closed` | boolean | Whether the garage is temporarily closed or not |
-| `free_space` | integer | The amount of free parking spaces |
-| `total_capacity` | integer | The total capacity of the garage |
-| `availability_pct` | float | The percentage of free parking spaces |
-| `occupancy_pct` | integer | The percentage of occupied parking spaces |
-| `longitude` | float | The longitude of the garage |
-| `latitude` | float | The latitude of the garage |
-| `updated_at` | datetime | The last time the data was updated |
-
-### Park and Ride
-
-Parameters:
-
-- **limit** (default: 10) - How many results you want to retrieve.
-- **gentse_feesten** - Whether a park and ride location is used for the [Gentse Feesten](https://gentsefeesten.stad.gent).
-
-| Variable | Type | Description |
-| :------- | :--- | :---------- |
-| `spot_id` | string | The id of the park and ride |
-| `name` | string | The name of the park and ride |
-| `parking_type` | string | The type of parking |
-| `url` | string | The url with more information about the park and ride |
-| `is_open` | boolean | Whether the park and ride is open or not |
-| `free_parking` | boolean | Whether there is free parking or not |
-| `temporary_closed` | boolean | Whether the park and ride is temporarily closed or not |
-| `gentse_feesten` | boolean | Whether the park and ride is used for the [Gentse Feesten](https://gentsefeesten.stad.gent) |
-| `free_space` | integer | The amount of free parking spaces |
-| `total_capacity` | integer | The total capacity of the park and ride |
-| `availability_pct` | float | The percentage of free parking spaces |
-| `occupancy_pct` | integer | The percentage of occupied parking spaces |
-| `longitude` | float | The longitude of the park and ride |
-| `latitude` | float | The latitude of the park and ride |
-| `updated_at` | datetime | The last time the data was updated |
-</details>
+Find here [more information](examples) about the different variables and parameters per dataset with this python package.
 
 ## Example
 
 ```python
 import asyncio
 
 from odp_gent import ODPGent
@@ -234,14 +187,19 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [api]: https://data.stad.gent/explore
 [nipkaart]: https://www.nipkaart.nl
 
+[garages]: https://data.stad.gent/explore/dataset/bezetting-parkeergarages-real-time/information
+[parkandride]: https://data.stad.gent/explore/dataset/real-time-bezetting-pr-gent/information
+[bluebike]: https://data.stad.gent/explore/?disjunctive.keyword&disjunctive.theme&sort=modified&q=bluebike
+[partago]: https://data.stad.gent/explore/dataset/real-time-locaties-deelwagen-partago/information
+
 <!-- MARKDOWN LINKS & IMAGES -->
 [build-shield]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/tests.yaml/badge.svg
 [build-url]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/tests.yaml
 [code-quality-shield]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/codeql.yaml/badge.svg
 [code-quality]: https://github.com/klaasnicolaas/python-odp-gent/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-odp-gent.svg
 [commits-url]: https://github.com/klaasnicolaas/python-odp-gent/commits/main
```

