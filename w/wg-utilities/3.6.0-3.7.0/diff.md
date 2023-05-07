# Comparing `tmp/wg_utilities-3.6.0.tar.gz` & `tmp/wg_utilities-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.6.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.7.0.tar", max compression
```

## Comparing `wg_utilities-3.6.0.tar` & `wg_utilities-3.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/README.md
--rw-r--r--   0        0        0     4825 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      685 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4305 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24119 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56658 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7692 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13531 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15915 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    27248 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    50664 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22398 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/README.md
+-rw-r--r--   0        0        0     4825 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      685 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4207 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    23741 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56658 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7580 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13265 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15915 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    27248 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    51568 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22398 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.7.0/PKG-INFO
```

### Comparing `wg_utilities-3.6.0/LICENSE` & `wg_utilities-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/README.md` & `wg_utilities-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/pyproject.toml` & `wg_utilities-3.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.6.0"
+version = "3.7.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.6.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.7.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.7.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/_google.py` & `wg_utilities-3.7.0/wg_utilities/clients/_google.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,36 +26,36 @@
     "GetJsonResponseGoogleClient", bound=Mapping[Any, Any]
 )
 
 
 class _PaginatedResponseBase(TypedDict):
     """Typing info for a paginated response."""
 
-    accessRole: str  # noqa: N815
-    defaultReminders: list[dict[str, object]]  # noqa: N815
+    accessRole: str
+    defaultReminders: list[dict[str, object]]
     etag: str
     kind: Literal["calendar#events"]
-    nextPageToken: str  # noqa: N815
+    nextPageToken: str
     summary: str
-    timeZone: str  # noqa: N815
+    timeZone: str
     updated: str
 
 
 class PaginatedResponseCalendar(_PaginatedResponseBase):
     """Paginated response specifically for the Calendar client."""
 
     items: list[GoogleCalendarEntityJson]
 
 
 class PaginatedResponseFit(TypedDict):
     """Paginated response specifically for the Fit client."""
 
-    minStartTimeNs: str  # noqa: N815
-    maxEndTimeNs: str  # noqa: N815
-    dataSourceId: str  # noqa: N815
+    minStartTimeNs: str
+    maxEndTimeNs: str
+    dataSourceId: str
     point: list[dict[str, object]]
 
 
 class PaginatedResponsePhotos(_PaginatedResponseBase):
     """Paginated response specifically for the Photos client."""
 
     albums: list[GooglePhotosEntityJson]
