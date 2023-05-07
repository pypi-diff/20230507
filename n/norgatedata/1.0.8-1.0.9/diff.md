# Comparing `tmp/norgatedata-1.0.8-py3-none-any.whl.zip` & `tmp/norgatedata-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21134 bytes, number of entries: 10
+Zip file size: 21083 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 19-Jul-02 11:44 norgatedata/__init__.py
--rw-rw-rw-  2.0 fat    19373 b- defN 19-Sep-20 02:18 norgatedata/api.py
+-rw-rw-rw-  2.0 fat    19373 b- defN 19-Sep-20 02:23 norgatedata/api.py
 -rw-rw-rw-  2.0 fat    25857 b- defN 19-Jun-30 04:33 norgatedata/norgatedata.py
 -rw-rw-rw-  2.0 fat        3 b- defN 19-Jul-21 04:31 norgatedata/norgatedata_release_version.json
 -rw-rw-rw-  2.0 fat     9774 b- defN 19-Aug-29 14:41 norgatedata/norgatehelper.py
--rw-rw-rw-  2.0 fat    15759 b- defN 19-Sep-20 02:19 norgatedata-1.0.8.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    19424 b- defN 19-Sep-20 02:19 norgatedata-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 19-Sep-20 02:19 norgatedata-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 19-Sep-20 02:19 norgatedata-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      833 b- defN 19-Sep-20 02:19 norgatedata-1.0.8.dist-info/RECORD
-10 files, 91152 bytes uncompressed, 19708 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat    15759 b- defN 19-Sep-20 02:24 norgatedata-1.0.9.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    19532 b- defN 19-Sep-20 02:24 norgatedata-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 19-Sep-20 02:24 norgatedata-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 19-Sep-20 02:24 norgatedata-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      833 b- defN 19-Sep-20 02:24 norgatedata-1.0.9.dist-info/RECORD
+10 files, 91260 bytes uncompressed, 19657 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: norgatedata/norgatedata_release_version.json
 Comment: 
 
 Filename: norgatedata/norgatehelper.py
 Comment: 
 
-Filename: norgatedata-1.0.8.dist-info/LICENSE.TXT
+Filename: norgatedata-1.0.9.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: norgatedata-1.0.8.dist-info/METADATA
+Filename: norgatedata-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: norgatedata-1.0.8.dist-info/WHEEL
+Filename: norgatedata-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: norgatedata-1.0.8.dist-info/top_level.txt
+Filename: norgatedata-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: norgatedata-1.0.8.dist-info/RECORD
+Filename: norgatedata-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## norgatedata/api.py

```diff
@@ -1,11 +1,11 @@
 """This is the Norgate Data Python interface
 """
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 __author__ = 'NorgateData Pty Ltd'
 
 from .norgatehelper import *
 import csv
 from enum import Enum
 import logbook
```

## Comparing `norgatedata-1.0.8.dist-info/LICENSE.TXT` & `norgatedata-1.0.9.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

## Comparing `norgatedata-1.0.8.dist-info/METADATA` & `norgatedata-1.0.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norgatedata
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python interface to financial data provided by Norgate Data
 Home-page: https://norgatedata.com
 Author: NorgateData Pty Ltd
 Author-email: support@norgatedata.com
 License: EULA
 Platform: UNKNOWN
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -76,20 +76,20 @@
 ```
 
 Price & Volume adjustment allows you to adjust historical stock prices and volumes to account for the effect of capital events and dividends.
 ```py
 priceadjust = norgatedata.StockPriceAdjustmentType.NONE
 priceadjust = norgatedata.StockPriceAdjustmentType.CAPITAL
 priceadjust = norgatedata.StockPriceAdjustmentType.CAPITALSPECIAL
-priceadjust = norgatedata.StockPriceAdjustmentType.TOTALRETURN # default
+priceadjust = norgatedata.StockPriceAdjustmentType.TOTALRETURN # Default
 
 ```
 Date padding allows you to repeat the prior close on days where no price record would otherwise exist.
 ```py
-padding_setting = norgatedata.PaddingType.NONE   # Default, if not specified on timeseries calls
+padding_setting = norgatedata.PaddingType.NONE  # Default
 padding_setting = norgatedata.PaddingType.ALLMARKETDAYS
 padding_setting = norgatedata.PaddingType.ALLWEEKDAYS
 padding_setting = norgatedata.PaddingType.ALLCALENDARDAYS
 ```
 
 ### Examples
 ```py
