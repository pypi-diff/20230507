# Comparing `tmp/zipline_norgatedata-2.3.4-py3-none-any.whl.zip` & `tmp/zipline_norgatedata-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 46621 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat     9227 b- defN 23-Feb-22 10:07 zipline_norgatedata/CHANGES.txt
+Zip file size: 36244 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     9308 b- defN 23-May-01 01:30 zipline_norgatedata/CHANGES.txt
 -rw-rw-rw-  2.0 fat    16020 b- defN 20-Sep-09 09:35 zipline_norgatedata/LICENSE.txt
--rw-rw-rw-  2.0 fat    31390 b- defN 20-Dec-08 23:36 zipline_norgatedata/README-Zipline130.md
 -rw-rw-rw-  2.0 fat       62 b- defN 19-Aug-27 04:23 zipline_norgatedata/__init__.py
--rw-rw-rw-  2.0 fat    10990 b- defN 21-Jun-20 12:54 zipline_norgatedata/pipelines.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Feb-22 10:09 zipline_norgatedata/version.py
--rw-rw-rw-  2.0 fat    40923 b- defN 22-Aug-10 01:16 zipline_norgatedata/zipline_norgatedata.py
--rw-rw-rw-  2.0 fat    16020 b- defN 23-Feb-22 10:28 zipline_norgatedata-2.3.4.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    28063 b- defN 23-Feb-22 10:28 zipline_norgatedata-2.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-22 10:28 zipline_norgatedata-2.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Feb-22 10:28 zipline_norgatedata-2.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1088 b- defN 23-Feb-22 10:28 zipline_norgatedata-2.3.4.dist-info/RECORD
-12 files, 153918 bytes uncompressed, 44767 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat    10981 b- defN 23-May-01 11:22 zipline_norgatedata/pipelines.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-01 01:29 zipline_norgatedata/version.py
+-rw-rw-rw-  2.0 fat    43970 b- defN 23-May-05 08:06 zipline_norgatedata/zipline_norgatedata.py
+-rw-rw-rw-  2.0 fat    16020 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    25842 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      990 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/RECORD
+11 files, 123328 bytes uncompressed, 34546 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: zipline_norgatedata/CHANGES.txt
 Comment: 
 
 Filename: zipline_norgatedata/LICENSE.txt
 Comment: 
 
-Filename: zipline_norgatedata/README-Zipline130.md
-Comment: 
-
 Filename: zipline_norgatedata/__init__.py
 Comment: 
 
 Filename: zipline_norgatedata/pipelines.py
 Comment: 
 
 Filename: zipline_norgatedata/version.py
 Comment: 
 
 Filename: zipline_norgatedata/zipline_norgatedata.py
 Comment: 
 
-Filename: zipline_norgatedata-2.3.4.dist-info/LICENSE.TXT
+Filename: zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: zipline_norgatedata-2.3.4.dist-info/METADATA
+Filename: zipline_norgatedata-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: zipline_norgatedata-2.3.4.dist-info/WHEEL
+Filename: zipline_norgatedata-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: zipline_norgatedata-2.3.4.dist-info/top_level.txt
+Filename: zipline_norgatedata-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: zipline_norgatedata-2.3.4.dist-info/RECORD
+Filename: zipline_norgatedata-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zipline_norgatedata/CHANGES.txt

```diff
@@ -108,7 +108,8 @@
 v2.2.9 20220715 Documentation change only - force install of iso3166 package to 2.0.2 due to change in name of "Turkey"
 v2.2.10 20220728 Updated iso3166 to be installed via mamba instead of pip
 v2.3.0 20220728 Bump to v2.3.0 due to version checking issue
 v2.3.1 20221027 Added Mac M1/M2 workaround to docs
 v2.3.2 20221114 Notes on Juneteenth holiday patch
 v2.3.3 20230122 Notes on TSXFailures patch
 v2.3.4 20230222 Update documentation to specify sqlalchemy<2
+v2.4.0 20230501 Change to zipline-reloaded and pyfolio-reloaded via conda-forge
```

## zipline_norgatedata/pipelines.py

```diff
@@ -185,14 +185,15 @@
             "Pipeline "
             + self.__class__.__name__
             + " populating on "
             + str(assets.size)
             + " securities"
         )
         norgatetimeseriesfunction = norgatedata.padding_status_timeseries
+
         result = ConvertNorgateBoolTimeSeriesToFilter(
             assets, norgatetimeseriesfunction, dates, mask
         )
         logger.info("Pipeline " + self.__class__.__name__ + ": Done")
         return result
 
     # def graph_repr(self):
@@ -202,15 +203,15 @@
 class NorgateDataUnadjustedClose(Factor):
     """
     A Filter that returns the unadjusted close of the security
 
     """
 
     window_length = 1
-    dtype = np.float
+    dtype = float
     inputs = []
     window_safe = True
 
     def _compute(self, arrays, dates, assets, mask):
         logger.info(
             "Pipeline "
             + self.__class__.__name__
@@ -228,15 +229,15 @@
 
 class NorgateDataDividendYield(Factor):
     """
     A Filter that computes the dividend yield of a stock based upon a 12 month rolling window, with some smarts to handle variations in dates
     """
 
     window_length = 1
-    dtype = np.float
+    dtype = float
     inputs = []
     window_safe = True
 
     def _compute(self, arrays, dates, assets, mask):
         logger.info(
             "Pipeline "
             + self.__class__.__name__
@@ -271,15 +272,15 @@
     timeseries = norgatetimeseriesfunction(
         symbol=symbol,
         padding_setting=norgatedata.PaddingType.ALLMARKETDAYS,
         timeseriesformat="pandas-dataframe",
         start_date=start_date,
         end_date=end_date,
         datetimeformat="datetime64nsutc",
-        timezone="UTC",
+        timezone=None,
     )
     timeseries = timeseries.reindex(dates, fill_value=0)
     out[:, assetindexcounter] = timeseries.iloc[:, 0] == 1
 
 
 def ConvertNorgateBoolTimeSeriesToFilter(
     assets, norgatetimeseriesfunction, dates, mask
@@ -331,27 +332,27 @@
     timeseries = norgatetimeseriesfunction(
         symbol=symbol,
         padding_setting=norgatedata.PaddingType.ALLMARKETDAYS,
         timeseriesformat="pandas-dataframe",
         start_date=start_date,
         end_date=end_date,
         datetimeformat="datetime64nsutc",
-        timezone="UTC",
+        timezone=None,
     )
     out[:, assetindexcounter] = timeseries.reindex(
         dates, fill_value=0, copy=False
     ).values[:, 0]
 
 
 def ConvertNorgateFloatTimeSeriesToFactor(
     assets, norgatetimeseriesfunction, dates, mask
 ):
     start_date = dates[0].to_pydatetime()
     end_date = dates[-1].to_pydatetime()
-    out = np.full_like(mask, np.nan, dtype=np.float, order="K")  # Fill with NaN
+    out = np.full_like(mask, np.nan, dtype=float, order="K")  # Fill with NaN
     assetindexcounter = 0
     for zipline_assetid in assets:
         symbol = sid(zipline_assetid).symbol
         PopulateFactor(
             symbol,
             norgatetimeseriesfunction,
             start_date,
```

## zipline_norgatedata/version.py

```diff
@@ -1 +1 @@
-__version__ = '2.3.4'
+__version__ = '2.4.0'
```

## zipline_norgatedata/zipline_norgatedata.py