```

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.7.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.7.0/wg_utilities/clients/google_calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,42 +52,42 @@
     response_status: ResponseStatus = Field(
         alias="responseStatus", default=ResponseStatus.UNKNOWN
     )
     self: bool = False
 
 
 class _ConferenceDataCreateRequest(TypedDict):
-    requestId: str  # noqa: N815
-    conferenceSolutionKey: dict[Literal["type"], Literal["hangoutsMeet"]]  # noqa: N815
+    requestId: str
+    conferenceSolutionKey: dict[Literal["type"], Literal["hangoutsMeet"]]
     status: dict[Literal["statusCode"], Literal["success"]]
 
 
 class _ConferenceDataEntryPoints(TypedDict, total=False):
-    entryPointType: str  # noqa: N815
+    entryPointType: str
     uri: str
     label: str
     pin: str | None
-    accessCode: str | None  # noqa: N815
-    meetingCode: str | None  # noqa: N815
+    accessCode: str | None
+    meetingCode: str | None
     passcode: str | None
     password: str | None
-    regionCode: str | None  # noqa: N815
+    regionCode: str | None
 
 
 class _ConferenceDataConferenceSolution(TypedDict):
     key: dict[Literal["type"], Literal["hangoutsMeet", "addOn"]]
     name: str
-    iconUri: str  # noqa: N815
+    iconUri: str
 
 
 class _ConferenceData(TypedDict, total=False):
-    createRequest: _ConferenceDataCreateRequest  # noqa: N815
-    entryPoints: list[_ConferenceDataEntryPoints]  # noqa: N815
-    conferenceSolution: _ConferenceDataConferenceSolution  # noqa: N815
-    conferenceId: str  # noqa: N815
+    createRequest: _ConferenceDataCreateRequest
+    entryPoints: list[_ConferenceDataEntryPoints]
+    conferenceSolution: _ConferenceDataConferenceSolution
+    conferenceId: str
     signature: str | None
     notes: str | None
     parameters: dict[str, object] | None
 
 
 class _Creator(BaseModelWithConfig):  # pylint: disable=too-few-public-methods
     display_name: str | None = Field(alias="displayName", default=None)
@@ -140,16 +140,16 @@
     description: str | None
     etag: str
     id: str
     location: str | None
     summary: str
 
     kind: Literal["calendar#calendar"]
-    timeZone: str  # noqa: N815
-    conferenceProperties: dict[  # noqa: N815
+    timeZone: str
+    conferenceProperties: dict[
         Literal["allowedConferenceSolutionTypes"],
         list[Literal["eventHangout", "eventNamedHangout", "hangoutsMeet"]],
     ]
 
 
 FJR = TypeVar("FJR", bound="GoogleCalendarEntity")
 
@@ -444,36 +444,36 @@
     etag: str
     id: str
     location: str | None
     summary: str | None
 
     attachments: list[dict[str, str]] | None
     attendees: list[_Attendee] | None
-    attendeesOmitted: bool | None  # noqa: N815
+    attendeesOmitted: bool | None
     created: datetime_
-    colorId: str | None  # noqa: N815
-    conferenceData: _ConferenceData | None  # noqa: N815
+    colorId: str | None
+    conferenceData: _ConferenceData | None
     creator: _Creator
     end: _StartEndDatetime
-    endTimeUnspecified: bool | None  # noqa: N815
-    eventType: EventType  # "default"  # noqa: N815
-    extendedProperties: dict[str, dict[str, str]] | None  # noqa: N815
-    guestsCanInviteOthers: bool | None  # noqa: N815
-    guestsCanModify: bool | None  # noqa: N815
-    guestsCanSeeOtherGuests: bool | None  # noqa: N815
-    hangoutLink: str | None  # noqa: N815
-    htmlLink: str  # noqa: N815
-    iCalUID: str  # noqa: N815
+    endTimeUnspecified: bool | None
+    eventType: EventType  # "default"
+    extendedProperties: dict[str, dict[str, str]] | None
+    guestsCanInviteOthers: bool | None
+    guestsCanModify: bool | None
+    guestsCanSeeOtherGuests: bool | None
+    hangoutLink: str | None
+    htmlLink: str
+    iCalUID: str
     kind: Literal["calendar#event"]
     locked: bool | None
     organizer: dict[str, bool | str]
     original_start_time: dict[str, str] | None
-    privateCopy: bool | None  # noqa: N815
+    privateCopy: bool | None
     recurrence: list[str] | None
-    recurringEventId: str | None  # noqa: N815
+    recurringEventId: str | None
     reminders: dict[str, bool | dict[str, str | int]]
     sequence: int
     source: dict[str, str] | None
     start: _StartEndDatetime
     status: Literal["cancelled", "confirmed", "tentative"] | None
     transparency: str | None
     updated: datetime_
```

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.7.0/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.7.0/wg_utilities/clients/google_fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 class _DataSourceDataTypeInfo(TypedDict):
     field: list[_DataSourceDataTypeFieldInfo]
     name: str
 
 
 class _DataSourceDescriptionInfo(TypedDict):
     application: dict[str, str]
-    dataStreamId: str  # noqa: N815
-    dataStreamName: str  # noqa: N815
-    dataType: _DataSourceDataTypeInfo  # noqa: N815
+    dataStreamId: str
+    dataStreamName: str
+    dataType: _DataSourceDataTypeInfo
 
 
 class _GoogleFitDataPointInfo(TypedDict):
     id: str
