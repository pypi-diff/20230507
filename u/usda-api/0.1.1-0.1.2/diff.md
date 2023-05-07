# Comparing `tmp/usda_api-0.1.1.tar.gz` & `tmp/usda_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda_api-0.1.1.tar", last modified: Sun May  7 03:42:07 2023, max compression
+gzip compressed data, was "usda_api-0.1.2.tar", last modified: Sun May  7 04:05:01 2023, max compression
```

## Comparing `usda_api-0.1.1.tar` & `usda_api-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.348842 usda_api-0.1.1/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 03:42:07.348022 usda_api-0.1.1/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:32:11.000000 usda_api-0.1.1/README.md
--rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2023-05-07 03:42:07.349077 usda_api-0.1.1/setup.cfg
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1850 2023-05-06 09:43:55.000000 usda_api-0.1.1/setup.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.329935 usda_api-0.1.1/src/
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.333858 usda_api-0.1.1/src/usda_api/
--rw-r--r--   0 lohyikuang   (501) staff       (20)       22 2023-05-06 14:37:07.000000 usda_api-0.1.1/src/usda_api/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.339325 usda_api-0.1.1/src/usda_api/scrapers/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 08:30:22.000000 usda_api-0.1.1/src/usda_api/scrapers/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.340938 usda_api-0.1.1/src/usda_api/scrapers/esr/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      201 2023-05-06 14:35:52.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     6552 2023-05-06 09:43:55.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/main.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.344606 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      470 2023-05-06 09:43:55.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     2019 2023-05-06 09:36:01.000000 usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/response.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.346161 usda_api-0.1.1/src/usda_api/scrapers/gats/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:42.000000 usda_api-0.1.1/src/usda_api/scrapers/gats/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.346896 usda_api-0.1.1/src/usda_api/scrapers/psd/
--rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:44.000000 usda_api-0.1.1/src/usda_api/scrapers/psd/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 03:42:07.338128 usda_api-0.1.1/src/usda_api.egg-info/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)      536 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/SOURCES.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/dependency_links.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       55 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/entry_points.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)      404 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/requires.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        9 2023-05-07 03:42:07.000000 usda_api-0.1.1/src/usda_api.egg-info/top_level.txt
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:01.003996 usda_api-0.1.2/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 04:05:01.002579 usda_api-0.1.2/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:32:11.000000 usda_api-0.1.2/README.md
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2023-05-07 04:05:01.004201 usda_api-0.1.2/setup.cfg
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1850 2023-05-06 09:43:55.000000 usda_api-0.1.2/setup.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:00.985083 usda_api-0.1.2/src/
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:00.989527 usda_api-0.1.2/src/usda_api/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       22 2023-05-07 04:04:49.000000 usda_api-0.1.2/src/usda_api/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:00.996351 usda_api-0.1.2/src/usda_api/scrapers/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 08:30:22.000000 usda_api-0.1.2/src/usda_api/scrapers/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:00.998476 usda_api-0.1.2/src/usda_api/scrapers/esr/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      201 2023-05-06 14:35:52.000000 usda_api-0.1.2/src/usda_api/scrapers/esr/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     7695 2023-05-07 04:03:55.000000 usda_api-0.1.2/src/usda_api/scrapers/esr/main.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:01.000637 usda_api-0.1.2/src/usda_api/scrapers/esr/schemas/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      533 2023-05-07 04:00:55.000000 usda_api-0.1.2/src/usda_api/scrapers/esr/schemas/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     2376 2023-05-07 04:03:40.000000 usda_api-0.1.2/src/usda_api/scrapers/esr/schemas/response.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:01.001464 usda_api-0.1.2/src/usda_api/scrapers/gats/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:42.000000 usda_api-0.1.2/src/usda_api/scrapers/gats/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:01.002049 usda_api-0.1.2/src/usda_api/scrapers/psd/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        0 2023-05-06 07:42:44.000000 usda_api-0.1.2/src/usda_api/scrapers/psd/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2023-05-07 04:05:00.994984 usda_api-0.1.2/src/usda_api.egg-info/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      184 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      536 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       55 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/entry_points.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      404 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/requires.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        9 2023-05-07 04:05:00.000000 usda_api-0.1.2/src/usda_api.egg-info/top_level.txt
```

### Comparing `usda_api-0.1.1/setup.py` & `usda_api-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `usda_api-0.1.1/src/usda_api/scrapers/esr/main.py` & `usda_api-0.1.2/src/usda_api/scrapers/esr/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     ESRUnitsOfMeasureCleanedType,
     ESRCountryExportType,
     ESRCountryExportCleanedType,
     ESRAllCountriesExportType,
     ESRAllCountriesExportCleanedType,
     ESRCountryExportGeneralType,
     ESRCountryExportGeneralCleanedType,
+    ESRDataReleaseDateType,
+    ESRDataReleaseDateCleanedType,
 )
 
 API_ID: str = "/api/esr"
 BASE_API: str = "https://apps.fas.usda.gov/OpenData"
 
 REGIONS: str = "/regions"
 COUNTRIES: str = "/countries"
@@ -112,15 +114,37 @@
                 "unit_id": entry["unitId"],
                 "unit_names": entry["unitNames"].strip(),
             },
             unitsofmeasure_response,
         )
     ]
 
-
+def get_esr_datareleasedate(api_key: str) -> List[ESRDataReleaseDateCleanedType]:
+    ENDPOINT: str = BASE_API + API_ID + DATA_RELEASE_DATES
+    response: requests.Response = generate_request(ENDPOINT, api_key=api_key)
+    datareleasedate_response: List[ESRDataReleaseDateType] = response.json()
+    return [
+        *map(
+            lambda entry: {
+                "commodity_code": entry['commodityCode'],
+                "market_year_start": datetime.strptime(
+                    entry['marketYearStart'], "%Y-%m-%dT%H:%M:%S"
+                ),
+                "market_year_end":  datetime.strptime(
+                    entry['marketYearEnd'], "%Y-%m-%dT%H:%M:%S"
+                ),
+                "market_year": entry['marketYear'],
+                "release_time_stamp": datetime.strptime(
+                    entry["releaseTimeStamp"], "%Y-%m-%dT%H:%M:%S"
+                ),
+            },
+            datareleasedate_response,
+        )
+    ]
+    
 def clean_country_exports(
     response: List[ESRCountryExportGeneralType],
 ) -> List[ESRCountryExportGeneralCleanedType]:
     return [
         *map(
             lambda entry: {
                 "commodity_code": entry["commodityCode"],
@@ -167,7 +191,11 @@
             countryCode=country_code,
             marketYear=market_year,
         )
     )
     response: requests.Response = generate_request(ENDPOINT, api_key=api_key)
     country_response: List[ESRCountryExportType] = response.json()
     return clean_country_exports(country_response)
+
+if __name__ == '__main__':
+    API_KEY = "f5458abd-198d-402b-b75e-3ce48527b0d2"
+    print(get_esr_datareleasedate(API_KEY))
```