```diff
@@ -11,18 +11,15 @@
     "__version__",
     "__author__",
 ]
 import sys
 from zipline.data.bundles import register
 import pandas as pd
 import zipline as zl
-if zl.__version__ < '2.2.0':
-    from trading_calendars import get_calendar
-else:
-    from exchange_calendars import get_calendar
+from exchange_calendars import get_calendar
 import norgatedata
 from numpy import empty, where
 import re
 from zipline.utils.cli import maybe_show_progress
 import logbook
 from os import environ, cpu_count
 import requests
@@ -109,28 +106,39 @@
     "FOAT4": "O4", # French govt bond (OAT) - day
     "FOAT9": "O9", # French govt bond (OAT) - Official Close
     "HTW": "TW",  # MSCI Taiwan 
     "HTW4": "T4",  # MSCI Taiwan (Day session)
 
 }
 
-
-def normalize_daily_start_end_session(calendar_name, start_session, end_session):
+def normalize_daily_start_end_session_OLD(calendar_name, start_session, end_session):
     if zl.__version__ < '2.2.0':
         cal = get_calendar(calendar_name)
     else:
         cal = get_calendar(calendar_name,start=start_session.strftime("%Y-%m-%d"))
     if not (cal.is_session(start_session)):
         # use next close instead of next open due to futures markets that start on Sundays
         # and we only want daily data
         start_session = cal.next_close(start_session).floor(freq="D")
     if not (cal.is_session(end_session)):
         end_session = cal.previous_close(end_session).floor(freq="D")
     return start_session, end_session
 
+def normalize_daily_start_end_session(calendar_name, start_session, end_session):
+    cal = get_calendar(calendar_name,start=start_session.strftime("%Y-%m-%d"))
+
+    if not (cal.is_session(start_session)):
+        # use next close instead of next open due to futures markets that start on Sundays
+        # and we only want daily data
+        start_session = cal.next_close(start_session).floor(freq="D")
+    if not (cal.is_session(end_session)):
+        end_session = cal.previous_close(end_session).floor(freq="D")
+
+    return start_session, end_session
+
 def define_non_US_country_code(exchanges):
     aulist = ('ASX','AU IDX')
     for exchange in aulist:
         #if exchanges.index.contains(exchange):
         if exchange in exchanges.index:
             exchanges.at[exchange,'country_code'] = 'AU'
     calist = ('TSX','TSX Venture','TSX Venture NEX','CSE','NEO','CA IDX')
@@ -521,42 +529,42 @@
         for symbol in reversed(
             symbols
         ):  # Do in reversed order, because we will be deleting some symbols and this
             # messes up iteration
             if excluded_symbol_list is not None and symbol in excluded_symbol_list:
                 symbols.remove(symbol)
                 continue
-            fqd = norgatedata.first_quoted_date(symbol)
+            fqd = norgatedata.first_quoted_date(symbol, tz=None)
             if fqd is None or fqd == "9999-12-31":
                 symbols.remove(symbol)
                 continue
-            fqd = pd.Timestamp(fqd, tz="utc")
+            fqd = pd.Timestamp(fqd, tz=None)
             if fqd > enddate:
                 symbols.remove(symbol)
                 continue
-            lqd = norgatedata.last_quoted_date(symbol)
+            lqd = norgatedata.last_quoted_date(symbol, tz=None)
             if not (lqd is None or lqd == "9999-12-31"):
-                lqd = pd.Timestamp(lqd, tz="utc")
+                lqd = pd.Timestamp(lqd, tz=None)
                 if lqd < startdate:
                     symbols.remove(symbol)
     
     revisedsymbols = []
     for symbol in symbols:  
         # messes up iteration
         if excluded_symbol_list is not None and symbol in excluded_symbol_list:
             continue
-        fqd = norgatedata.first_quoted_date(symbol)
+        fqd = norgatedata.first_quoted_date(symbol, tz=None)
         if fqd is None or fqd == "9999-12-31":
             continue
-        fqd = pd.Timestamp(fqd, tz="utc")
+        fqd = pd.Timestamp(fqd, tz=None)
         if fqd > enddate:
             continue
-        lqd = norgatedata.last_quoted_date(symbol)
+        lqd = norgatedata.last_quoted_date(symbol, tz=None)
         if not (lqd is None or lqd == "9999-12-31"):
-            lqd = pd.Timestamp(lqd, tz="utc")
+            lqd = pd.Timestamp(lqd, tz=None)
             if lqd < startdate:
                 continue
         revisedsymbols.append(symbol)
     revisedsymbols.sort()
     logger.info(
         "Metadata process complete.  Revised security count: " + str(len(revisedsymbols))
     )
@@ -611,28 +619,33 @@
     revisedsymbols = []
     for symbol in symbols:
         if excluded_symbol_list is not None and symbol in excluded_symbol_list:
             continue
         fqd = norgatedata.first_quoted_date(symbol)
         if fqd is None or fqd == "9999-12-31":
             continue
-        fqd = pd.Timestamp(fqd, tz="utc")
+        fqd = pd.Timestamp(fqd, tz=None)
         if fqd > enddate:
             continue
-        lqd = norgatedata.last_quoted_date(symbol)
+        lqd = norgatedata.last_quoted_date(symbol, tz=None)
         if lqd is not None:
-            lqdtimestamp = pd.Timestamp(lqd, tz="utc")
+            lqdtimestamp = pd.Timestamp(lqd, tz=None)
             if lqdtimestamp < startdate:
                 continue
+        notice_date = norgatedata.first_notice_date(symbol, tz=None)
+        if notice_date is not None and pd.Timestamp(notice_date,tz=None) <= startdate: # Not much point including this delivery if FND is on or prior to startdate
+            continue
+
         if norgatedata.base_type(symbol) == "Futures Market":
             if (lqd is None or lqd == "9999-12-31") and not symbol.startswith('&'):
                 logger.info("Newly listed futures contract " + symbol + " ignored due to incomplete metadata")
                 continue
             session_symbol = norgatedata.futures_market_session_symbol(symbol)
-            root_symbol = translate_futures_symbol(session_symbol)
+            #root_symbol = translate_futures_symbol(session_symbol) # Zipline 2.4 extends root symbol to more than 2 characters, so no need to do this any more
+            root_symbol = session_symbol
             if len(root_symbol) > 0 and not root_symbol in root_symbols:
                 root_symbols.add(root_symbol)
                 exchange = norgatedata.exchange_name(symbol)
                 exchanges[root_symbol] = exchange
                 marketname = norgatedata.futures_market_session_name(symbol)
                 marketnames[root_symbol] = marketname
                 sector = norgatedata.classification(
@@ -666,15 +679,15 @@
     marketnames = pd.Series(marketnames)
     exchanges = pd.Series(exchanges)
     sectors = pd.Series(sectors)
     root_symbols["description"] = marketnames[root_symbols["root_symbol"]].tolist()
     root_symbols["exchange"] = exchanges[root_symbols["root_symbol"]].tolist()
     root_symbols["sector"] = sectors[root_symbols["root_symbol"]].tolist()
     logger.info(
-        "Metadata process complete.  Revised security count: " + str(len(symbols))
+        "Metadata process complete.  Revised security count: " + str(len(revisedsymbols))
     )
     return revisedsymbols, root_symbols
 
 def _pricing_iter_equities(
     symbols,
     metadata,
     sessions,
@@ -701,15 +714,15 @@
                 timeseriesformat="pandas-dataframe-zipline",
                 start_date=start_session,
                 end_date=end_session,
                 stock_price_adjustment_setting=stock_price_adjustment_setting,
                 padding_setting=norgatedata.PaddingType.ALLMARKETDAYS,  # Must do this - Zipline can only market day padded data
                 fields=["Open", "High", "Low", "Close", "Volume"],
                 datetimeformat="datetime64nsutc",
-                timezone="UTC",
+                timezone=None,
             )
 
             start_date = df.index[0]
             end_date = df.index[-1]
 
             # Add missing columns
             if not "volume" in df.columns:
@@ -721,15 +734,15 @@
             # Zipline can't handle crazy volumes for stocks where there have been lots of splits
             # Turn adjusted volume data into max UINT32 of 4294967295
             if "volume" in df.columns:
                 df["volume"] = where(
                     df["volume"] > 4294967295, 4294967295, df["volume"]
                 )
             slqd = norgatedata.second_last_quoted_date(
-                symbol, datetimeformat="pandas-timestamp"
+                symbol, datetimeformat="pandas-timestamp", tz=None
             )
             if slqd is None:
                 ac_date = end_date + BDay(1) # Set bogus autoclose date after end date
             else:
                 ac_date = slqd
             norgate_data_symbol = symbol
             norgate_data_assetid = norgatedata.assetid(symbol)
@@ -759,14 +772,17 @@
                 start_date,
             )
             yield sid, df
 
 
 ################################################
 def translate_futures_symbol(symbol):
+    # This was required for Zipline 2.2 for two character root, but has been enhanced in 2.4 to offer multi-character root.  However, still requires MYY format where M is alphabetic month and YY = year
+    #  but Zipline 2.4 adds multicharacter root systems to futures
+    # so this is no longer needed
     newsymbol = symbol
     if symbol[0] == "&":  # Continuous futures, strip leading &
         newsymbol = symbol[1:]
     if not symbol[0].isalnum():
         return newsymbol
     match = re.search("^([0-9A-Z]+)-(\d\d)(\d\d)([A-Z])", newsymbol)
     if match:
@@ -775,72 +791,97 @@
         newsymbol = _symbol_translate[newsymbol]
     elif len(symbol) >= 3:
         newsymbol = newsymbol[0:2]
     if match:
         newsymbol += match.group(4) + match.group(3)
     return newsymbol
 
+def translate_futures_symbol(symbol):
+    # This was required for Zipline 2.2 but Zipline 2.4 adds multicharacter root systems to futures
+    # so this is no longer needed
+    newsymbol = symbol
+    if symbol[0] == "&":  # Continuous futures, strip leading &
+        newsymbol = symbol[1:]
+    if not symbol[0].isalnum():
+        return newsymbol
+    match = re.search("^([0-9A-Z]+)-(\d\d)(\d\d)([A-Z])", newsymbol)
+    if match:
+        newsymbol = match.group(1)
+    #if newsymbol in _symbol_translate:
+    #    newsymbol = _symbol_translate[newsymbol]
+    #elif len(symbol) >= 3:
+    #    newsymbol = newsymbol[0:2]
+    if match:
+        newsymbol += match.group(4) + match.group(3)
+    return newsymbol
+
 def _progress_symbol(a):
     if a is None: 
         return ""
     else:
         return a
 
 def _pricing_iter_futures(
     symbols, metadata, sessions, show_progress, start_session, end_session
 ):
     with maybe_show_progress(
         symbols, show_progress, label="Loading Norgate futures:", item_show_func=lambda a:_progress_symbol(a),
     ) as it:
         for sid, symbol in enumerate(it):
-            # 2000 is the maximum here - anything before is not defined as a
-            # session apparently (!) - probably the calendars need work in
-            # zipline
             # Padding must be all market days, otherwise it will bork zipline's
             # expection that there's a bar for every day
             # Open interest is here even though zipline can't yet use it
             df = norgatedata.price_timeseries(
                 symbol,
                 timeseriesformat="pandas-dataframe-zipline",
                 start_date="1970-01-01",
                 padding_setting=norgatedata.PaddingType.ALLMARKETDAYS,
                 stock_price_adjustment_setting=norgatedata.StockPriceAdjustmentType.NONE,
-                datetimeformat="datetime64nsutc",
-                timezone="UTC",
+                datetimeformat="datetime64ns",
+                timezone=None,
             )
             # Add missing columns
             if not "volume" in df.columns:
                 df["volume"] = 0
             if not "open interest" in df.columns:
                 df["open interest"] = 0
             # Zipline can't handle volumes above 4294967295, so for indices, we'll divide by 1000.
             # Many indices including S&P 500, Russell 3000 etc. have this level of volume
             if norgatedata.subtype1(symbol) == "Index":
                 df.loc[:, "volume"] /= 1000
             # Zipline can't handle crazy volumes for stocks where there have been lots of splits
             # Turn adjusted volume data into max UINT32 of 4294967295
             df["volume"] = where(df["volume"] > 4294967295, 4294967295, df["volume"])
+            # Zipline can't handle negative numbers since it internally stores data as uint32
+            # This happened in Crude Oil in 2020
+            # so it will be set to zero until Zipline can handle it
+            # Most traders would have already rolled anyway, so not a real big issue
+            df["open"] = where(df["open"] < 0, 0, df["open"])
+            df["high"] = where(df["high"] < 0, 0, df["high"])
+            df["low"] = where(df["low"] < 0, 0, df["low"])
+            df["close"] = where(df["close"] < 0, 0, df["close"])
             asset_name = norgatedata.security_name(symbol)
             exchange = norgatedata.exchange_name(symbol)
             exchange_full = norgatedata.exchange_name_full(symbol)
             norgate_data_symbol = symbol
             norgate_data_assetid = norgatedata.assetid(symbol)
             notice_date = norgatedata.first_notice_date(
-                symbol, datetimeformat="pandas-timestamp"
+                symbol, datetimeformat="pandas-timestamp", tz=None
             )
 
             expiration_date = norgatedata.last_quoted_date(
-                symbol, datetimeformat="pandas-timestamp"
+                symbol, datetimeformat="pandas-timestamp", tz=None
             )
             if norgatedata.base_type(symbol) == "Futures Market":
                 tick_size = norgatedata.tick_size(symbol)
                 multiplier = norgatedata.point_value(symbol)
-                root_symbol = translate_futures_symbol(
-                    norgatedata.futures_market_session_symbol(symbol)
-                )
+                #root_symbol = translate_futures_symbol(
+                #    norgatedata.futures_market_session_symbol(symbol)
+                #)
+                root_symbol = norgatedata.futures_market_session_symbol(symbol)
                 symbol = translate_futures_symbol(symbol)
                 asset_type = "futures"
             else:
                 tick_size = 0.0001
                 multiplier = 1
                 root_symbol = symbol
                 asset_type = "equities"
@@ -848,49 +889,17 @@
                 logger.info(
                     "Futures contract found with no price data: " + symbol + "(perhaps it has just been listed and the exchange has not yet sent down trading prices)... skipping"
                 )
                 continue
             start_date = None
             end_date = None
             ac_date = None
-
             if len(df.index) > 0:
                 start_date = df.index[0]
                 end_date = df.index[-1]
-
-            if notice_date is not None:
-                # ac_date = df.index[df.index.searchsorted(pd.Timestamp(notice_date)) - 1] # Day prior to FND.  This method was used prior to 20200713
-                if df.index[-1] >= pd.Timestamp(notice_date):
-                    if len(df.index) > 2:
-                        ac_date = df.index[
-                            df.index.searchsorted(pd.Timestamp(notice_date)) - 2
-                        ]  # 2 days prior to FND
-                    else:
-                        ac_date = pd.Timestamp(notice_date) - BDay(2)
-                else:
-                    ac_date = pd.Timestamp(notice_date) - BDay(2)
-            elif expiration_date is not None:
-                # ac_date = pd.Timestamp(expiration_date, tz="utc") # This method was used prior to 20200713
-                if df.index[-1] >= pd.Timestamp(expiration_date): # Last value is on or after expiration date
-                    if len(df.index) > 2:
-                        ac_date = df.index[
-                            df.index.searchsorted(pd.Timestamp(expiration_date)) - 2
-                        ]  # second last trading date, as determined by the data
-                    else:
-                        ac_date = pd.Timestamp(notice_date) - BDay(2) # Corner case - perhaps we are ingesting around a boundary of expiration
-                else:
-                    ac_date = pd.Timestamp(expiration_date) - BDay(2)
-
-            if ac_date is None: # Every futures contract needs an autoclose date of some sort
-                expiration_date = end_date + BDay(1) # Set a bogus date
-                ac_date = pd.Timestamp(expiration_date) - BDay(2)
-
-            if notice_date is None:
-                notice_date = expiration_date + BDay(1)  # Put a notice date 1 day after expiration
-
             all_dates = sessions.snap("D")
             valid_dates = all_dates.slice_indexer(start=start_date, end=end_date)
 
             # Check if the first date from valid_dates exists in df - if not, we have to pad this ourselves so that the forward fill works in the future
             if (
                 len(all_dates[valid_dates]) > 0
                 and all_dates[valid_dates][0] not in df.index
@@ -903,28 +912,69 @@
                     all_dates[single_date_slice], method="ffill"
                 )
                 # Now set OHL to Close, vol to zero
                 single_date_df["open"] = single_date_df["close"]
                 single_date_df["high"] = single_date_df["close"]
                 single_date_df["low"] = single_date_df["close"]
                 single_date_df["volume"] = 0
-                df = df.append(single_date_df).sort_index()
+                # df = df.append(single_date_df).sort_index() # old pandas method
+                df = pd.concat([df,single_date_df]).sort_index()
             df = df.reindex(all_dates[valid_dates])
             zerovalues = {"volume": 0}
             df.fillna(zerovalues, inplace=True)
             df["close"].fillna(method="ffill", inplace=True)
             df["open interest"].fillna(method="ffill", inplace=True)
             df = df.fillna(
                 method="bfill", axis=1, limit=3
             )  # For some reason, inplace=True doesn't work here with Pandas 0.18
 
             if len(df.index) > 0:
                 start_date = df.index[0]
             else:
                 start_date = None
+
+
+            if notice_date  is not None:
+                if notice_date <= start_date: # Handle case when the backtest starts on a notice date - eg. start backtest 2000-01-03 with GC
+                    ac_date = start_date
+                else:
+                    # if last date of price date is beyond notice date, set auto close date to notice date - 2
+                    if df.index[-1] >= pd.Timestamp(notice_date, tz=None):
+                        if len(df.index) > 2:
+                            ac_date = df.index[
+                                df.index.searchsorted(pd.Timestamp(notice_date, tz=None)) - 2
+                            ]  # 2 days prior to FND
+                        else:
+                            ac_date = pd.Timestamp(notice_date, tz=None) - BDay(2)
+                    else:
+                        ac_date = pd.Timestamp(notice_date, tz=None) - BDay(2)
+                    if ac_date < start_date: # Handle situations where we might have gone prior to backtest
+                        ac_date = start_date
+            elif expiration_date is not None:
+                # ac_date = pd.Timestamp(expiration_date, tz="utc") # This method was used prior to 20200713
+                if df.index[-1] >= pd.Timestamp(expiration_date, tz=None): # Last value is on or after expiration date
+                    if len(df.index) > 2:
+                        ac_date = df.index[
+                            df.index.searchsorted(pd.Timestamp(expiration_date,tz=None)) - 2
+                        ]  # second last trading date, as determined by the data
+                    else:
+                        ac_date = pd.Timestamp(notice_date, tz=None) - BDay(2) # Corner case - perhaps we are ingesting around a boundary of expiration
+                else:
+                    ac_date = pd.Timestamp(expiration_date, tz=None) - BDay(2)
+
+
+
+
+            if ac_date is None: # Every futures contract needs an autoclose date of some sort
+                expiration_date = end_date + BDay(1) # Set a bogus date
+                ac_date = pd.Timestamp(expiration_date, tz=None) - BDay(2)
+
+            if notice_date is None:
+                notice_date = expiration_date + BDay(1)  # Put a notice date 1 day after expiration
+
             metadata.iloc[sid] = (
                 start_date,
                 end_date,
                 ac_date,
                 symbol,
                 root_symbol,
                 asset_name,
@@ -950,19 +1000,19 @@
     calendar_name="NYSE",
     symbol_list=None,
     watchlists=None,
     excluded_symbol_list=None,
 ):
     if not isinstance(start_session, pd.Timestamp):
         start_session = norgatedata.norgatehelper.decode_date(
-            start_session, datetimeformat="pandas-timestamp"
+            start_session, datetimeformat="pandas-timestamp", tz=None
         )
     if not isinstance(end_session, pd.Timestamp):
         end_session = norgatedata.norgatehelper.decode_date(
-            end_session, datetimeformat="pandas-timestamp"
+            end_session, datetimeformat="pandas-timestamp", tz=None
         )
     start_session, end_session = normalize_daily_start_end_session(
         calendar_name, start_session, end_session
     )
     register(
         bundlename,
         create_norgatedata_equities_bundle(
@@ -988,19 +1038,19 @@
     symbol_list=None,
     session_symbols=None,
     watchlists=None,
     excluded_symbol_list=None,
 ):
     if not isinstance(start_session, pd.Timestamp):
         start_session = norgatedata.norgatehelper.decode_date(
-            start_session, datetimeformat="pandas-timestamp"
+            start_session, datetimeformat="pandas-timestamp", tz=None
         )
     if not isinstance(end_session, pd.Timestamp):
         end_session = norgatedata.norgatehelper.decode_date(
-            end_session, datetimeformat="pandas-timestamp"
+            end_session, datetimeformat="pandas-timestamp", tz=None
         )
     start_session, end_session = normalize_daily_start_end_session(
         calendar_name, start_session, end_session
     )
     register(
         bundlename,
         create_norgatedata_futures_bundle(
@@ -1018,15 +1068,16 @@
     )
 
 
 def zipline_futures_root_symbols_dict():
     zipline_markets = {}
     session_symbols = norgatedata.futures_market_session_symbols()
     for session_symbol in session_symbols:
-        zipline_symbol = translate_futures_symbol(session_symbol)
+        #zipline_symbol = translate_futures_symbol(session_symbol)
+        zipline_symbol = session_symbol
         name = norgatedata.futures_market_session_name(session_symbol)
         if zipline_symbol in zipline_markets:
             logger.error(
                 "Zipline already has a session symbol of "
                 + zipline_symbol
                 + ":"
                 + zipline_markets[zipline_symbol]
```