-    startTimeNanos: str  # noqa: N815
-    endTimeNanos: str  # noqa: N815
-    dataTypeName: str  # noqa: N815
-    originDataSourceId: str  # noqa: N815
+    startTimeNanos: str
+    endTimeNanos: str
+    dataTypeName: str
+    originDataSourceId: str
     value: list[dict[str, int]]
 
 
 class DataSource:
     """Class for interacting with Google Fit Data Sources.
 
     An example of a data source is Strava, Google Fit, MyFitnessPal, etc. The ID is
@@ -53,15 +53,15 @@
         "floatPoint": "fpVal",
         "integer": "intVal",
     }
 
     class DataPointValueKeyLookupInfo(TypedDict):
         """Typing info for the Data Point lookup dict."""
 
-        floatPoint: Literal["fpVal"]  # noqa: N815
+        floatPoint: Literal["fpVal"]
         integer: Literal["intVal"]
 
     def __init__(self, data_source_id: str, *, google_client: GoogleFitClient):
         self.data_source_id = data_source_id
         self.url = f"/users/me/dataSources/{self.data_source_id}"
         self.google_client = google_client
```

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.7.0/wg_utilities/clients/google_photos.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(DEBUG)
 add_stream_handler(LOGGER)
 
 
 class _SharedAlbumOptionsInfo(TypedDict):
-    isCollaborative: bool  # noqa: N815
-    isCommentable: bool  # noqa: N815
+    isCollaborative: bool
+    isCommentable: bool
 
 
 class _ShareInfoInfo(TypedDict):
-    isJoinable: bool  # noqa: N815
-    isJoined: bool  # noqa: N815
-    isOwned: bool  # noqa: N815
-    shareableUrl: str  # noqa: N815
-    sharedAlbumOptions: _SharedAlbumOptionsInfo  # noqa: N815
-    shareToken: str  # noqa: N815
+    isJoinable: bool
+    isJoined: bool
+    isOwned: bool
+    shareableUrl: str
+    sharedAlbumOptions: _SharedAlbumOptionsInfo
+    shareToken: str
 
 
 class _MediaItemMetadataPhoto(BaseModelWithConfig):
     camera_make: str | None = Field(alias="cameraMake")
     camera_model: str | None = Field(alias="cameraModel")
     focal_length: float | None = Field(alias="focalLength")
     aperture_f_number: float | None = Field(alias="apertureFNumber")
@@ -104,21 +104,21 @@
         return instance
 
 
 class AlbumJson(TypedDict):
     """JSON representation of an Album."""
 
     id: str
-    productUrl: str  # noqa: N815
+    productUrl: str
 
-    coverPhotoBaseUrl: str  # noqa: N815
-    coverPhotoMediaItemId: str  # noqa: N815
-    isWriteable: bool | None  # noqa: N815
-    mediaItemsCount: int  # noqa: N815
-    shareInfo: _ShareInfoInfo | None  # noqa: N815
+    coverPhotoBaseUrl: str
+    coverPhotoMediaItemId: str
+    isWriteable: bool | None
+    mediaItemsCount: int
+    shareInfo: _ShareInfoInfo | None
     title: str
 
 
 class Album(GooglePhotosEntity):
     """Class for Google Photos albums and their metadata/content."""
 
     cover_photo_base_url: str = Field(alias="coverPhotoBaseUrl")
@@ -170,22 +170,22 @@
         return item.id in [media_item.id for media_item in self.media_items]
 
 
 class MediaItemJson(TypedDict):
     """JSON representation of a Media Item (photo or video)."""
 
     id: str
-    productUrl: str  # noqa: N815
+    productUrl: str
 
-    baseUrl: str  # noqa: N815
-    contributorInfo: dict[str, str] | None  # noqa: N815
+    baseUrl: str
+    contributorInfo: dict[str, str] | None
     description: str | None
     filename: str
-    mediaMetadata: _MediaItemMetadata  # noqa: N815
-    mimeType: str  # noqa: N815
+    mediaMetadata: _MediaItemMetadata
+    mimeType: str
 
 
 class MediaItem(GooglePhotosEntity):
     """Class for representing a MediaItem and its metadata/content."""
 
     base_url: str = Field(alias="baseUrl")
     contributor_info: dict[str, str] | None = Field(alias="contributorInfo")
```

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.7.0/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.7.0/wg_utilities/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.7.0/wg_utilities/clients/spotify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1188,14 +1188,16 @@
             other.id.lower(),
         )
 
 
 class User(SpotifyEntity[UserSummaryJson]):
     """A Spotify user, usually just the current user."""
 
+    PLAYLIST_REFRESH_INTERVAL: ClassVar[timedelta] = timedelta(minutes=10)
+
     display_name: str
     country: str | None
     email: str | None
     explicit_content: dict[str, bool] | None
     followers: Followers | None
     images: list[Image] | None
     product: str | None
@@ -1204,14 +1206,16 @@
     _albums: list[Album]
     _artists: list[Artist]
     _playlists: list[Playlist]
     _top_artists: tuple[Artist, ...]
     _top_tracks: tuple[Track, ...]
     _tracks: list[Track]
 
+    _playlist_refresh_time: datetime
+
     sj_type: ClassVar[type_[SpotifyEntityJson]] = UserSummaryJson
 
     @validator("display_name", pre=True)
     def set_user_name_value(
         cls, value: str, values: dict[str, Any]  # noqa: N805
     ) -> str:
         """Set the user's `name` field to the display name if it is not set.