@@ -100,160 +100,160 @@
 start_date = '1990-01-01'
 timeseriesformat = 'numpy-recarray'
 
 # Provides data on GOOG from 1990 until today in 
 # a NumPy recarray format, with explicitly set stock price 
 # adjustment and padding settings
 pricedata_recarray = norgatedata.price_timeseries(
-	symbol,
+    symbol,
     stock_price_adjustment_setting = priceadjust
     padding_setting = padding_setting,
     start_date = start_date,
     format=timeseriesformat)
 
 # Now in a Pandas-compatible format
 timeseriesformat = 'pandas-dataframe'
 pricedata_dataframe = norgatedata.price_timeseries(
-	symbol,
+    symbol,
     stock_price_adjustment_setting = priceadjust,
     padding_setting = padding_setting,
     start_date = start_date,
     format=timeseriesformat)
 
 # Now in a Numpy Ndarray
 timeseriesformat = 'numpy-ndarray'
 pricedata_ndarray = norgatedata.price_timeseries(
-	symbol,
+    symbol,
     stock_price_adjustment_setting = priceadjust,
     padding_setting = padding_setting,
     start_date = start_date,
     format=timeseriesformat)
 
 # Now limiting results to final 500 bars
 pricedata_dataframe = norgatedata.price_timeseries(
-	symbol,
-	stock_price_adjustment_setting = priceadjust,
-	padding_setting = padding_setting,
-	limit=500,
-	format=timeseriesformat)
+    symbol,
+    stock_price_adjustment_setting = priceadjust,
+    padding_setting = padding_setting,
+    limit=500,
+    format=timeseriesformat)
 
 # Now limiting results to a specific date range
 end_date='1999-12-31'
 pricedata_dataframe = norgatedata.price_timeseries(
-	symbol,
-	stock_price_adjustment_setting = priceadjust,
-	padding_setting = padding_setting,
-	start_date = start_date,
-	end_date = end_date,
-	format=timeseriesformat)
+    symbol,
+    stock_price_adjustment_setting = priceadjust,
+    padding_setting = padding_setting,
+    start_date = start_date,
+    end_date = end_date,
+    format=timeseriesformat)
 
 # Now using a numerical unchanging assetid instead of a symbol
 timeseriesformat = 'pandas-dataframe'
 assetid = 129769
 pricedata_dataframe = norgatedata.price_timeseries(
-	assetid,
-	limit=500,
+    assetid,
+    limit=500,
     format=timeseriesformat)
 
 ```
 
 ### Index Constituent
 
 To determine whether a stock was an index constituent on a particular date, you can use the index constituent timeseries function.  You can also pass in an existing
 NumPy ndarray or Pandas Dataframe and a new column will be added and returned
 
 ```py
 symbol = 'AAPL'
 indexname = 'S&P 500'  # Can also be an index symbol, such as $SPX, $RUI etc.
 
 idx = norgatedata.index_constituent_timeseries(
-	symbol,
+    symbol,
     indexname,
     format = "numpy-recarray")
 
 idx = norgatedata.index_constituent_timeseries(
-	symbol,
+    symbol,
     indexname,
     padding_setting = padding_setting,
     start_date = start_date,
     limit = -1,
     format = "numpy-ndarray")
 
 idx = norgatedata.index_constituent_timeseries(
-	symbol,
+    symbol,
     indexname,
     padding_setting = padding_setting,
     start_date = start_date,
     limit = -1,
     format = "pandas-dataframe")
 
 pricedata_recarray2 = norgatedata.index_constituent_timeseries(
-	symbol,
-	indexname,
-	padding_setting = padding_setting,
-	start_date = start_date,
-	limit = -1,
-	numpy_recarray = pricedata_recarray,
-	format = "numpy-recarray")
+    symbol,
+    indexname,
+    padding_setting = padding_setting,
+    start_date = start_date,
+    limit = -1,
+    numpy_recarray = pricedata_recarray,
+    format = "numpy-recarray")
 
 ```
 
 ### Major Exchange Listed
 
 ```py
 majexch = norgatedata.major_exchange_listed_timeseries(
-	symbol,
+    symbol,
     format = "numpy-recarray")
 ```
 
 Provides indication about US stocks on whether they are listed on a major exchange (e.g. NYSE, Nasdaq, NYSE American, NYSE Arca, Cboe BZX, IEX) (value = 1) or as an OTC/Pink Sheet stock (value = 0) for each trading date is available for all Equities and ETPs.
 
 Note:  Data is only available for this item from 2000 onwards.
 
 ### Capital Event
 
 ```py
 capevent = norgatedata.capital_event_timeseries(
-	symbol,
+    symbol,
     format = "numpy-recarray")
 ```
 
 This indicator will show when a capital event occurred. Effective on holding the security at the close on the day prior to the ex-date. Events include splits, reverse splits, bonus issues, stock dividends (dividends paid as stock) and complex reorganizations of capital (value = 1, otherwise if there is no event, value = 0)
 
 
 ### Dividend Yield
 
 ```py
 divyield = norgatedata.dividend_yield_timeseries(
-	symbol,
+    symbol,
     format = "numpy-recarray")
 ```
 
 This indicator provides a trailing 12 month sum of all split-adjusted ordinary dividends. It is calculated daily against the close price. New dividends are incorporated on the entitlement date (the trading day prior to the ex-dividend date) after which the trailing 12 month sum of dividends is recalculated. Special dividends, distributions and spin-offs are not included. The lookback period is adaptive to take into account slight variations in ex-dividend dates from year-to-year.
 
 ### Padding Status
 
 ```py
 paddingstatus = norgatedata.padding_status_timeseries(
-	symbol,
+    symbol,
     format = "numpy-recarray")
 ```
 
 This indicator will show when a price record has been padded in accordance with the Date Padding setting. If the Date Padding is set to "No padding" then this indicator will not return any values.
 
 
 ### Unadjusted Close
 
 This is not normally needed, as Unadjusted Close is provided in the price timeseries.  
 It is provided here to be used as a helper routine for other Python libraries such
 as zipline-norgatedata.
 
 ```py
 unadjclose = norgatedata.unadjusted_close_timeseries(
-	symbol,
+    symbol,
     format = "numpy-recarray")
 ```
 
 # Watchlists
 
 The symbols of a watchlist can be retrieved into a Python list using the watchlist_symbols function
 
@@ -425,48 +425,48 @@
 schemename = 'NorgateFuturesClassification'
 schemename = 'TRBC'
 schemename = 'GICS'
 classificationresulttype = 'ClassificationId'
 classificationresulttype = 'Name'
 classification = norgatedata.classification(
     symbol,
-	schemename,
-	classificationresulttype)
+    schemename,
+    classificationresulttype)
 ```
 
 Provides the classification for a given security.  
 
 ```py
 schemename = 'TRBC'
 schemename = 'GICS'
 classificationresulttype = 'ClassificationId'
 classificationresulttype = 'Name'
 level = 1
 level = 4
 classificationatlevel = norgatedata.classification(
     symbol,
-	schemename,
-	classificationresulttype,
-	level)
+    schemename,
+    classificationresulttype,
+    level)
 ```
 
 Provides the classification for a given security, at a given level of the classification scheme.
 
 
 ```py
 indexfamilycode = '$SPX'
 indexfamilycode = '$SP1500'
 level = 3
 indexreturntype = 'PR'
 indexreturntype = 'TR'
 indexsymbol = norgatedata.corresponding_industry_index(
     symbol,
-	indexfamilycode,
-	level,
-	indexreturntype)
+    indexfamilycode,
+    level,
+    indexreturntype)
 ```
 
 Provides the symbol of a corresponding index, at a given level of the classification scheme.
 
 
 # Other informational functions
 norgatedata.last_database_update_time