## Comparing `zipline_norgatedata/README-Zipline130.md` & `zipline_norgatedata-2.4.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,136 @@
-![alt text](https://norgatedata.com/assets/images/norgate-data-logo-400x188.svg "Norgate Data") ![alt text](https://media.quantopian.com/logos/open_source/zipline-logo-03_.png "Zipline")
+Metadata-Version: 2.1
+Name: zipline-norgatedata
+Version: 2.4.0
+Summary: Zipline extension to provide bundles of data from Norgate Data into the Zipline algorithmic trading library for the Python programming language
+Home-page: https://norgatedata.com
+Author: NorgateData Pty Ltd
+Author-email: support@norgatedata.com
+License: EULA
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.TXT
+Requires-Dist: norgatedata
+Requires-Dist: logbook
 
-Integrates financial market data provided by [Norgate Data](https://norgatedata.com/) with [Zipline](https://zipline.io/), a Pythonic algorithmic trading library for backtesting.
+
+![alt text](https://norgatedata.com/assets/images/norgate-data-logo-400x188.svg "Norgate Data") ![alt text](https://norgatedata.com/assets/images/zipline-logo-03.png "Zipline")
+
+Integrates financial market data provided by [Norgate Data](https://norgatedata.com/) with [Zipline](https://zipline.ml4trading.io/), a Pythonic algorithmic trading library for backtesting.
 
 Key features of this extension
  * Simple bundle creation
  * Survivorship bias-free bundles
  * Incorporates time series data such as historical index membership and dividend yield into Zipline's Pipeline mechanism
  * No modifications to the Zipline code base (except to fix problems with installation and obsolete calls that crash Zipline)
 
-# Installation
+# Requirements
 
-```sh
-pip install zipline-norgatedata
-```
+* Zipline 2.4 and above (based upon the [Zipline Reloaded fork](https://zipline.ml4trading.io/) led by Stefan Jansen, which originates from the Quantopian-developed Zipline (which became become abandonware).  We recommend the latest release of Zipline Reloaded (currently v2.4) and associated packages (such as exchange-calendars) - there are too many quirks and workarounds for issues with older versions of Zipline to continue to maintain backwards compatibility.
+* Python 3.8+ (Python 3.10 recommended)
+* Microsoft Windows
+* An active [Norgate Data](https://norgatedata.com/) subscription
+* Norgate Data Updater software installed and running
+* Writable local user folder named .norgatedata (or defined in environment variable NORGATEDATA_ROOT) - defaults to C:\\Users\\Your username\\.norgatedata
+* Python packages: Pandas, Numpy, Logbook
+
+Note: The "Norgate Data Updater" application (NDU) is a Windows-only application. NDU must be running for this Python package to work.
 
-# Upgrades
+# How to install Zipline using Anaconda/Miniconda
+
+Most people have problems installing Zipline because they attempt to install it into their base environment.  The solution is simple:  Create a separate virtual environment that only has the necessary Python pacakges you require.  If you want to experiment then just create a new environment.
+
+Firstly, install either Anaconda (graphical environment) or Miniconda (cut-down command-line-based).  These instructions relate to Windows only.
+
+## How to install Zipline Reloaded and PyFolio, and Zipline-NorgateData
+
+Here's how we installed it here at Norgate:  
+Note:  We use Mamba instead of conda for the majority of the install, as it seems to be much quicker in resolving everything (ie seconds instead of minutes) and parallelizing the downlodas/install.
+
+Install the latest 64 bit [MiniConda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda Distribution](https://www.anaconda.com/distribution/).
+
+If you have ANY other running instances of Anaconda prompt/jupyter etc., *ensure sure they are all shut down.*
+
+
+Start an Anaconda (base) prompt, create an environment and install the appropriate versions of packages:
+
+````
+conda create -y -n zip310 python=3.10
+conda activate zip310
+conda install -y -c conda-forge mamba
+mamba install -y -c conda-forge -c zipline-reloaded pyfolio-reloaded
+mamba install -y -c conda-forge jupyter logbook
+pip install norgatedata zipline-norgatedata
+if not exist %HOMEPATH%\.zipline mkdir %HOMEPATH%\.zipline
+if not exist %HOMEPATH%\.zipline\extension.py copy /b NUL %HOMEPATH%\.zipline\extension.py
+````
+
+Note:  Mamba is used to install zipline-reloaded, because the Conda package manager becomes confused with so many dependencies required.  Mamba is also about 10 times quicker than Conda.
+
+## Upgrades of Zipline-NorgateData
 
 To receive upgrades/updates
 
 ```sh
 pip install zipline-norgatedata --upgrade
 ```
 
-# Requirements
+# Exchange Calendar Issues that require patching
 
-* Zipline 1.3.0
-* Python 3.5 only (this is a limitation of Zipline)
-* Microsoft Windows
-* An active [Norgate Data](https://norgatedata.com/) subscription
-* Norgate Data Updater software installed and running
-* Writable local user folder named .norgatedata (or defined in environment variable NORGATEDATA_ROOT) - defaults to C:\\Users\\Your username\\.norgatedata
-* Python packages: Pandas, Numpy, Logbook
+Norgate Data has developed the following patches.  Please make sure you implement all of them (most support messages we get are from people that have forgotten to patch all of the files).
+
+## Patch to add 17 Dec 2008 as holiday for CA Equities
+
+On this date, TSX had a major outage and was halted not long after the open, and never reopened.  In general, the financial industry has written off this day as a bust for the purposes of data analysis.
+
+
+Edit exchange_calendar_xtse.py
+Add the following at line 98:
+
+```
+# Significant failures where TSX was, for practical purposes, closed for the entire day
+TSXFailures = [pd.Timestamp("2008-12-17", tz=UTC),]
+```
+
+Edit exchange_calendar_nys.py
+change the following at line 164:
+
+```
+                September11ClosingsCanada
+
+```
+
+to:
+
+```
+                September11ClosingsCanada, TSXFailures
+
+```
 
-Note: The "Norgate Data Updater" application (NDU) is a Windows-only application. NDU must be running for this Python package to work.
 
-# Assumptions
+
+
+# Backtest Assumptions
 - Stocks are automatically set an auto_close_date of the last quoted date 
-- Futures are automatically set an auto_close_date to the earlier of following: Last trading date (for cash settled futures, and physically delivered futures that only allow delivery after the last trading date), or 1 trading day prior to first notice date for futures that have a first notice date prior to the last trading date.
+- Futures are automatically set an auto_close_date to the earlier of following: 2 days prior to last trading date (for cash settled futures, and physically delivered futures that only allow delivery after the last trading date), or 2 trading days prior to first notice date for futures that have a first notice date prior to the last trading date.
 
 # Bundle Creation 
 
 Navigate to your Zipline local settings folder.  This is typically located at **c:\\users\\<your username>\\.zipline**
 
-Add the following lines at the top of your Zipline local settings file - extension.py:
+Add the following lines at the top of your Zipline local settings file - extension.py (:
 **Note:  This is _NOT_ the extension.py file inside the Anaconda3\\envs\\<your environment>\\lib\\site-packages\\zipline**
 
 ```py
 from norgatedata import StockPriceAdjustmentType
 from zipline_norgatedata import (
     register_norgatedata_equities_bundle,
     register_norgatedata_futures_bundle )
@@ -56,42 +140,45 @@
 
 Here are some examples with varying parameters.  You should adapt these to your requirements.
 
 register_norgatedata_equities_bundle has the following default parameters:
     stock_price_adjustment_setting = StockPriceAdjustmentType.TOTALRETURN,
     end_session = 'now',
 	calendar_name = 'NYSE',
+    excluded_symbol_list = None,
 
 register_norgatedata_futures_bundle has the following default parameters:
     end_session = 'now',
-    calendar_name = 'us_futures'
+    calendar_name = 'us_futures',
+    excluded_symbol_list = None,
+
 
 ```py
 
 # EQUITIES BUNDLES
 
 # Single stock bundle - AAPL from 1990 though 2018
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-aapl',
-    symbol_list = ['AAPL'], 
+    symbol_list = ['AAPL','$SPXTR',], 
     start_session = '1990-01-01',
-    end_session = '2018-12-31'
+    end_session = '2020-12-01'
 )
 
 # FANG stocks (Facebook, Amazon, Netflix, Google) - 2012-05-18 until now
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-fang',
-    symbol_list = ['FB','AMZN','NFLX','GOOGL'], 
+    symbol_list = ['FB','AMZN','NFLX','GOOGL','$SPXTR',], 
     start_session = '2012-05-18',  # This is that FB first traded
 )
 
 # A small set of selected ETFs
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-selected-etfs',
-    symbol_list = ['SPY','GLD','USO'],
+    symbol_list = ['SPY','GLD','USO','$SPXTR',],
     start_session = '2006-04-10', # This is the USO first trading date
 )
 
 # S&P 500 Bundle for backtesting including all current & past constituents back to 1990
 # and the S&P 500 Total Return index (useful for benchmarking and/or index trend filtering)
 # (around 1800 securities)
 register_norgatedata_equities_bundle(
@@ -108,35 +195,41 @@
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-russell3000',
     watchlists = ['Russell 3000 Current & Past'],
     symbol_list = ['$RUATR'],
     start_session = '1990-01-01' ,
 )
 
+# And now a watchlist excluding a given list of symbols
+
+register_norgatedata_equities_bundle(
+    bundlename = 'norgatedata-russell3000-exfroth',
+    watchlists = ['Russell 3000 Current & Past'],
+    symbol_list = ['$RUATR'],
+    start_session = '1990-01-01' ,
+    excluded_symbol_list = ['TSLA','AMZN','FB','NFLX','GOOGL',]
+)
+
 # FUTURES BUNDLES
 
 # Example bundle for all of the individual contracts from three futures markets:
-# E-mini S&P 500, E-mini Nasdaq 100, E-mini Russell 2000
+# E-mini S&P 500, E-mini Nasdaq 100, E-mini Russell 2000,
+# with $SPXTR added for benchmark reference
 register_norgatedata_futures_bundle(
     bundlename = 'norgatedata-selected-index-futures',
     session_symbols = ['ES','NQ','RTY'],
+    symbol_list = ['$SPXTR'],
     start_session = '2000-01-01',
 )
 
-# Same as above, but also adds the S&P 500 Total Return index ($SPXTR) for reference
-register_norgatedata_futures_bundle(
-    bundlename = 'norgatedata-selected-index-futures-and-index',
-    session_symbols = ['ES','NQ','RTY'],
-    symbol_list = ['$SPXTR']
-    start_session = '2000-01-01',
-)
 
 # Bundle of futures used in Andreas Clenow's Trading Evolved book
 # (contains 6000+ individual futures contracts/deliveries)
 bundlename = 'norgatedata-tradingevolved-futures'
+symbol_list = ['$SPXTR',]
 session_symbols = [
 	'6A', # AUD
 	'6B', # GBP
 	'6C', # CAD
 	'6E', # EUR
 	'DX', # USDX
 	'6J', # JPY
@@ -174,25 +267,33 @@
 	'ZF', # 5-Year US T-Note
 	'ZT', # 2-Year US T-Note
 	'ZN', # 10-Year US T-Note
 	'ZB', # 30-Year US T-Bond        
 ]
 start_session = '2000-01-01',
 
-register_norgatedata_futures_bundle(bundlename,start_session,session_symbols = session_symbols )
-
+register_norgatedata_futures_bundle(bundlename,start_session,session_symbols = session_symbols, symbol_list = symbol_list )
 
 ```
 
 To ingest a bundle:
 
 ```sh
 zipline ingest -b <bundlename>
 ```
 
+# Benchmark against a symbol
+
+To benchmark against an index, you should use add set_benchmark within the intialize function.
+
+```py
+ def initialize(context):
+    set_benchmark(symbol('$SPXTR')) # Note: $SPXTR must be included in the bundle
+    # ...
+```
 
 # Pipelines - accessing timeseries data
 
 Timeseries data has been exposed into Zipline's Pipeline interface.   During a backtest, the Pipelines will be calculated against all securities in the bundle.
 
 The following Filter (i.e. boolean) pipelines are available:
  - [NorgateDataIndexConstituent](https://norgatedata.com/data-content-tables.php#ushics)
@@ -206,15 +307,15 @@
 
  To incorporate these into your trading model, you need to import the relevant packages/methods:
  
 ```py
 from zipline.pipeline import Pipeline
 from zipline_norgatedata.pipelines import (
     NorgateDataIndexConstituent, NorgateDataDividendYield )
-from zipline.api import order_target_percent
+from zipline.api import order_target_percent, set_benchmark
 ```
 
 It is recommended you put your pipeline construction in its own function:
 
  ```py
 def make_pipeline():
     indexconstituent = NorgateDataIndexConstituent('S&P 1500')
@@ -228,14 +329,15 @@
 
 Incorporate this into your trading system by attaching it to your initialize method.  Note, for better efficiency, use chunks=9999 or however many bars you are likely to need.  
 This will save unnecessary access to the Norgate Data database.
 
 ```py
 
  def initialize(context):
+    set_benchmark(symbol('$SPXTR')) # Note: $SPXTR must be included in the bundle
     attach_pipeline(make_pipeline(), 'norgatedata_pipeline', chunks=9999,eager=True)
     # ...
 ```
 
 Now you can access the contents of the pipeline in before_trading_start and/or handle_data by using Zipline's pipline_output method.  You can exit positions not already in the 
 
 ```py
@@ -254,27 +356,31 @@
     for asset in context.portfolio.positions:   
         if asset not in current_constituents:
             order_target_percent(asset,0.0)
 
     # ... your code here ...
 ```
 
+Note: Access to historical index constituents requires a Norgate Data Stocks subscription at the Platinum or Diamond level.
+
 # Worked example backtesting S&P 500 Constituents back to 1990
 
 This example comprises a backtest on the S&P 500, with a basic trend filter that is applied on the S&P 500 index ($SPX).  The total return version of the index is also ingested ($SPXTR) for comparison purposes.
 
+Note: This requires a Norgate Data US Stocks subscription at the Platinum or Diamond level.
+
 Create a bundle definition in extensions.py as follows:
 
 ```py
 from zipline_norgatedata import register_norgatedata_equities_bundle
 
 register_norgatedata_equities_bundle(
     bundlename = 'norgatedata-sp500-backtest',
-    symbol_list = ['$SPX','$SPXTR'],
-    watchlists = ['S&P 500 Current & Past'],
+    symbol_list = ['$SPX','$SPXTR',],
+    watchlists = ['S&P 500 Current & Past',],
     start_session = '1990-01-01',
 )
 ```
 
 Now, ingest that bundle into zipline:
 
 ```sh
@@ -296,14 +402,15 @@
     return Pipeline(
         columns={
              'NorgateDataIndexConstituent':indexconstituent,
         },
         screen = indexconstituent)
 
  def initialize(context):
+    set_benchmark(symbol('$SPXTR')) # Note: $SPXTR must be included in the bundle
     attach_pipeline(make_pipeline(), 'norgatedata_pipeline', chunks=9999,eager=True)
     # ... your code here ...
 
 def before_trading_start(context, data):
     context.pipeline_data = pipeline_output('norgatedata_pipeline')
     # ... your code here ...
 
@@ -328,15 +435,16 @@
 
 Create a bundle definition in extensions.py as follows:
 
 ```py
 from zipline_norgatedata import register_norgatedata_futures_bundle
 
 bundlename = 'norgatedata-es-futures'
-session_symbols = ['ES']
+session_symbols = ['ES',]
+symbol_list = ['$SPXTR',],
 start_session = '2000-01-01'
 register_norgatedata_futures_bundle(bundlename,start_session,session_symbols = session_symbols )
 
 ```
 
 Now, ingest that bundle into zipline:
 
@@ -344,19 +452,19 @@
 zipline ingest -b norgatedata-es-futures
 ```
 
 Inside your trading system file, you'd incorporate the following code snippets:
 
 ```py
  def initialize(context):
-
+    set_benchmark(symbol('$SPXTR')) # Note: $SPXTR must be included in the bundle
     # Obtain market(s)s directly from the bundle
     af =  context.asset_finder
     markets = set([]) # a set eliminates dupes
-    allcontracts = af.retrieve_futures_contracts(af.sids)
+    allcontracts = af.retrieve_futures_contracts(af.futures_sids)
     for contract in allcontracts:
         markets.add(allcontracts[contract].root_symbol)
            
     markets = list(markets)
     markets.sort()
   
     # Make a list of all continuations
@@ -411,330 +519,123 @@
 
 To obtain just the futures market sessions symbols, you can use the norgatedata package and adapt the following code:
 ```py
 import norgatedata
 for session_symbol in norgatedata.futures_market_session_symbols():
     print (session_symbol + " " + norgatedata.futures_market_session_name(session_symbol)) 
 ```
-# Zipline Futures root symbols
-
-To show the translated 2 character root symbols for each futures market session, and a description of each market you can run a tiny script (or adapt this):
-
-```py
-import zipline_norgatedata
-root_symbols_dict = zipline_norgatedata.zipline_futures_root_symbols_dict()
-print (root_symbols_dict)
-```
-
-# Zipline installation best practice
-
-- Zipline can be difficult to install if you do it in the wrong order.  Here's how we did it:
-
-  1.  Install the latest [Anaconda Distribution](https://www.anaconda.com/distribution/) 
-  2.  If using Conda v4.7 from an older Anaconda distribution, upgrade it to v4.8.  If installing Anaconda after July 2020 you can skip this.
-  3.  Start Ananconda and Create a fresh Python 3.5 environment (Click Environments, then click Create, give it a name such as zip35, select Python 3.5 and click Create)
-  4.  Run a terminal in the new environment, and use conda to install zipline 
-      ```
-      conda install zipline -c Quantopian
-      ```
-      and any other packages you want such as jupyter,  matplotlib etc.  
-      ```
-      conda install jupyter matplotlib
-      ```
-      Note, if you want Pyfolio (you probably will at some point), you should install this using Pip, as there is a very old version on Anaconda:
-      ```
-      pip install pyfolio
-      ```
-  5.  Install norgatedata and  zipline-norgatedata using pip 
-      ```
-      pip install norgatedata zipline-norgatedata
-      ```
-  6.  Upgrade logbook
-      The version of logbook (v0.12) installed as a dependency when you zipline has some incompatilities.  Upgrade it to a fresher (v0.15+) version.  You'll need to do this if you get an RLock error.
-      ```
-      pip install logbook --upgrade
-      ```
-  7.  Patch the zipline package (see ***Zipline 1.3.0 Benchmark Patch*** below) to resolve backtest failure) within your new environment
-  8.  Start a command prompt/terminal in your zipline environment you created, and simply run ```zipline bundles``` to ensure that it work (this also creates the .zipline folder too)
-  9.  If you are backtesting futures data and create your own continuous futures from within your backtesting, you'll need to patch Zipline.  (see ***Zipline 1.3.0 Patches to resolve KeyError on Continuous Futures backtesting***)
-  10.  If you want to backtest data prior to 1990 (Stocks) or 2000 (Futures) see ***Backtesting prior to in-built Zipline/trading-calendar limits***
-
 
 # Zipline Limitations/Quirks
 
-- Zipline 1.3.0 is only compatible with Python 3.5.  Hopefully they'll update it one day....
-- Zipline has not been not had an official release since v1.3.0 (July 2018).  For reasons unknown, even though many fixes and changes have been implemented to the source code, no release has been made.
-- Zipline is hard-coded to handle equities data from 1990 onwards only
-- Zipline is hard-coded handle futures data from 2000 onwards.
-- Zipline has unnecessarily complicated futures contracts by restricting symbols to 2 characters.  This is not a conventional followed by exchanges.  We hope they see the light and allow variable futures root symbol lengths (up to 5 characters).  In the meantime, you can get a list of futures market sessions covered and translated to their 2 character limit with: zipline_futures_root_symbols()
 - Zipline doesn't define all futures markets and doesn't provide any runtime extensibility in this area - you will need to add them to <your_environment>\lib\site-packages\zipline\finance\constants.py if they are not defined.  Be sure to backup this file as it will be overwritten any time you update zipline.
 - Zipline assumes that there are bars for every day of trading.  If a security doesn't trade for a given day (e.g. it was halted/suspended, or simply nobody wanted to trade it), it will be padded with the previous close repeated in the OHLC fields, with volume set to zero.  Consider how this might affect your trading calculations.  
 - Index volumes cannot be accurately ingested due to Zipline trying to convert large volumes to UINTs which are out-of-bounds for UINT32.  Index volumes will be divided by 1000.
-- Any stock whose adjusted volume exceeds the upper bound of UINT32 will be set to the maximum UINT32 value (4294967295).  This only occurs for stocks with a lot of splis and/or very large special dsitributions.
+- Any stock whose adjusted volume exceeds the upper bound of UINT32 will be set to the maximum UINT32 value (4294967295).  This only occurs for stocks with a lot of splits and/or very large special dsitributions.
 - Some stocks have adjusted volume values that fall below the boundaries used by winsorize_uint32 (e.g. volume of 8.225255e-05).  You'll see a warning when those stocks are ingested "UserWarning: Ignoring 12911 values because they are out of bounds for uint32".   These are  There's not much we can do here.  For now, just ignore those warnings.
-- Suprisingly, Zipline benchmarks do not work from securities ingested into your bundle.   Rather, the benchmark uses hardcoded logic that attempts to download the security SPY from an IEX API (which is now retired).  See the "Zipline 1.3.0 Benchmark patch" below to fix/bypass this issue.
-- Ingestion times could be improved significantly with multiprocessing (this requires Zipline enhancements)
-
-If you are brave you could try with the latest Zipline source code (make sure you install the release version first, to solve dependencies):
-```
-conda install -c quantopian/label/ci zipline
-```
-Note:  You'll need to re-ingest any previously ingested bundles, as the underlying database schema used in Zipline is different.
-
-
+- Ingestion times could be improved significantly with multiprocessing (this would require Zipline enhancements)
+- Zipline cannot handle negative prices (eg. Crude Oil in 2020) - any such prices will be set to zero.  Most systems would have rolled prior to this strange event anyway.
 
-# Zipline 1.3.0 Benchmark Patch to resolve backtest failure 
+# Testing on Australian ASX data
 
-Strangely, by default, Zipline attempts to obtain benchmark data for for the symbol SPY from IEX (even if you define another symbol as the benchmark).  The public IEX API was retired in June 2019 so this causes all backtests to fail.
-
-This will show this lovely error JSONDecodeError message similar to the following:
-```
-[2019-09-02 00:38:53.586933] INFO: Loader: Downloading benchmark data for 'SPY' from 1989-12-29 00:00:00+00:00 to 2019-08-30 00:00:00+00:00
-Traceback (most recent call last): 
-  File "C:\Users\pyuser\Anaconda3\envs\zip35\Scripts\zipline-script.py", line 11, in <module>
-    load_entry_point('zipline==1.3.0+383.g069e97b2', 'console_scripts', 'zipline')()
-  File "C:\Users\pyuser\Anaconda3\envs\zip35\lib\site-packages\click\core.py", line 722, in __call__
-    return self.main(*args, **kwargs)
-...
-  File "C:\Users\pyuser\Anaconda3\envs\zip35\lib\json\decoder.py", line 357, in raw_decode
-    raise JSONDecodeError("Expecting value", s, err.value) from None
-json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
-```
-
-A workaround is to simply return a benchmark that shows no return.  To do this you'll need to edit your Zipline libraries as follows:
-
-* Firstly, navigate to the exact path of your Python environment installation (from the error message above, the environment path is C:\Users\pyuser\Anaconda3\envs\zip35 )
-* Then navigate to Lib\site-packages\zipline\data  (i.e. full path for an environment named zip35 would be "C:\Users\\<your username>\Anaconda3\envs\zip35\Lib\site-packages\zipline\data")
-* Edit the file benchmarks.py and replace all of the contents with the following:
+By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.  For the ASX, the calendar name is XASX.    
 
+At the top of your algorithm:
 ```py
-import pandas as pd
 from trading_calendars import get_calendar
-
-# Modified to avoid downloading data from obsolete IEX interface
-def get_benchmark_returns(symbol):
-    cal = get_calendar('NYSE')
-    first_date = pd.Timestamp('1896-01-01', tz='utc')
-    last_date = pd.Timestamp.today(tz='utc')
-    dates = cal.sessions_in_range(first_date, last_date)
-    data = pd.DataFrame(0.0, index=dates, columns=['close'])
-    data = data['close']
-    return data.sort_index().iloc[1:]
-
 ```
 
-* Edit the file loader.py
-* search for the method ensure_benchmark_data, and comment out the following four lines as shown (around line 200):
-
-```py
-    #data = _load_cached_data(filename, first_date, last_date, now, 'benchmark',
-    #                         environ)
-    #if data is not None:
-    #    return data
-```
-
-Thanks to Andreas Clenow for this workaround, found here: https://github.com/quantopian/zipline/issues/2480
-
-# Zipline 1.3.0 Patch to resolve KeyError on Continuous Futures backtesting
-
-This bug shows as the following crypic error messgae:
-```
-KeyError: <class 'zipline.assets.continuous_futures.ContinuousFutures'>
-```
-
-Part 1:  Bug fix for DataPortal
-
-If you want to create continuous futures, you'll need to fix Zipline for a bug in the DataPortal code.  Effectively what has been left out of the Zipline source code is the ability to read futures data.  We could either fake our futures data to look like Equities data, or do this simple patch.
-
-You'll need to edit your Zipline package library as follows:
-
-* Firstly, navigate to the exact path of your Python environment installation (from the error message above, the environment path is C:\Users\pyuser\Anaconda3\envs\zip35 )
-* Then navigate to Lib\site-packages\zipline\utils  (i.e. full path for an environment named zip35 would be "C:\Users\<your username>\Anaconda3\envs\zip35\Lib\site-packages\zipline\utils")
-* Edit the file run_algo.py and find the following lines (around line 141):
-
-```py
-        data = DataPortal(
-            env.asset_finder,
-            trading_calendar=trading_calendar,
-            first_trading_day=first_trading_day,
-            equity_minute_reader=bundle_data.equity_minute_bar_reader,
-            equity_daily_reader=bundle_data.equity_daily_bar_reader,
-            adjustment_reader=bundle_data.adjustment_reader,
-```
-
-Add the following two lines to the end of this argument list:
-```py
-            future_minute_reader=bundle_data.equity_minute_bar_reader,
-            future_daily_reader=bundle_data.equity_daily_bar_reader,
-```
-
-The entire section of code should now read as follows:
-```py
-        data = DataPortal(
-            env.asset_finder,
-            trading_calendar=trading_calendar,
-            first_trading_day=first_trading_day,
-            equity_minute_reader=bundle_data.equity_minute_bar_reader,
-            equity_daily_reader=bundle_data.equity_daily_bar_reader,
-            adjustment_reader=bundle_data.adjustment_reader,
-            future_minute_reader=bundle_data.equity_minute_bar_reader,
-            future_daily_reader=bundle_data.equity_daily_bar_reader,
-            )
-```
-
-Part 2:  Workaround for markets without defined volatility
-
-By default, Zipline has defined constants for volatility that are used for slippage modelling.  If you attempt to test on a market that is not defined in the constants.py file, you will get a KeyError like this:
-
-This bug shows as the following crypic error messgae:
-```
-KeyError: 'KC'
-```
-
-This patch will give any market without an explicitly defined volatility a default volatility.
-
-* Edit finance/slippage.py
-* At around line 27, find the following:
-
-```py
-from zipline.finance.constants import ROOT_SYMBOL_TO_ETA
-```
-
-Change this to:
-
-```py
-from zipline.finance.constants import ROOT_SYMBOL_TO_ETA, DEFAULT_ETA
-```
-
-* At around line 510, within get_simulated_impact, find:
-
-```py
-        eta = self._eta[order.asset.root_symbol]
-```
-
-change this to:
-
-```py
-        try:
-            eta = self._eta[order.asset.root_symbol]
-        except:
-            eta = DEFAULT_ETA
-```
-
-# Jupyter reports no module named win32api
-
-Install/reinstall pywin32
-
-```
-conda install pywin32
-```
-
-
-# Backtesting prior to in-built Zipline/trading-calendar limits
-
-Zipline will only backtest according to the calendar within the trading_calendars package.  With some easy patches you can extend backtesting for US stocks from 1990 to 1970 and Futures from 2000 to 1970.
-
-1970 is the limit though.  It is not possible to extend prior to this  Most likely there's an underlying limitation to the Unix Epoch (1970-01-01 00:00:00).
-
-Firstly, we need extend internal benchmarking code to handle dates prior to 1980:
-* Navigate to the exact path of your Python environment installation (from the error message above, the environment path is C:\Users\pyuser\Anaconda3\envs\zip35 )
-* Then navigate to Lib\site-packages\zipline\data  (i.e. full path for an environment named zip35 would be "C:\Users\<your username>\Anaconda3\envs\zip35\Lib\site-packages\zipline\data")
-* Edit the file treasuries.py and find the following lines (around line 58):
-```py
-    return pd.Timestamp('1980', tz='UTC')
-```
-
-change this to:
-```py
-    return pd.Timestamp('1970', tz='UTC')
-```
-
-To extend backtestng prior to 1970 for US stocks:
-* Navigate to the exact path of your Python environment installation (from the error message above, the environment path is C:\Users\pyuser\Anaconda3\envs\zip35 )
-* Then navigate to Lib\site-packages\trading_calendars  (i.e. full path for an environnment named zip35 would be "C:\Users\<your username>\Anaconda3\envs\zip35\Lib\site-packages\trading_calendars")
-* Edit the file trading_calendar.py and find the following lines (around line 45):
-```py
-start_default = pd.Timestamp('1990-01-01', tz=UTC)
-```
-
-change this to:
-```py
-start_default = pd.Timestamp('1970-01-01', tz=UTC)
-```
-
-To extend backtestng prior to 2000 for futures:
-* Firstly, navigate to the exact path of your Python environment installation (from the error message above, the environment path is C:\Users\pyuser\Anaconda3\envs\zip35 )
-* Then navigate to Lib\site-packages\trading_calendars  (i.e. full path for an environment named zip35 would be "C:\Users\<your username>\Anaconda3\envs\zip35\Lib\site-packages\trading_calendars")
-* Edit the file us_futures_calendar.py and find the following lines (around line 49):
-```py
-                 start=Timestamp('2000-01-01', tz=UTC),
-```
+In the run_algorithm call, add a trading_calendar= line, for example:
 
-change this to:
 ```py
-                 start=Timestamp('1970-01-01', tz=UTC),
+results = run_algorithm(
+    start=start, end=end, 
+    initialize=initialize, analyze=analyze, 
+    handle_data=handle_data, 
+    capital_base=10000, 
+    trading_calendar=get_calendar('XASX'),
+    data_frequency = 'daily', 
+    bundle='norgatedata-spasx200',
+)
 ```
 
-Note:  This section is a work-in-progress.  There are additional trading holidays that need to be included.  Norgate Data will be submitting a pull request for such changes to the trading_calendar package.  In the meantime, if you want accurate holidays for NYSE (US Stocks), or ASX (Australian Stocks) contact Norgate data.  We'd be happy to email the trading calendar files.
-
-# Testing on ASX data
+# Testing on Canadian TSX data
 
-By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.
+By default, run_algorithm uses the 'NYSE' trading calendar.  To backtest other markets, you need to specify the calendar.  For the TSX, the calendar name is XTSE.  
 
 At the top of your algorithm:
 ```py
 from trading_calendars import get_calendar
 ```
 
 In the run_algorithm call, add a trading_calendar= line, for example:
 
 ```py
 results = run_algorithm(
     start=start, end=end, 
     initialize=initialize, analyze=analyze, 
     handle_data=handle_data, 
     capital_base=10000, 
-    trading_calendar=get_calendar('XASX'),
+    trading_calendar=get_calendar('XTSE'),
     data_frequency = 'daily', 
-    bundle='norgatedata-spasx200',
+    bundle='norgatedata-sptsx60',
 )
 ```
 
-ASX users will need an updated ASX trading calendar too.
-
-This can be upgraded by conda.
-
-```
-conda upgrade trading-calendars -c Quantopian
-```
+Be sure to implement the trading_calendars patch mentioned above too.
 
 # Books/publications that use Zipline, adapted for Norgate Data use
 
 We have adapted the Python code in the following books to use Norgate Data.  
+[Trading Evoled:  Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  
 
-* [Trading Evoled:  Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  Source code in Jupyter notebook format here: http://norgatedata.com/book-examples/trading-evolved/NorgateDataTradingEvolvedExamples.zip
+Source code compatible with Zipline (Reloaded) v2.4 in Jupyter notebook format, can be downloaded here:
+https://norgatedata.com/book-examples/trading-evolved/NorgateDataTradingEvolvedExamples.zipline240.zip
 
 If there are other book/publications that use Zipline and worth adding here, let us know.
 
 # FAQs
 
 ### During a backtest I receive an error ValueError: 'Time Period' is not in list.  How do I fix this?
 
-This can occur when the items in the bundle do not match the latest data in the Norgate Data database.  For stocks, if there are symbol changes within the database then the bundle will have the old symbol but the Norgate database will have the new symbol.    For Futures, there may have been additional futures contracts listed since your previous ingestion and the roll-over algorithm is trying to roll into them.  The solution is simple:  Ingest the bundle with the fresh data.
+This can occur when the items in the bundle do not match the latest data in the Norgate Data database.  For stocks, if there are symbol changes within the database then the bundle will have the old symbol but the Norgate database will have the new symbol.    For Futures, there may have been additional futures contracts listed since your previous ingestion and the roll-over algorithm is trying to roll into them.  
+
+The solution is simple:  Ingest the bundle with fresh data.
+
+# Change log
+
+Released versions and release dates can be seen here:
+https://pypi.org/project/zipline-norgatedata/#history
+
+The CHANGES.TXT within the package details the changes.
+
+# Installing older versions
+
+Older versions of Zipline-NorgateData can be installed easily using pip.  For example, to install v2.0.17.
+
+
+````
+pip install zipline-norgatedata==2.0.17
+````
+
+Note that prior versions may be only suited to older versions of Zipline.  However, due to the constantly evolving nature of Zipline, we can only really support the current version.
 
 # Support
 
 For support on Norgate Data or usage of the zipline-norgatedata extension:
 [Norgate Data support](https://norgatedata.com/contact.php)
 
 Please put separate issues in separate emails, as this ensures each issue is separately ticketed and tracked.
 
-For Zipline coding/usage issues, join the [Zipline Google Group](https://groups.google.com/forum/#!forum/zipline).  For bug reports on Zipline, report them on [Zipline Github](https://github.com/quantopian/zipline/issues)
+For bug reports on Zipline Reloaded, report them on Stefan Jansen's [Zipline Reloaded Github](https://github.com/stefan-jansen/zipline-reloaded/issues)
+
+There is also a Google Group, which isn't used much these days: [Zipline Google Group](https://groups.google.com/forum/#!forum/zipline).  
+
 
 # Thanks
 
 Thanks to:
 
-* [Andreas Clenow](https://www.followingthetrend.com) for his pioneering work in documenting Zipline bundles in his latest book [Trading Evolved: Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  We used many of the techniques described in the book to build our bundle code.
+* [Andreas Clenow](https://www.followingthetrend.com) for his pioneering work in documenting Zipline bundles in his latest book [Trading Evolved: Anyone can Build Killer Trading Strategies in Python](https://www.followingthetrend.com/trading-evolved/).  We used many of the techniques described in the book to build our bundle code.  There are many excellent examples of how to implement various trading systems including trend following, counter trend following, momentum, curve trading and combining multiple trading systems together.
 * Norgate Data alpha and beta testers.  Without your persistence we wouldn't have implemented half of the features.
-* The team at Quantopian for developing and open sourcing Zipline
+* The team that were formerly employed by Quantopian for developing and open sourcing Zipline
+* Continued development efforts on Zipline and associated packages since Quantopian ceased, by Stefan Jansen, Mehdi Bounouar, Allan Coppola and Shlomi Kushchi and many more.
```

## Comparing `zipline_norgatedata-2.3.4.dist-info/LICENSE.TXT` & `zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