@@ -1491,25 +1495,44 @@
     def playlists(self) -> list[Playlist]:
         """Return a list of playlists owned by the current user.
 
         Returns:
             list: a list of playlists owned by the current user
         """
 
+        if (
+            hasattr(self, "_playlist_refresh_time")
+            and (datetime.utcnow() - self._playlist_refresh_time)
+            < self.PLAYLIST_REFRESH_INTERVAL
+        ):
+            return self._playlists
+
+        self._set_private_attr("_playlist_refresh_time", datetime.utcnow())
+
+        all_playlist_json = cast(
+            list[PlaylistSummaryJson], self.spotify_client.get_items("/me/playlists")
+        )
+
         if not hasattr(self, "_playlists"):
             playlists = [
                 Playlist.from_json_response(item, spotify_client=self.spotify_client)
-                for item in cast(
-                    list[PlaylistSummaryJson],
-                    self.spotify_client.get_items("/me/playlists"),
-                )
+                for item in all_playlist_json
                 if item["owner"]["id"] == self.id
             ]
 
             self._set_private_attr("_playlists", playlists)
+        else:
+            existing_ids = (p.id for p in self._playlists)
+            new_playlists = [
+                Playlist.from_json_response(item, spotify_client=self.spotify_client)
+                for item in all_playlist_json
+                if item["owner"]["id"] == self.id and item["id"] not in existing_ids
+            ]
+
+            self._playlists.extend(new_playlists)
 
         return self._playlists
 
     @property
     def top_artists(self) -> tuple[Artist, ...]:
         """Top artists for the user.
 
@@ -1602,12 +1625,15 @@
             "tracks",
         ]
 
         for prop_name in property_names:
             if hasattr(self, attr_name := f"_{prop_name}"):
                 delattr(self, attr_name)
 
+        if "playlists" in property_names:
+            delattr(self, "_playlist_refresh_time")
+
 
 SpotifyEntity.update_forward_refs()
 Album.update_forward_refs()
 Artist.update_forward_refs()
 Track.update_forward_refs()
```

### Comparing `wg_utilities-3.6.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.7.0/wg_utilities/clients/truelayer.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.7.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.7.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.7.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.7.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.7.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.7.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.7.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.7.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.7.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/json.py` & `wg_utilities-3.7.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/processes.py` & `wg_utilities-3.7.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.7.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/functions/xml.py` & `wg_utilities-3.7.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.7.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.7.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.6.0/PKG-INFO` & `wg_utilities-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.6.0
+Version: 3.7.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