@@ -509,24 +509,24 @@
 # Obtain a Pandas dataframe for a given security from Norgate Data
 priceadjust = norgatedata.StockPriceAdjustmentType.TOTALRETURN 
 padding_setting = norgatedata.PaddingType.NONE   
 symbol = 'AAPL'
 start_date = '2010-01-01'
 timeseriesformat = 'pandas-dataframe'
 pricedata_dataframe = norgatedata.price_timeseries(
-	symbol,
-	stock_price_adjustment_setting = priceadjust,
-	padding_setting = padding_setting,
-	start_date = start_date,
-	format=timeseriesformat)
+    symbol,
+    stock_price_adjustment_setting = priceadjust,
+    padding_setting = padding_setting,
+    start_date = start_date,
+    format=timeseriesformat)
 
 # Rename columns to suit Backtrader
 pricedata_dataframe.rename(
-	columns={ 'Open':'open',  'High':'high', 'Low':'low', 'Close':'close', 'Volume':'volume', 'Open Interest':'open},
-	inplace=True)
+    columns={ 'Open':'open',  'High':'high', 'Low':'low', 'Close':'close', 'Volume':'volume', 'Open Interest':'open},
+    inplace=True)
 
 # Backtrader can convert this dataframe into its own internal format with:
 data = bt.feeds.PandasData(dataname=pricedata_dataframe)
 cerebro.adddata(data)  # Add the data feed
 # ... your code here ...
 
 ```
@@ -552,24 +552,24 @@
 # Obtain data from Norgate Data first, in Pandas dataframe format
 priceadjust = norgatedata.StockPriceAdjustmentType.TOTALRETURN 
 padding_setting = norgatedata.PaddingType.NONE   
 symbol = 'AAPL'
 start_date = '2010-01-01'
 timeseriesformat = 'pandas-dataframe'
 ohlc = norgatedata.price_timeseries(
-	symbol,
+    symbol,
     stock_price_adjustment_setting = priceadjust,
     padding_setting = padding_setting,
     start_date = start_date,
     format=timeseriesformat)
 
 # Change column names
 ohlc.rename(
-	columns={'Open':'O', 'High':'H', 'Low':'L', 'Close':'C', 'Volume':'V'},
-	inplace=True)
+    columns={'Open':'O', 'High':'H', 'Low':'L', 'Close':'C', 'Volume':'V'},
+    inplace=True)
 
 # pybacktest code:
 ms = ohlc.C.rolling(50).mean()
 ml = ohlc.L.rolling(100).mean()
 buy = cover = (ms > ml) & (ms.shift() < ml.shift())
 sell = short = (ms < ml) & (ms.shift() > ml.shift())
```

## Comparing `norgatedata-1.0.8.dist-info/RECORD` & `norgatedata-1.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 norgatedata/__init__.py,sha256=im_GUxTTQKblzjYKYxumPuXMJ_NXHuWy8QiNIQThl6g,20
-norgatedata/api.py,sha256=9UnU75w12J9vNA2Jf3CoAjq_0PloWS3sqoAnyPjEVOo,19373
+norgatedata/api.py,sha256=EzB-Wwmq9ynPbty0tQh8I96IwQgsxcbKO4h9bJyPaRU,19373
 norgatedata/norgatedata.py,sha256=QGIWhYJ-IhWvB9jImSIuioz44_Cew9O3ib51-8CnDC8,25857
 norgatedata/norgatedata_release_version.json,sha256=mAiebTb3jpdmyeo01ayzYR86ks2BxesQIJXZJP_H0Is,3
 norgatedata/norgatehelper.py,sha256=SmBK9sRgtNqSeqPC0vvZhuoFhCNxQuyPas8G0jZhpQA,9774
-norgatedata-1.0.8.dist-info/LICENSE.TXT,sha256=fa4yXMwYV7MXOzXHCt84ZmPvT00e5zDVtAWsfDHe7nc,15759
-norgatedata-1.0.8.dist-info/METADATA,sha256=gc8IYoVGeVC6ynlGa1jBG1KPnTVtq6AHsOeP0ZlH_ps,19424
-norgatedata-1.0.8.dist-info/WHEEL,sha256=QBOOAdG2icRHGBs2s94rfaUlHrdfNBp-TceubUYCwOE,97
-norgatedata-1.0.8.dist-info/top_level.txt,sha256=CTIJD8yTdbDcCpCxTirWRkQqyL6YjUEc-noofp3jpps,12
-norgatedata-1.0.8.dist-info/RECORD,,
+norgatedata-1.0.9.dist-info/LICENSE.TXT,sha256=fa4yXMwYV7MXOzXHCt84ZmPvT00e5zDVtAWsfDHe7nc,15759
+norgatedata-1.0.9.dist-info/METADATA,sha256=XFaLoHVSEl9dy6zGSy_6kTkDno29Vkf3MjK4OIMJ1rU,19532
+norgatedata-1.0.9.dist-info/WHEEL,sha256=QBOOAdG2icRHGBs2s94rfaUlHrdfNBp-TceubUYCwOE,97
+norgatedata-1.0.9.dist-info/top_level.txt,sha256=CTIJD8yTdbDcCpCxTirWRkQqyL6YjUEc-noofp3jpps,12
+norgatedata-1.0.9.dist-info/RECORD,,
```