### Comparing `usda_api-0.1.1/src/usda_api/scrapers/esr/schemas/response.py` & `usda_api-0.1.2/src/usda_api/scrapers/esr/schemas/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,21 @@
 
 class ESRCountriesType(BaseModel):
     countryCode: int
     countryName: str
     countryDescription: str
     regionId: int
     gencCode: str
-
+    
+class ESRDataReleaseDateType(BaseModel):
+    commodityCode: int
+    marketYearStart: str 
+    marketYearEnd: str
+    marketYear: int
+    releaseTimeStamp: str
 
 class ESRCountriesCleanedType(BaseModel):
     country_code: int
     country_name: str
     country_description: str
     region_id: int
     genc_code: str
@@ -34,14 +40,21 @@
     unitId: int
 
 
 class ESRCommoditiesCleanedType(BaseModel):
     commodity_code: int
     commodity_name: str
     unit_id: int
+    
+class ESRDataReleaseDateCleanedType(BaseModel):
+    commodity_code: int
+    market_year_start: datetime 
+    market_year_end: datetime
+    market_year: int
+    release_time_stamp: datetime
 
 
 class ESRUnitsOfMeasureType(BaseModel):
     unitId: str
     unitNames: str
```

### Comparing `usda_api-0.1.1/src/usda_api.egg-info/SOURCES.txt` & `usda_api-0.1.2/src/usda_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

