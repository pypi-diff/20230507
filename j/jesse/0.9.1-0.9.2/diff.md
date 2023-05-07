# Comparing `tmp/jesse-0.9.1.tar.gz` & `tmp/jesse-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jesse-0.9.1.tar", last modified: Wed Jul  8 09:02:31 2020, max compression
+gzip compressed data, was "dist/jesse-0.9.2.tar", last modified: Fri Jul 10 14:00:11 2020, max compression
```

## Comparing `jesse-0.9.1.tar` & `jesse-0.9.2.tar`

### file list

```diff
@@ -1,358 +1,358 @@
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:31.000000 jesse-0.9.1/
--rw-r--r--   0 sully      (501) staff       (20)     6544 2020-07-08 09:02:31.000000 jesse-0.9.1/PKG-INFO
--rw-r--r--   0 sully      (501) staff       (20)     5115 2020-05-27 13:40:25.000000 jesse-0.9.1/README.md
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/assets/
--rw-r--r--   0 sully      (501) staff       (20)   169463 2020-04-06 12:53:30.000000 jesse-0.9.1/assets/chart-example.png
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/
--rw-r--r--   0 sully      (501) staff       (20)    14305 2020-06-29 16:24:05.000000 jesse-0.9.1/jesse/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     3739 2020-06-16 14:01:35.000000 jesse-0.9.1/jesse/config.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/enums/
--rw-r--r--   0 sully      (501) staff       (20)     1251 2020-06-16 14:01:35.000000 jesse-0.9.1/jesse/enums/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/exceptions/
--rw-r--r--   0 sully      (501) staff       (20)      822 2020-06-19 14:02:06.000000 jesse-0.9.1/jesse/exceptions/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/exchanges/
--rw-r--r--   0 sully      (501) staff       (20)       37 2020-03-31 14:54:13.000000 jesse-0.9.1/jesse/exchanges/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)      670 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/exchanges/exchange.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/exchanges/sandbox/
--rw-r--r--   0 sully      (501) staff       (20)     2340 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/exchanges/sandbox/Sandbox.py
--rw-r--r--   0 sully      (501) staff       (20)       29 2020-04-07 06:41:01.000000 jesse-0.9.1/jesse/exchanges/sandbox/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/factories/
--rw-r--r--   0 sully      (501) staff       (20)      188 2020-04-07 06:41:01.000000 jesse-0.9.1/jesse/factories/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     2275 2020-03-03 14:38:38.000000 jesse-0.9.1/jesse/factories/candle_factory.py
--rw-r--r--   0 sully      (501) staff       (20)     1047 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/factories/order_factory.py
--rw-r--r--   0 sully      (501) staff       (20)    16348 2020-06-14 10:20:52.000000 jesse-0.9.1/jesse/helpers.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/indicators/
--rw-r--r--   0 sully      (501) staff       (20)     2922 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)      687 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/acosc.py
--rw-r--r--   0 sully      (501) staff       (20)      548 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/ad.py
--rw-r--r--   0 sully      (501) staff       (20)      741 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/adosc.py
--rw-r--r--   0 sully      (501) staff       (20)      620 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/adx.py
--rw-r--r--   0 sully      (501) staff       (20)      630 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/adxr.py
--rw-r--r--   0 sully      (501) staff       (20)     1528 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/alligator.py
--rw-r--r--   0 sully      (501) staff       (20)      628 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/ao.py
--rw-r--r--   0 sully      (501) staff       (20)      851 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/apo.py
--rw-r--r--   0 sully      (501) staff       (20)      647 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/aroon.py
--rw-r--r--   0 sully      (501) staff       (20)      602 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/aroonosc.py
--rw-r--r--   0 sully      (501) staff       (20)      604 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/atr.py
--rw-r--r--   0 sully      (501) staff       (20)      563 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/avgprice.py
--rw-r--r--   0 sully      (501) staff       (20)      577 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/beta.py
--rw-r--r--   0 sully      (501) staff       (20)     1243 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/bollinger_bands.py
--rw-r--r--   0 sully      (501) staff       (20)     1143 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/bollinger_bands_width.py
--rw-r--r--   0 sully      (501) staff       (20)      551 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/bop.py
--rw-r--r--   0 sully      (501) staff       (20)      609 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/cci.py
--rw-r--r--   0 sully      (501) staff       (20)      753 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/cmo.py
--rw-r--r--   0 sully      (501) staff       (20)      616 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/correl.py
--rw-r--r--   0 sully      (501) staff       (20)      651 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/cvi.py
--rw-r--r--   0 sully      (501) staff       (20)     1582 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/dec_osc.py
--rw-r--r--   0 sully      (501) staff       (20)     1083 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/decycler.py
--rw-r--r--   0 sully      (501) staff       (20)      704 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/dema.py
--rw-r--r--   0 sully      (501) staff       (20)      743 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/di.py
--rw-r--r--   0 sully      (501) staff       (20)      714 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/dm.py
--rw-r--r--   0 sully      (501) staff       (20)      798 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/donchian.py
--rw-r--r--   0 sully      (501) staff       (20)      792 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/dpo.py
--rw-r--r--   0 sully      (501) staff       (20)      551 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/dx.py
--rw-r--r--   0 sully      (501) staff       (20)      692 2020-06-04 14:25:51.000000 jesse-0.9.1/jesse/indicators/ema.py
--rw-r--r--   0 sully      (501) staff       (20)     1808 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/emd.py
--rw-r--r--   0 sully      (501) staff       (20)      625 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/emv.py
--rw-r--r--   0 sully      (501) staff       (20)     1078 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/fisher.py
--rw-r--r--   0 sully      (501) staff       (20)      788 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/fosc.py
--rw-r--r--   0 sully      (501) staff       (20)     2036 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/frama.py
--rw-r--r--   0 sully      (501) staff       (20)     1857 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/gatorosc.py
--rw-r--r--   0 sully      (501) staff       (20)     2031 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/gauss.py
--rw-r--r--   0 sully      (501) staff       (20)      779 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/hma.py
--rw-r--r--   0 sully      (501) staff       (20)      666 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/ht_dcperiod.py
--rw-r--r--   0 sully      (501) staff       (20)      663 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/ht_dcphase.py
--rw-r--r--   0 sully      (501) staff       (20)      787 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/ht_phasor.py
--rw-r--r--   0 sully      (501) staff       (20)      775 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/ht_sine.py
--rw-r--r--   0 sully      (501) staff       (20)      671 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/ht_trendline.py
--rw-r--r--   0 sully      (501) staff       (20)      665 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/ht_trendmode.py
--rw-r--r--   0 sully      (501) staff       (20)     1870 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/ichimoku_cloud.py
--rw-r--r--   0 sully      (501) staff       (20)     1375 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/itrend.py
--rw-r--r--   0 sully      (501) staff       (20)      702 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/kama.py
--rw-r--r--   0 sully      (501) staff       (20)     1153 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/keltner.py
--rw-r--r--   0 sully      (501) staff       (20)      838 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/kvo.py
--rw-r--r--   0 sully      (501) staff       (20)      703 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/linearreg.py
--rw-r--r--   0 sully      (501) staff       (20)      727 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/linearreg_angle.py
--rw-r--r--   0 sully      (501) staff       (20)      743 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/linearreg_intercept.py
--rw-r--r--   0 sully      (501) staff       (20)      727 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/linearreg_slope.py
--rw-r--r--   0 sully      (501) staff       (20)     1489 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/lrsi.py
--rw-r--r--   0 sully      (501) staff       (20)     1109 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/macd.py
--rw-r--r--   0 sully      (501) staff       (20)     1421 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/macdext.py
--rw-r--r--   0 sully      (501) staff       (20)      891 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/mama.py
--rw-r--r--   0 sully      (501) staff       (20)      649 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/marketfi.py
--rw-r--r--   0 sully      (501) staff       (20)      646 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/mass.py
--rw-r--r--   0 sully      (501) staff       (20)      532 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/medprice.py
--rw-r--r--   0 sully      (501) staff       (20)      617 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/mfi.py
--rw-r--r--   0 sully      (501) staff       (20)      762 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/midpoint.py
--rw-r--r--   0 sully      (501) staff       (20)      612 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/midprice.py
--rw-r--r--   0 sully      (501) staff       (20)     1644 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/minmax.py
--rw-r--r--   0 sully      (501) staff       (20)      735 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/mom.py
--rw-r--r--   0 sully      (501) staff       (20)      990 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/msw.py
--rw-r--r--   0 sully      (501) staff       (20)      618 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/natr.py
--rw-r--r--   0 sully      (501) staff       (20)      763 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/nvi.py
--rw-r--r--   0 sully      (501) staff       (20)      522 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/obv.py
--rw-r--r--   0 sully      (501) staff       (20)     9331 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/pattern_recognition.py
--rw-r--r--   0 sully      (501) staff       (20)     3264 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/pivot.py
--rw-r--r--   0 sully      (501) staff       (20)      852 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/ppo.py
--rw-r--r--   0 sully      (501) staff       (20)      763 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/pvi.py
--rw-r--r--   0 sully      (501) staff       (20)      638 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/qstick.py
--rw-r--r--   0 sully      (501) staff       (20)      769 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/roc.py
--rw-r--r--   0 sully      (501) staff       (20)      784 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/rocp.py
--rw-r--r--   0 sully      (501) staff       (20)      769 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/rocr.py
--rw-r--r--   0 sully      (501) staff       (20)      792 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/rocr100.py
--rw-r--r--   0 sully      (501) staff       (20)      685 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/rsi.py
--rw-r--r--   0 sully      (501) staff       (20)      622 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/sar.py
--rw-r--r--   0 sully      (501) staff       (20)     1433 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/sarext.py
--rw-r--r--   0 sully      (501) staff       (20)      687 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/sma.py
--rw-r--r--   0 sully      (501) staff       (20)     1032 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/smma.py
--rw-r--r--   0 sully      (501) staff       (20)     1345 2020-06-15 13:17:25.000000 jesse-0.9.1/jesse/indicators/srsi.py
--rw-r--r--   0 sully      (501) staff       (20)      750 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/stddev.py
--rw-r--r--   0 sully      (501) staff       (20)      920 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/stochastic.py
--rw-r--r--   0 sully      (501) staff       (20)      910 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/stochf.py
--rw-r--r--   0 sully      (501) staff       (20)     1429 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/supersmoother.py
--rw-r--r--   0 sully      (501) staff       (20)     3207 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/supertrend.py
--rw-r--r--   0 sully      (501) staff       (20)      768 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/t3.py
--rw-r--r--   0 sully      (501) staff       (20)      702 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/tema.py
--rw-r--r--   0 sully      (501) staff       (20)      539 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/trange.py
--rw-r--r--   0 sully      (501) staff       (20)      699 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/trima.py
--rw-r--r--   0 sully      (501) staff       (20)      720 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/trix.py
--rw-r--r--   0 sully      (501) staff       (20)      688 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/tsf.py
--rw-r--r--   0 sully      (501) staff       (20)      898 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/tsi.py
--rw-r--r--   0 sully      (501) staff       (20)      548 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/typprice.py
--rw-r--r--   0 sully      (501) staff       (20)      820 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/ultosc.py
--rw-r--r--   0 sully      (501) staff       (20)      797 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/var.py
--rw-r--r--   0 sully      (501) staff       (20)      972 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/vidya.py
--rw-r--r--   0 sully      (501) staff       (20)      721 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/vosc.py
--rw-r--r--   0 sully      (501) staff       (20)      838 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/vwma.py
--rw-r--r--   0 sully      (501) staff       (20)     1096 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/vwmacd.py
--rw-r--r--   0 sully      (501) staff       (20)      642 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/wad.py
--rw-r--r--   0 sully      (501) staff       (20)      555 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/wclprice.py
--rw-r--r--   0 sully      (501) staff       (20)      795 2020-06-03 12:43:28.000000 jesse-0.9.1/jesse/indicators/wilders.py
--rw-r--r--   0 sully      (501) staff       (20)      604 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/willr.py
--rw-r--r--   0 sully      (501) staff       (20)      691 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/wma.py
--rw-r--r--   0 sully      (501) staff       (20)      801 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/indicators/zlema.py
--rw-r--r--   0 sully      (501) staff       (20)      896 2020-06-04 07:25:44.000000 jesse-0.9.1/jesse/indicators/zscore.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/libs/
--rw-r--r--   0 sully      (501) staff       (20)       51 2020-03-18 09:56:14.000000 jesse-0.9.1/jesse/libs/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/libs/dynamic_numpy_array/
--rw-r--r--   0 sully      (501) staff       (20)     2817 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/libs/dynamic_numpy_array/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/models/
--rw-r--r--   0 sully      (501) staff       (20)      973 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Candle.py
--rw-r--r--   0 sully      (501) staff       (20)     4364 2020-06-27 16:22:39.000000 jesse-0.9.1/jesse/models/CompletedTrade.py
--rw-r--r--   0 sully      (501) staff       (20)     1504 2020-06-21 16:38:39.000000 jesse-0.9.1/jesse/models/Exchange.py
--rw-r--r--   0 sully      (501) staff       (20)     4626 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Order.py
--rw-r--r--   0 sully      (501) staff       (20)      764 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Orderbook.py
--rw-r--r--   0 sully      (501) staff       (20)     9320 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Position.py
--rw-r--r--   0 sully      (501) staff       (20)      293 2019-09-24 14:56:48.000000 jesse-0.9.1/jesse/models/Route.py
--rw-r--r--   0 sully      (501) staff       (20)     1035 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Ticker.py
--rw-r--r--   0 sully      (501) staff       (20)      907 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/Trade.py
--rw-r--r--   0 sully      (501) staff       (20)      317 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     3728 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/models/utils.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/
--rw-r--r--   0 sully      (501) staff       (20)        0 2020-03-31 14:27:02.000000 jesse-0.9.1/jesse/modes/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/backtest_mode/
--rw-r--r--   0 sully      (501) staff       (20)    12697 2020-06-29 16:24:05.000000 jesse-0.9.1/jesse/modes/backtest_mode/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/import_candles_mode/
--rw-r--r--   0 sully      (501) staff       (20)    12281 2020-06-16 14:03:08.000000 jesse-0.9.1/jesse/modes/import_candles_mode/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/
--rw-r--r--   0 sully      (501) staff       (20)      378 2020-06-16 14:01:35.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     2488 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/binance.py
--rw-r--r--   0 sully      (501) staff       (20)     2606 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/binance_futures.py
--rw-r--r--   0 sully      (501) staff       (20)     2365 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/bitfinex.py
--rw-r--r--   0 sully      (501) staff       (20)     2530 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/coinbase.py
--rw-r--r--   0 sully      (501) staff       (20)      487 2020-04-06 08:19:06.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/interface.py
--rw-r--r--   0 sully      (501) staff       (20)     2442 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/import_candles_mode/drivers/testnet_binance_futures.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/optimize_mode/
--rw-r--r--   0 sully      (501) staff       (20)    12786 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/optimize_mode/Genetics.py
--rw-r--r--   0 sully      (501) staff       (20)     8094 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/optimize_mode/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/modes/routes_mode/
--rw-r--r--   0 sully      (501) staff       (20)     1680 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/modes/routes_mode/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/research/
--rw-r--r--   0 sully      (501) staff       (20)     1057 2020-05-18 06:53:50.000000 jesse-0.9.1/jesse/research/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     2240 2020-01-24 09:21:45.000000 jesse-0.9.1/jesse/research/get_candles.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/routes/
--rw-r--r--   0 sully      (501) staff       (20)     1522 2020-06-14 10:21:04.000000 jesse-0.9.1/jesse/routes/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/
--rw-r--r--   0 sully      (501) staff       (20)        0 2020-01-05 20:22:17.000000 jesse-0.9.1/jesse/services/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     1470 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/api.py
--rw-r--r--   0 sully      (501) staff       (20)     6081 2020-06-14 10:28:25.000000 jesse-0.9.1/jesse/services/broker.py
--rw-r--r--   0 sully      (501) staff       (20)     2076 2020-04-20 11:58:09.000000 jesse-0.9.1/jesse/services/cache.py
--rw-r--r--   0 sully      (501) staff       (20)     4779 2020-03-05 10:34:43.000000 jesse-0.9.1/jesse/services/candle.py
--rw-r--r--   0 sully      (501) staff       (20)     3934 2020-06-29 16:32:38.000000 jesse-0.9.1/jesse/services/charts.py
--rw-r--r--   0 sully      (501) staff       (20)      678 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/db.py
--rw-r--r--   0 sully      (501) staff       (20)     1471 2020-06-29 16:30:14.000000 jesse-0.9.1/jesse/services/file.py
--rw-r--r--   0 sully      (501) staff       (20)     1074 2020-05-12 08:17:00.000000 jesse-0.9.1/jesse/services/logger.py
--rw-r--r--   0 sully      (501) staff       (20)      607 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/notifier.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/project_maker/
--rw-r--r--   0 sully      (501) staff       (20)     1024 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/project_maker/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/project_maker/project_template/
--rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:41:52.000000 jesse-0.9.1/jesse/services/project_maker/project_template/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     3022 2020-07-01 14:04:24.000000 jesse-0.9.1/jesse/services/project_maker/project_template/config.py
--rw-r--r--   0 sully      (501) staff       (20)      494 2020-06-19 15:25:26.000000 jesse-0.9.1/jesse/services/project_maker/project_template/routes.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/project_maker/project_template/storage/
--rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:43:03.000000 jesse-0.9.1/jesse/services/project_maker/project_template/storage/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/project_maker/project_template/strategies/
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/project_maker/project_template/strategies/ExampleStrategy/
--rw-r--r--   0 sully      (501) staff       (20)      321 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/project_maker/project_template/strategies/ExampleStrategy/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:42:57.000000 jesse-0.9.1/jesse/services/project_maker/project_template/strategies/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     9988 2020-06-09 09:02:25.000000 jesse-0.9.1/jesse/services/report.py
--rw-r--r--   0 sully      (501) staff       (20)     5605 2020-07-08 09:01:36.000000 jesse-0.9.1/jesse/services/required_candles.py
--rw-r--r--   0 sully      (501) staff       (20)      978 2020-06-19 16:37:42.000000 jesse-0.9.1/jesse/services/selectors.py
--rw-r--r--   0 sully      (501) staff       (20)     6798 2020-06-09 09:02:25.000000 jesse-0.9.1/jesse/services/statistics.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/strategy_maker/
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/services/strategy_maker/ExampleStrategy/
--rw-r--r--   0 sully      (501) staff       (20)      374 2020-06-25 13:49:43.000000 jesse-0.9.1/jesse/services/strategy_maker/ExampleStrategy/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)      882 2020-01-06 10:53:42.000000 jesse-0.9.1/jesse/services/strategy_maker/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)      817 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/services/table.py
--rwxr-xr-x   0 sully      (501) staff       (20)     1507 2020-06-29 16:30:41.000000 jesse-0.9.1/jesse/services/tradingview.py
--rw-r--r--   0 sully      (501) staff       (20)      265 2020-03-25 09:00:47.000000 jesse-0.9.1/jesse/services/validators.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/store/
--rw-r--r--   0 sully      (501) staff       (20)     3798 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/store/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)      232 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/store/state_app.py
--rw-r--r--   0 sully      (501) staff       (20)     9079 2020-06-28 08:04:56.000000 jesse-0.9.1/jesse/store/state_candles.py
--rw-r--r--   0 sully      (501) staff       (20)      207 2019-09-03 15:07:20.000000 jesse-0.9.1/jesse/store/state_completed_trades.py
--rw-r--r--   0 sully      (501) staff       (20)      414 2020-01-05 17:20:35.000000 jesse-0.9.1/jesse/store/state_exchanges.py
--rw-r--r--   0 sully      (501) staff       (20)       89 2019-12-15 15:25:59.000000 jesse-0.9.1/jesse/store/state_logs.py
--rw-r--r--   0 sully      (501) staff       (20)     4470 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/store/state_orderbook.py
--rw-r--r--   0 sully      (501) staff       (20)     1945 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/store/state_orders.py
--rw-r--r--   0 sully      (501) staff       (20)      563 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/store/state_positions.py
--rw-r--r--   0 sully      (501) staff       (20)     1489 2020-04-01 09:01:16.000000 jesse-0.9.1/jesse/store/state_tickers.py
--rw-r--r--   0 sully      (501) staff       (20)     2403 2020-04-01 09:01:16.000000 jesse-0.9.1/jesse/store/state_trades.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/
--rw-r--r--   0 sully      (501) staff       (20)    41145 2020-06-19 16:39:51.000000 jesse-0.9.1/jesse/strategies/Strategy.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test01/
--rw-r--r--   0 sully      (501) staff       (20)      522 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test01/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test02/
--rw-r--r--   0 sully      (501) staff       (20)      587 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test02/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test03/
--rw-r--r--   0 sully      (501) staff       (20)      652 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test03/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test04/
--rw-r--r--   0 sully      (501) staff       (20)     1443 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test04/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test05/
--rw-r--r--   0 sully      (501) staff       (20)      720 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test05/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test06/
--rw-r--r--   0 sully      (501) staff       (20)     1081 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test06/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test07/
--rw-r--r--   0 sully      (501) staff       (20)     1022 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test07/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test08/
--rw-r--r--   0 sully      (501) staff       (20)      965 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test08/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test09/
--rw-r--r--   0 sully      (501) staff       (20)      377 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test09/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test10/
--rw-r--r--   0 sully      (501) staff       (20)      549 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test10/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test11/
--rw-r--r--   0 sully      (501) staff       (20)      544 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test11/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test12/
--rw-r--r--   0 sully      (501) staff       (20)      675 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test12/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test13/
--rw-r--r--   0 sully      (501) staff       (20)      705 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test13/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test14/
--rw-r--r--   0 sully      (501) staff       (20)      701 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test14/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test15/
--rw-r--r--   0 sully      (501) staff       (20)      531 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test15/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test16/
--rw-r--r--   0 sully      (501) staff       (20)      681 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test16/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test17/
--rw-r--r--   0 sully      (501) staff       (20)      781 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test17/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test18/
--rw-r--r--   0 sully      (501) staff       (20)      606 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test18/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test19/
--rw-r--r--   0 sully      (501) staff       (20)      618 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test19/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test20/
--rw-r--r--   0 sully      (501) staff       (20)      531 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test20/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test21/
--rw-r--r--   0 sully      (501) staff       (20)      562 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test21/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test22/
--rw-r--r--   0 sully      (501) staff       (20)      398 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test22/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test23/
--rw-r--r--   0 sully      (501) staff       (20)      556 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test23/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test24/
--rw-r--r--   0 sully      (501) staff       (20)      396 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test24/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test25/
--rw-r--r--   0 sully      (501) staff       (20)      550 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test25/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test26/
--rw-r--r--   0 sully      (501) staff       (20)      393 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test26/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test27/
--rw-r--r--   0 sully      (501) staff       (20)      548 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test27/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test28/
--rw-r--r--   0 sully      (501) staff       (20)      458 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test28/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test29/
--rw-r--r--   0 sully      (501) staff       (20)     1250 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test29/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test30/
--rw-r--r--   0 sully      (501) staff       (20)      790 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test30/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test31/
--rw-r--r--   0 sully      (501) staff       (20)      584 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test31/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test32/
--rw-r--r--   0 sully      (501) staff       (20)      513 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test32/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test33/
--rw-r--r--   0 sully      (501) staff       (20)      439 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test33/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test34/
--rw-r--r--   0 sully      (501) staff       (20)      624 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test34/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test35/
--rw-r--r--   0 sully      (501) staff       (20)      727 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test35/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test36/
--rw-r--r--   0 sully      (501) staff       (20)      948 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test36/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test37/
--rw-r--r--   0 sully      (501) staff       (20)      927 2020-05-14 08:24:39.000000 jesse-0.9.1/jesse/strategies/Test37/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test38/
--rw-r--r--   0 sully      (501) staff       (20)      608 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test38/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test39/
--rw-r--r--   0 sully      (501) staff       (20)      607 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test39/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test40/
--rw-r--r--   0 sully      (501) staff       (20)      380 2020-04-16 07:03:33.000000 jesse-0.9.1/jesse/strategies/Test40/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test41/
--rw-r--r--   0 sully      (501) staff       (20)      705 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test41/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test42/
--rw-r--r--   0 sully      (501) staff       (20)      755 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test42/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test43/
--rw-r--r--   0 sully      (501) staff       (20)      686 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test43/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test44/
--rw-r--r--   0 sully      (501) staff       (20)      455 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test44/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test45/
--rw-r--r--   0 sully      (501) staff       (20)      586 2020-05-05 10:32:25.000000 jesse-0.9.1/jesse/strategies/Test45/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test46/
--rw-r--r--   0 sully      (501) staff       (20)      509 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/Test46/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test47/
--rw-r--r--   0 sully      (501) staff       (20)      654 2020-06-04 07:23:46.000000 jesse-0.9.1/jesse/strategies/Test47/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse/strategies/Test48/
--rw-r--r--   0 sully      (501) staff       (20)      505 2020-06-19 16:48:52.000000 jesse-0.9.1/jesse/strategies/Test48/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)       31 2020-06-02 13:45:57.000000 jesse-0.9.1/jesse/strategies/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)     5886 2020-06-25 13:50:51.000000 jesse-0.9.1/jesse/utils.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:30.000000 jesse-0.9.1/jesse.egg-info/
--rw-r--r--   0 sully      (501) staff       (20)     6544 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/PKG-INFO
--rw-r--r--   0 sully      (501) staff       (20)     8323 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/SOURCES.txt
--rw-r--r--   0 sully      (501) staff       (20)        1 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/dependency_links.txt
--rw-r--r--   0 sully      (501) staff       (20)       64 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/entry_points.txt
--rw-r--r--   0 sully      (501) staff       (20)      149 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/requires.txt
--rw-r--r--   0 sully      (501) staff       (20)       12 2020-07-08 09:02:29.000000 jesse-0.9.1/jesse.egg-info/top_level.txt
--rw-r--r--   0 sully      (501) staff       (20)       38 2020-07-08 09:02:31.000000 jesse-0.9.1/setup.cfg
--rw-r--r--   0 sully      (501) staff       (20)     1393 2020-07-08 09:01:43.000000 jesse-0.9.1/setup.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:31.000000 jesse-0.9.1/tests/
--rw-r--r--   0 sully      (501) staff       (20)        0 2019-10-08 17:11:56.000000 jesse-0.9.1/tests/__init__.py
-drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-08 09:02:31.000000 jesse-0.9.1/tests/data/
--rw-r--r--   0 sully      (501) staff       (20)       86 2019-10-08 16:59:09.000000 jesse-0.9.1/tests/data/__init__.py
--rw-r--r--   0 sully      (501) staff       (20)    96915 2019-07-05 07:23:38.000000 jesse-0.9.1/tests/data/test_candles_0.py
--rw-r--r--   0 sully      (501) staff       (20)     4007 2019-07-04 09:14:19.000000 jesse-0.9.1/tests/data/test_candles_1.py
--rw-r--r--   0 sully      (501) staff       (20)   397893 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/data/test_candles_indicators.py
--rw-r--r--   0 sully      (501) staff       (20)     4312 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_backtest.py
--rw-r--r--   0 sully      (501) staff       (20)    11538 2020-06-14 10:29:43.000000 jesse-0.9.1/tests/test_broker.py
--rw-r--r--   0 sully      (501) staff       (20)     4352 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_candle_service.py
--rw-r--r--   0 sully      (501) staff       (20)     3086 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_conflicting_orders.py
--rw-r--r--   0 sully      (501) staff       (20)     1071 2020-06-19 14:11:38.000000 jesse-0.9.1/tests/test_exchange.py
--rw-r--r--   0 sully      (501) staff       (20)    10547 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_helpers.py
--rw-r--r--   0 sully      (501) staff       (20)     2676 2020-03-18 16:10:57.000000 jesse-0.9.1/tests/test_import_candles.py
--rw-r--r--   0 sully      (501) staff       (20)    36841 2020-06-04 07:25:44.000000 jesse-0.9.1/tests/test_indicators.py
--rw-r--r--   0 sully      (501) staff       (20)     7110 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_metrics.py
--rw-r--r--   0 sully      (501) staff       (20)     1042 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_order.py
--rw-r--r--   0 sully      (501) staff       (20)    30016 2020-06-19 16:47:59.000000 jesse-0.9.1/tests/test_parent_strategy.py
--rw-r--r--   0 sully      (501) staff       (20)     5781 2020-02-27 16:19:06.000000 jesse-0.9.1/tests/test_position.py
--rw-r--r--   0 sully      (501) staff       (20)     1255 2020-01-18 18:21:36.000000 jesse-0.9.1/tests/test_router.py
--rw-r--r--   0 sully      (501) staff       (20)     4656 2020-06-28 08:05:07.000000 jesse-0.9.1/tests/test_state_candle.py
--rw-r--r--   0 sully      (501) staff       (20)      616 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_state_exchanges.py
--rw-r--r--   0 sully      (501) staff       (20)     1082 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_state_logs.py
--rw-r--r--   0 sully      (501) staff       (20)    11074 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_state_orderbook.py
--rw-r--r--   0 sully      (501) staff       (20)     2130 2020-06-02 13:45:57.000000 jesse-0.9.1/tests/test_state_orders.py
--rw-r--r--   0 sully      (501) staff       (20)     1888 2020-02-06 09:25:52.000000 jesse-0.9.1/tests/test_state_ticker.py
--rw-r--r--   0 sully      (501) staff       (20)     2960 2020-01-18 18:21:36.000000 jesse-0.9.1/tests/test_state_trades.py
--rw-r--r--   0 sully      (501) staff       (20)     4219 2020-06-25 13:50:51.000000 jesse-0.9.1/tests/test_strategy_utils.py
--rw-r--r--   0 sully      (501) staff       (20)     3875 2020-02-27 16:38:41.000000 jesse-0.9.1/tests/test_trade.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/
+-rw-r--r--   0 sully      (501) staff       (20)     6544 2020-07-10 14:00:11.000000 jesse-0.9.2/PKG-INFO
+-rw-r--r--   0 sully      (501) staff       (20)     5115 2020-05-27 13:40:25.000000 jesse-0.9.2/README.md
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/assets/
+-rw-r--r--   0 sully      (501) staff       (20)   169463 2020-04-06 12:53:30.000000 jesse-0.9.2/assets/chart-example.png
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/
+-rw-r--r--   0 sully      (501) staff       (20)    14305 2020-06-29 16:24:05.000000 jesse-0.9.2/jesse/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     3739 2020-06-16 14:01:35.000000 jesse-0.9.2/jesse/config.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/enums/
+-rw-r--r--   0 sully      (501) staff       (20)     1251 2020-06-16 14:01:35.000000 jesse-0.9.2/jesse/enums/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/exceptions/
+-rw-r--r--   0 sully      (501) staff       (20)      822 2020-06-19 14:02:06.000000 jesse-0.9.2/jesse/exceptions/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/exchanges/
+-rw-r--r--   0 sully      (501) staff       (20)       37 2020-03-31 14:54:13.000000 jesse-0.9.2/jesse/exchanges/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)      670 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/exchanges/exchange.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/exchanges/sandbox/
+-rw-r--r--   0 sully      (501) staff       (20)     2340 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/exchanges/sandbox/Sandbox.py
+-rw-r--r--   0 sully      (501) staff       (20)       29 2020-04-07 06:41:01.000000 jesse-0.9.2/jesse/exchanges/sandbox/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse/factories/
+-rw-r--r--   0 sully      (501) staff       (20)      188 2020-04-07 06:41:01.000000 jesse-0.9.2/jesse/factories/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     2275 2020-03-03 14:38:38.000000 jesse-0.9.2/jesse/factories/candle_factory.py
+-rw-r--r--   0 sully      (501) staff       (20)     1047 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/factories/order_factory.py
+-rw-r--r--   0 sully      (501) staff       (20)    16348 2020-06-14 10:20:52.000000 jesse-0.9.2/jesse/helpers.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/indicators/
+-rw-r--r--   0 sully      (501) staff       (20)     2922 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)      687 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/acosc.py
+-rw-r--r--   0 sully      (501) staff       (20)      548 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/ad.py
+-rw-r--r--   0 sully      (501) staff       (20)      741 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/adosc.py
+-rw-r--r--   0 sully      (501) staff       (20)      620 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/adx.py
+-rw-r--r--   0 sully      (501) staff       (20)      630 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/adxr.py
+-rw-r--r--   0 sully      (501) staff       (20)     1528 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/alligator.py
+-rw-r--r--   0 sully      (501) staff       (20)      628 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/ao.py
+-rw-r--r--   0 sully      (501) staff       (20)      851 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/apo.py
+-rw-r--r--   0 sully      (501) staff       (20)      647 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/aroon.py
+-rw-r--r--   0 sully      (501) staff       (20)      602 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/aroonosc.py
+-rw-r--r--   0 sully      (501) staff       (20)      604 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/atr.py
+-rw-r--r--   0 sully      (501) staff       (20)      563 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/avgprice.py
+-rw-r--r--   0 sully      (501) staff       (20)      577 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/beta.py
+-rw-r--r--   0 sully      (501) staff       (20)     1243 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/bollinger_bands.py
+-rw-r--r--   0 sully      (501) staff       (20)     1143 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/bollinger_bands_width.py
+-rw-r--r--   0 sully      (501) staff       (20)      551 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/bop.py
+-rw-r--r--   0 sully      (501) staff       (20)      609 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/cci.py
+-rw-r--r--   0 sully      (501) staff       (20)      753 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/cmo.py
+-rw-r--r--   0 sully      (501) staff       (20)      616 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/correl.py
+-rw-r--r--   0 sully      (501) staff       (20)      651 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/cvi.py
+-rw-r--r--   0 sully      (501) staff       (20)     1582 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/dec_osc.py
+-rw-r--r--   0 sully      (501) staff       (20)     1083 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/decycler.py
+-rw-r--r--   0 sully      (501) staff       (20)      704 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/dema.py
+-rw-r--r--   0 sully      (501) staff       (20)      743 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/di.py
+-rw-r--r--   0 sully      (501) staff       (20)      714 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/dm.py
+-rw-r--r--   0 sully      (501) staff       (20)      798 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/donchian.py
+-rw-r--r--   0 sully      (501) staff       (20)      792 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/dpo.py
+-rw-r--r--   0 sully      (501) staff       (20)      551 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/dx.py
+-rw-r--r--   0 sully      (501) staff       (20)      692 2020-06-04 14:25:51.000000 jesse-0.9.2/jesse/indicators/ema.py
+-rw-r--r--   0 sully      (501) staff       (20)     1808 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/emd.py
+-rw-r--r--   0 sully      (501) staff       (20)      625 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/emv.py
+-rw-r--r--   0 sully      (501) staff       (20)     1078 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/fisher.py
+-rw-r--r--   0 sully      (501) staff       (20)      788 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/fosc.py
+-rw-r--r--   0 sully      (501) staff       (20)     2036 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/frama.py
+-rw-r--r--   0 sully      (501) staff       (20)     1857 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/gatorosc.py
+-rw-r--r--   0 sully      (501) staff       (20)     2031 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/gauss.py
+-rw-r--r--   0 sully      (501) staff       (20)      779 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/hma.py
+-rw-r--r--   0 sully      (501) staff       (20)      666 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/ht_dcperiod.py
+-rw-r--r--   0 sully      (501) staff       (20)      663 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/ht_dcphase.py
+-rw-r--r--   0 sully      (501) staff       (20)      787 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/ht_phasor.py
+-rw-r--r--   0 sully      (501) staff       (20)      775 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/ht_sine.py
+-rw-r--r--   0 sully      (501) staff       (20)      671 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/ht_trendline.py
+-rw-r--r--   0 sully      (501) staff       (20)      665 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/ht_trendmode.py
+-rw-r--r--   0 sully      (501) staff       (20)     1870 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/ichimoku_cloud.py
+-rw-r--r--   0 sully      (501) staff       (20)     1375 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/itrend.py
+-rw-r--r--   0 sully      (501) staff       (20)      702 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/kama.py
+-rw-r--r--   0 sully      (501) staff       (20)     1153 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/keltner.py
+-rw-r--r--   0 sully      (501) staff       (20)      838 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/kvo.py
+-rw-r--r--   0 sully      (501) staff       (20)      703 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/linearreg.py
+-rw-r--r--   0 sully      (501) staff       (20)      727 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/linearreg_angle.py
+-rw-r--r--   0 sully      (501) staff       (20)      743 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/linearreg_intercept.py
+-rw-r--r--   0 sully      (501) staff       (20)      727 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/linearreg_slope.py
+-rw-r--r--   0 sully      (501) staff       (20)     1489 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/lrsi.py
+-rw-r--r--   0 sully      (501) staff       (20)     1109 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/macd.py
+-rw-r--r--   0 sully      (501) staff       (20)     1421 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/macdext.py
+-rw-r--r--   0 sully      (501) staff       (20)      891 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/mama.py
+-rw-r--r--   0 sully      (501) staff       (20)      649 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/marketfi.py
+-rw-r--r--   0 sully      (501) staff       (20)      646 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/mass.py
+-rw-r--r--   0 sully      (501) staff       (20)      532 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/medprice.py
+-rw-r--r--   0 sully      (501) staff       (20)      617 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/mfi.py
+-rw-r--r--   0 sully      (501) staff       (20)      762 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/midpoint.py
+-rw-r--r--   0 sully      (501) staff       (20)      612 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/midprice.py
+-rw-r--r--   0 sully      (501) staff       (20)     1644 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/minmax.py
+-rw-r--r--   0 sully      (501) staff       (20)      735 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/mom.py
+-rw-r--r--   0 sully      (501) staff       (20)      990 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/msw.py
+-rw-r--r--   0 sully      (501) staff       (20)      618 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/natr.py
+-rw-r--r--   0 sully      (501) staff       (20)      763 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/nvi.py
+-rw-r--r--   0 sully      (501) staff       (20)      522 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/obv.py
+-rw-r--r--   0 sully      (501) staff       (20)     9331 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/pattern_recognition.py
+-rw-r--r--   0 sully      (501) staff       (20)     3264 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/pivot.py
+-rw-r--r--   0 sully      (501) staff       (20)      852 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/ppo.py
+-rw-r--r--   0 sully      (501) staff       (20)      763 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/pvi.py
+-rw-r--r--   0 sully      (501) staff       (20)      638 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/qstick.py
+-rw-r--r--   0 sully      (501) staff       (20)      769 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/roc.py
+-rw-r--r--   0 sully      (501) staff       (20)      784 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/rocp.py
+-rw-r--r--   0 sully      (501) staff       (20)      769 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/rocr.py
+-rw-r--r--   0 sully      (501) staff       (20)      792 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/rocr100.py
+-rw-r--r--   0 sully      (501) staff       (20)      685 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/rsi.py
+-rw-r--r--   0 sully      (501) staff       (20)      622 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/sar.py
+-rw-r--r--   0 sully      (501) staff       (20)     1433 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/sarext.py
+-rw-r--r--   0 sully      (501) staff       (20)      687 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/sma.py
+-rw-r--r--   0 sully      (501) staff       (20)     1032 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/smma.py
+-rw-r--r--   0 sully      (501) staff       (20)     1345 2020-06-15 13:17:25.000000 jesse-0.9.2/jesse/indicators/srsi.py
+-rw-r--r--   0 sully      (501) staff       (20)      750 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/stddev.py
+-rw-r--r--   0 sully      (501) staff       (20)      920 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/stochastic.py
+-rw-r--r--   0 sully      (501) staff       (20)      910 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/stochf.py
+-rw-r--r--   0 sully      (501) staff       (20)     1429 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/supersmoother.py
+-rw-r--r--   0 sully      (501) staff       (20)     3207 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/supertrend.py
+-rw-r--r--   0 sully      (501) staff       (20)      768 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/t3.py
+-rw-r--r--   0 sully      (501) staff       (20)      702 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/tema.py
+-rw-r--r--   0 sully      (501) staff       (20)      539 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/trange.py
+-rw-r--r--   0 sully      (501) staff       (20)      699 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/trima.py
+-rw-r--r--   0 sully      (501) staff       (20)      720 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/trix.py
+-rw-r--r--   0 sully      (501) staff       (20)      688 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/tsf.py
+-rw-r--r--   0 sully      (501) staff       (20)      898 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/tsi.py
+-rw-r--r--   0 sully      (501) staff       (20)      548 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/typprice.py
+-rw-r--r--   0 sully      (501) staff       (20)      820 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/ultosc.py
+-rw-r--r--   0 sully      (501) staff       (20)      797 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/var.py
+-rw-r--r--   0 sully      (501) staff       (20)      972 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/vidya.py
+-rw-r--r--   0 sully      (501) staff       (20)      721 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/vosc.py
+-rw-r--r--   0 sully      (501) staff       (20)      838 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/vwma.py
+-rw-r--r--   0 sully      (501) staff       (20)     1096 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/vwmacd.py
+-rw-r--r--   0 sully      (501) staff       (20)      642 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/wad.py
+-rw-r--r--   0 sully      (501) staff       (20)      555 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/wclprice.py
+-rw-r--r--   0 sully      (501) staff       (20)      795 2020-06-03 12:43:28.000000 jesse-0.9.2/jesse/indicators/wilders.py
+-rw-r--r--   0 sully      (501) staff       (20)      604 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/willr.py
+-rw-r--r--   0 sully      (501) staff       (20)      691 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/wma.py
+-rw-r--r--   0 sully      (501) staff       (20)      801 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/indicators/zlema.py
+-rw-r--r--   0 sully      (501) staff       (20)      896 2020-06-04 07:25:44.000000 jesse-0.9.2/jesse/indicators/zscore.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/libs/
+-rw-r--r--   0 sully      (501) staff       (20)       51 2020-03-18 09:56:14.000000 jesse-0.9.2/jesse/libs/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/libs/dynamic_numpy_array/
+-rw-r--r--   0 sully      (501) staff       (20)     2817 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/libs/dynamic_numpy_array/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/models/
+-rw-r--r--   0 sully      (501) staff       (20)      973 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Candle.py
+-rw-r--r--   0 sully      (501) staff       (20)     4364 2020-06-27 16:22:39.000000 jesse-0.9.2/jesse/models/CompletedTrade.py
+-rw-r--r--   0 sully      (501) staff       (20)     1504 2020-06-21 16:38:39.000000 jesse-0.9.2/jesse/models/Exchange.py
+-rw-r--r--   0 sully      (501) staff       (20)     4626 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Order.py
+-rw-r--r--   0 sully      (501) staff       (20)      764 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Orderbook.py
+-rw-r--r--   0 sully      (501) staff       (20)     9320 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Position.py
+-rw-r--r--   0 sully      (501) staff       (20)      293 2019-09-24 14:56:48.000000 jesse-0.9.2/jesse/models/Route.py
+-rw-r--r--   0 sully      (501) staff       (20)     1035 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Ticker.py
+-rw-r--r--   0 sully      (501) staff       (20)      907 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/Trade.py
+-rw-r--r--   0 sully      (501) staff       (20)      317 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     3728 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/models/utils.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/
+-rw-r--r--   0 sully      (501) staff       (20)        0 2020-03-31 14:27:02.000000 jesse-0.9.2/jesse/modes/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/backtest_mode/
+-rw-r--r--   0 sully      (501) staff       (20)    12697 2020-06-29 16:24:05.000000 jesse-0.9.2/jesse/modes/backtest_mode/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/import_candles_mode/
+-rw-r--r--   0 sully      (501) staff       (20)    12281 2020-06-16 14:03:08.000000 jesse-0.9.2/jesse/modes/import_candles_mode/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/
+-rw-r--r--   0 sully      (501) staff       (20)      378 2020-06-16 14:01:35.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     2488 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/binance.py
+-rw-r--r--   0 sully      (501) staff       (20)     2606 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/binance_futures.py
+-rw-r--r--   0 sully      (501) staff       (20)     2365 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/bitfinex.py
+-rw-r--r--   0 sully      (501) staff       (20)     2530 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/coinbase.py
+-rw-r--r--   0 sully      (501) staff       (20)      487 2020-04-06 08:19:06.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/interface.py
+-rw-r--r--   0 sully      (501) staff       (20)     2442 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/import_candles_mode/drivers/testnet_binance_futures.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/optimize_mode/
+-rw-r--r--   0 sully      (501) staff       (20)    12786 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/optimize_mode/Genetics.py
+-rw-r--r--   0 sully      (501) staff       (20)     8094 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/optimize_mode/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/modes/routes_mode/
+-rw-r--r--   0 sully      (501) staff       (20)     1680 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/modes/routes_mode/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/research/
+-rw-r--r--   0 sully      (501) staff       (20)     1057 2020-05-18 06:53:50.000000 jesse-0.9.2/jesse/research/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     2240 2020-01-24 09:21:45.000000 jesse-0.9.2/jesse/research/get_candles.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/routes/
+-rw-r--r--   0 sully      (501) staff       (20)     1522 2020-06-14 10:21:04.000000 jesse-0.9.2/jesse/routes/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/
+-rw-r--r--   0 sully      (501) staff       (20)        0 2020-01-05 20:22:17.000000 jesse-0.9.2/jesse/services/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     1470 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/api.py
+-rw-r--r--   0 sully      (501) staff       (20)     6081 2020-06-14 10:28:25.000000 jesse-0.9.2/jesse/services/broker.py
+-rw-r--r--   0 sully      (501) staff       (20)     2076 2020-04-20 11:58:09.000000 jesse-0.9.2/jesse/services/cache.py
+-rw-r--r--   0 sully      (501) staff       (20)     4779 2020-03-05 10:34:43.000000 jesse-0.9.2/jesse/services/candle.py
+-rw-r--r--   0 sully      (501) staff       (20)     3934 2020-06-29 16:32:38.000000 jesse-0.9.2/jesse/services/charts.py
+-rw-r--r--   0 sully      (501) staff       (20)      678 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/db.py
+-rw-r--r--   0 sully      (501) staff       (20)     1471 2020-06-29 16:30:14.000000 jesse-0.9.2/jesse/services/file.py
+-rw-r--r--   0 sully      (501) staff       (20)     1074 2020-05-12 08:17:00.000000 jesse-0.9.2/jesse/services/logger.py
+-rw-r--r--   0 sully      (501) staff       (20)      607 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/notifier.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/project_maker/
+-rw-r--r--   0 sully      (501) staff       (20)     1024 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/project_maker/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/project_maker/project_template/
+-rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:41:52.000000 jesse-0.9.2/jesse/services/project_maker/project_template/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     3023 2020-07-08 09:02:35.000000 jesse-0.9.2/jesse/services/project_maker/project_template/config.py
+-rw-r--r--   0 sully      (501) staff       (20)      494 2020-06-19 15:25:26.000000 jesse-0.9.2/jesse/services/project_maker/project_template/routes.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/project_maker/project_template/storage/
+-rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:43:03.000000 jesse-0.9.2/jesse/services/project_maker/project_template/storage/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/project_maker/project_template/strategies/
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/project_maker/project_template/strategies/ExampleStrategy/
+-rw-r--r--   0 sully      (501) staff       (20)      321 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/project_maker/project_template/strategies/ExampleStrategy/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)        0 2020-04-07 06:42:57.000000 jesse-0.9.2/jesse/services/project_maker/project_template/strategies/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     9988 2020-06-09 09:02:25.000000 jesse-0.9.2/jesse/services/report.py
+-rw-r--r--   0 sully      (501) staff       (20)     5605 2020-07-08 09:01:36.000000 jesse-0.9.2/jesse/services/required_candles.py
+-rw-r--r--   0 sully      (501) staff       (20)      978 2020-06-19 16:37:42.000000 jesse-0.9.2/jesse/services/selectors.py
+-rw-r--r--   0 sully      (501) staff       (20)     6798 2020-06-09 09:02:25.000000 jesse-0.9.2/jesse/services/statistics.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/strategy_maker/
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/services/strategy_maker/ExampleStrategy/
+-rw-r--r--   0 sully      (501) staff       (20)      374 2020-06-25 13:49:43.000000 jesse-0.9.2/jesse/services/strategy_maker/ExampleStrategy/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)      882 2020-01-06 10:53:42.000000 jesse-0.9.2/jesse/services/strategy_maker/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)      817 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/services/table.py
+-rwxr-xr-x   0 sully      (501) staff       (20)     1507 2020-06-29 16:30:41.000000 jesse-0.9.2/jesse/services/tradingview.py
+-rw-r--r--   0 sully      (501) staff       (20)      265 2020-03-25 09:00:47.000000 jesse-0.9.2/jesse/services/validators.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/store/
+-rw-r--r--   0 sully      (501) staff       (20)     3798 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/store/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)      232 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/store/state_app.py
+-rw-r--r--   0 sully      (501) staff       (20)     9079 2020-06-28 08:04:56.000000 jesse-0.9.2/jesse/store/state_candles.py
+-rw-r--r--   0 sully      (501) staff       (20)      207 2019-09-03 15:07:20.000000 jesse-0.9.2/jesse/store/state_completed_trades.py
+-rw-r--r--   0 sully      (501) staff       (20)      414 2020-01-05 17:20:35.000000 jesse-0.9.2/jesse/store/state_exchanges.py
+-rw-r--r--   0 sully      (501) staff       (20)       89 2019-12-15 15:25:59.000000 jesse-0.9.2/jesse/store/state_logs.py
+-rw-r--r--   0 sully      (501) staff       (20)     4470 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/store/state_orderbook.py
+-rw-r--r--   0 sully      (501) staff       (20)     1945 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/store/state_orders.py
+-rw-r--r--   0 sully      (501) staff       (20)      563 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/store/state_positions.py
+-rw-r--r--   0 sully      (501) staff       (20)     1489 2020-04-01 09:01:16.000000 jesse-0.9.2/jesse/store/state_tickers.py
+-rw-r--r--   0 sully      (501) staff       (20)     2403 2020-04-01 09:01:16.000000 jesse-0.9.2/jesse/store/state_trades.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/
+-rw-r--r--   0 sully      (501) staff       (20)    41145 2020-06-19 16:39:51.000000 jesse-0.9.2/jesse/strategies/Strategy.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test01/
+-rw-r--r--   0 sully      (501) staff       (20)      522 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test01/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test02/
+-rw-r--r--   0 sully      (501) staff       (20)      587 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test02/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test03/
+-rw-r--r--   0 sully      (501) staff       (20)      652 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test03/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test04/
+-rw-r--r--   0 sully      (501) staff       (20)     1443 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test04/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test05/
+-rw-r--r--   0 sully      (501) staff       (20)      720 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test05/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test06/
+-rw-r--r--   0 sully      (501) staff       (20)     1081 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test06/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test07/
+-rw-r--r--   0 sully      (501) staff       (20)     1022 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test07/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test08/
+-rw-r--r--   0 sully      (501) staff       (20)      965 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test08/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test09/
+-rw-r--r--   0 sully      (501) staff       (20)      377 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test09/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test10/
+-rw-r--r--   0 sully      (501) staff       (20)      549 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test10/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test11/
+-rw-r--r--   0 sully      (501) staff       (20)      544 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test11/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test12/
+-rw-r--r--   0 sully      (501) staff       (20)      675 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test12/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test13/
+-rw-r--r--   0 sully      (501) staff       (20)      705 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test13/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test14/
+-rw-r--r--   0 sully      (501) staff       (20)      701 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test14/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test15/
+-rw-r--r--   0 sully      (501) staff       (20)      531 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test15/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test16/
+-rw-r--r--   0 sully      (501) staff       (20)      681 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test16/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test17/
+-rw-r--r--   0 sully      (501) staff       (20)      781 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test17/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test18/
+-rw-r--r--   0 sully      (501) staff       (20)      606 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test18/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test19/
+-rw-r--r--   0 sully      (501) staff       (20)      618 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test19/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test20/
+-rw-r--r--   0 sully      (501) staff       (20)      531 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test20/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test21/
+-rw-r--r--   0 sully      (501) staff       (20)      562 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test21/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test22/
+-rw-r--r--   0 sully      (501) staff       (20)      398 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test22/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test23/
+-rw-r--r--   0 sully      (501) staff       (20)      556 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test23/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test24/
+-rw-r--r--   0 sully      (501) staff       (20)      396 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test24/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test25/
+-rw-r--r--   0 sully      (501) staff       (20)      550 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test25/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test26/
+-rw-r--r--   0 sully      (501) staff       (20)      393 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test26/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test27/
+-rw-r--r--   0 sully      (501) staff       (20)      548 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test27/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test28/
+-rw-r--r--   0 sully      (501) staff       (20)      458 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test28/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test29/
+-rw-r--r--   0 sully      (501) staff       (20)     1250 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test29/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test30/
+-rw-r--r--   0 sully      (501) staff       (20)      790 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test30/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test31/
+-rw-r--r--   0 sully      (501) staff       (20)      584 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test31/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test32/
+-rw-r--r--   0 sully      (501) staff       (20)      513 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test32/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test33/
+-rw-r--r--   0 sully      (501) staff       (20)      439 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test33/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test34/
+-rw-r--r--   0 sully      (501) staff       (20)      624 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test34/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test35/
+-rw-r--r--   0 sully      (501) staff       (20)      727 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test35/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test36/
+-rw-r--r--   0 sully      (501) staff       (20)      948 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test36/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:10.000000 jesse-0.9.2/jesse/strategies/Test37/
+-rw-r--r--   0 sully      (501) staff       (20)      927 2020-05-14 08:24:39.000000 jesse-0.9.2/jesse/strategies/Test37/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test38/
+-rw-r--r--   0 sully      (501) staff       (20)      608 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test38/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test39/
+-rw-r--r--   0 sully      (501) staff       (20)      607 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test39/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test40/
+-rw-r--r--   0 sully      (501) staff       (20)      380 2020-04-16 07:03:33.000000 jesse-0.9.2/jesse/strategies/Test40/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test41/
+-rw-r--r--   0 sully      (501) staff       (20)      705 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test41/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test42/
+-rw-r--r--   0 sully      (501) staff       (20)      755 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test42/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test43/
+-rw-r--r--   0 sully      (501) staff       (20)      686 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test43/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test44/
+-rw-r--r--   0 sully      (501) staff       (20)      455 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test44/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test45/
+-rw-r--r--   0 sully      (501) staff       (20)      586 2020-05-05 10:32:25.000000 jesse-0.9.2/jesse/strategies/Test45/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test46/
+-rw-r--r--   0 sully      (501) staff       (20)      509 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/Test46/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test47/
+-rw-r--r--   0 sully      (501) staff       (20)      654 2020-06-04 07:23:46.000000 jesse-0.9.2/jesse/strategies/Test47/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/jesse/strategies/Test48/
+-rw-r--r--   0 sully      (501) staff       (20)      505 2020-06-19 16:48:52.000000 jesse-0.9.2/jesse/strategies/Test48/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)       31 2020-06-02 13:45:57.000000 jesse-0.9.2/jesse/strategies/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)     5886 2020-07-10 13:52:25.000000 jesse-0.9.2/jesse/utils.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/
+-rw-r--r--   0 sully      (501) staff       (20)     6544 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/PKG-INFO
+-rw-r--r--   0 sully      (501) staff       (20)     8323 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/SOURCES.txt
+-rw-r--r--   0 sully      (501) staff       (20)        1 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/dependency_links.txt
+-rw-r--r--   0 sully      (501) staff       (20)       64 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/entry_points.txt
+-rw-r--r--   0 sully      (501) staff       (20)      149 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/requires.txt
+-rw-r--r--   0 sully      (501) staff       (20)       12 2020-07-10 14:00:09.000000 jesse-0.9.2/jesse.egg-info/top_level.txt
+-rw-r--r--   0 sully      (501) staff       (20)       38 2020-07-10 14:00:11.000000 jesse-0.9.2/setup.cfg
+-rw-r--r--   0 sully      (501) staff       (20)     1393 2020-07-10 13:59:29.000000 jesse-0.9.2/setup.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/tests/
+-rw-r--r--   0 sully      (501) staff       (20)        0 2019-10-08 17:11:56.000000 jesse-0.9.2/tests/__init__.py
+drwxr-xr-x   0 sully      (501) staff       (20)        0 2020-07-10 14:00:11.000000 jesse-0.9.2/tests/data/
+-rw-r--r--   0 sully      (501) staff       (20)       86 2019-10-08 16:59:09.000000 jesse-0.9.2/tests/data/__init__.py
+-rw-r--r--   0 sully      (501) staff       (20)    96915 2019-07-05 07:23:38.000000 jesse-0.9.2/tests/data/test_candles_0.py
+-rw-r--r--   0 sully      (501) staff       (20)     4007 2019-07-04 09:14:19.000000 jesse-0.9.2/tests/data/test_candles_1.py
+-rw-r--r--   0 sully      (501) staff       (20)   397893 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/data/test_candles_indicators.py
+-rw-r--r--   0 sully      (501) staff       (20)     4312 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_backtest.py
+-rw-r--r--   0 sully      (501) staff       (20)    11538 2020-06-14 10:29:43.000000 jesse-0.9.2/tests/test_broker.py
+-rw-r--r--   0 sully      (501) staff       (20)     4352 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_candle_service.py
+-rw-r--r--   0 sully      (501) staff       (20)     3086 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_conflicting_orders.py
+-rw-r--r--   0 sully      (501) staff       (20)     1071 2020-06-19 14:11:38.000000 jesse-0.9.2/tests/test_exchange.py
+-rw-r--r--   0 sully      (501) staff       (20)    10547 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_helpers.py
+-rw-r--r--   0 sully      (501) staff       (20)     2676 2020-03-18 16:10:57.000000 jesse-0.9.2/tests/test_import_candles.py
+-rw-r--r--   0 sully      (501) staff       (20)    36841 2020-06-04 07:25:44.000000 jesse-0.9.2/tests/test_indicators.py
+-rw-r--r--   0 sully      (501) staff       (20)     7110 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_metrics.py
+-rw-r--r--   0 sully      (501) staff       (20)     1042 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_order.py
+-rw-r--r--   0 sully      (501) staff       (20)    30016 2020-06-19 16:47:59.000000 jesse-0.9.2/tests/test_parent_strategy.py
+-rw-r--r--   0 sully      (501) staff       (20)     5781 2020-02-27 16:19:06.000000 jesse-0.9.2/tests/test_position.py
+-rw-r--r--   0 sully      (501) staff       (20)     1255 2020-01-18 18:21:36.000000 jesse-0.9.2/tests/test_router.py
+-rw-r--r--   0 sully      (501) staff       (20)     4656 2020-06-28 08:05:07.000000 jesse-0.9.2/tests/test_state_candle.py
+-rw-r--r--   0 sully      (501) staff       (20)      616 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_state_exchanges.py
+-rw-r--r--   0 sully      (501) staff       (20)     1082 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_state_logs.py
+-rw-r--r--   0 sully      (501) staff       (20)    11074 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_state_orderbook.py
+-rw-r--r--   0 sully      (501) staff       (20)     2130 2020-06-02 13:45:57.000000 jesse-0.9.2/tests/test_state_orders.py
+-rw-r--r--   0 sully      (501) staff       (20)     1888 2020-02-06 09:25:52.000000 jesse-0.9.2/tests/test_state_ticker.py
+-rw-r--r--   0 sully      (501) staff       (20)     2960 2020-01-18 18:21:36.000000 jesse-0.9.2/tests/test_state_trades.py
+-rw-r--r--   0 sully      (501) staff       (20)     4219 2020-06-25 13:50:51.000000 jesse-0.9.2/tests/test_strategy_utils.py
+-rw-r--r--   0 sully      (501) staff       (20)     3875 2020-02-27 16:38:41.000000 jesse-0.9.2/tests/test_trade.py
```

### Comparing `jesse-0.9.1/PKG-INFO` & `jesse-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesse
-Version: 0.9.1
+Version: 0.9.2
 Summary: A trading framework for cryptocurrencies
 Home-page: https://jesse-ai.com
 Author: Saleh Mirnezami
 Author-email: mirnezami.saleh@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://docs.jesse-ai.com
 Project-URL: Say Thanks!, http://forum.jesse-ai.com/
```

### Comparing `jesse-0.9.1/README.md` & `jesse-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/assets/chart-example.png` & `jesse-0.9.2/assets/chart-example.png`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/__init__.py` & `jesse-0.9.2/jesse/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/config.py` & `jesse-0.9.2/jesse/config.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/enums/__init__.py` & `jesse-0.9.2/jesse/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/exceptions/__init__.py` & `jesse-0.9.2/jesse/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/exchanges/exchange.py` & `jesse-0.9.2/jesse/exchanges/exchange.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/exchanges/sandbox/Sandbox.py` & `jesse-0.9.2/jesse/exchanges/sandbox/Sandbox.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/factories/candle_factory.py` & `jesse-0.9.2/jesse/factories/candle_factory.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/factories/order_factory.py` & `jesse-0.9.2/jesse/factories/order_factory.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/helpers.py` & `jesse-0.9.2/jesse/helpers.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/__init__.py` & `jesse-0.9.2/jesse/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/acosc.py` & `jesse-0.9.2/jesse/indicators/acosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ad.py` & `jesse-0.9.2/jesse/indicators/ad.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/adosc.py` & `jesse-0.9.2/jesse/indicators/adosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/adx.py` & `jesse-0.9.2/jesse/indicators/adx.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/adxr.py` & `jesse-0.9.2/jesse/indicators/adxr.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/alligator.py` & `jesse-0.9.2/jesse/indicators/alligator.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ao.py` & `jesse-0.9.2/jesse/indicators/ao.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/apo.py` & `jesse-0.9.2/jesse/indicators/apo.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/aroon.py` & `jesse-0.9.2/jesse/indicators/aroon.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/aroonosc.py` & `jesse-0.9.2/jesse/indicators/aroonosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/atr.py` & `jesse-0.9.2/jesse/indicators/atr.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/avgprice.py` & `jesse-0.9.2/jesse/indicators/avgprice.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/beta.py` & `jesse-0.9.2/jesse/indicators/beta.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/bollinger_bands.py` & `jesse-0.9.2/jesse/indicators/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/bollinger_bands_width.py` & `jesse-0.9.2/jesse/indicators/bollinger_bands_width.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/bop.py` & `jesse-0.9.2/jesse/indicators/bop.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/cci.py` & `jesse-0.9.2/jesse/indicators/cci.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/cmo.py` & `jesse-0.9.2/jesse/indicators/cmo.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/correl.py` & `jesse-0.9.2/jesse/indicators/correl.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/cvi.py` & `jesse-0.9.2/jesse/indicators/cvi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/dec_osc.py` & `jesse-0.9.2/jesse/indicators/dec_osc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/decycler.py` & `jesse-0.9.2/jesse/indicators/decycler.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/dema.py` & `jesse-0.9.2/jesse/indicators/dema.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/di.py` & `jesse-0.9.2/jesse/indicators/di.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/dm.py` & `jesse-0.9.2/jesse/indicators/dm.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/donchian.py` & `jesse-0.9.2/jesse/indicators/donchian.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/dpo.py` & `jesse-0.9.2/jesse/indicators/dpo.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/dx.py` & `jesse-0.9.2/jesse/indicators/dx.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ema.py` & `jesse-0.9.2/jesse/indicators/ema.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/emd.py` & `jesse-0.9.2/jesse/indicators/emd.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/emv.py` & `jesse-0.9.2/jesse/indicators/emv.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/fisher.py` & `jesse-0.9.2/jesse/indicators/fisher.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/fosc.py` & `jesse-0.9.2/jesse/indicators/fosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/frama.py` & `jesse-0.9.2/jesse/indicators/frama.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/gatorosc.py` & `jesse-0.9.2/jesse/indicators/gatorosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/gauss.py` & `jesse-0.9.2/jesse/indicators/gauss.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/hma.py` & `jesse-0.9.2/jesse/indicators/hma.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_dcperiod.py` & `jesse-0.9.2/jesse/indicators/ht_dcperiod.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_dcphase.py` & `jesse-0.9.2/jesse/indicators/ht_dcphase.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_phasor.py` & `jesse-0.9.2/jesse/indicators/ht_phasor.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_sine.py` & `jesse-0.9.2/jesse/indicators/ht_sine.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_trendline.py` & `jesse-0.9.2/jesse/indicators/ht_trendline.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ht_trendmode.py` & `jesse-0.9.2/jesse/indicators/ht_trendmode.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ichimoku_cloud.py` & `jesse-0.9.2/jesse/indicators/ichimoku_cloud.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/itrend.py` & `jesse-0.9.2/jesse/indicators/itrend.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/kama.py` & `jesse-0.9.2/jesse/indicators/kama.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/keltner.py` & `jesse-0.9.2/jesse/indicators/keltner.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/kvo.py` & `jesse-0.9.2/jesse/indicators/kvo.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/linearreg.py` & `jesse-0.9.2/jesse/indicators/linearreg.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/linearreg_angle.py` & `jesse-0.9.2/jesse/indicators/linearreg_angle.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/linearreg_intercept.py` & `jesse-0.9.2/jesse/indicators/linearreg_intercept.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/linearreg_slope.py` & `jesse-0.9.2/jesse/indicators/linearreg_slope.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/lrsi.py` & `jesse-0.9.2/jesse/indicators/lrsi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/macd.py` & `jesse-0.9.2/jesse/indicators/macd.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/macdext.py` & `jesse-0.9.2/jesse/indicators/macdext.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/mama.py` & `jesse-0.9.2/jesse/indicators/mama.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/marketfi.py` & `jesse-0.9.2/jesse/indicators/marketfi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/mass.py` & `jesse-0.9.2/jesse/indicators/mass.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/medprice.py` & `jesse-0.9.2/jesse/indicators/medprice.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/mfi.py` & `jesse-0.9.2/jesse/indicators/mfi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/midpoint.py` & `jesse-0.9.2/jesse/indicators/midpoint.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/midprice.py` & `jesse-0.9.2/jesse/indicators/midprice.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/minmax.py` & `jesse-0.9.2/jesse/indicators/minmax.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/mom.py` & `jesse-0.9.2/jesse/indicators/mom.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/msw.py` & `jesse-0.9.2/jesse/indicators/msw.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/natr.py` & `jesse-0.9.2/jesse/indicators/natr.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/nvi.py` & `jesse-0.9.2/jesse/indicators/nvi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/obv.py` & `jesse-0.9.2/jesse/indicators/obv.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/pattern_recognition.py` & `jesse-0.9.2/jesse/indicators/pattern_recognition.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/pivot.py` & `jesse-0.9.2/jesse/indicators/pivot.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ppo.py` & `jesse-0.9.2/jesse/indicators/ppo.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/pvi.py` & `jesse-0.9.2/jesse/indicators/pvi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/qstick.py` & `jesse-0.9.2/jesse/indicators/qstick.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/roc.py` & `jesse-0.9.2/jesse/indicators/roc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/rocp.py` & `jesse-0.9.2/jesse/indicators/rocp.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/rocr.py` & `jesse-0.9.2/jesse/indicators/rocr.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/rocr100.py` & `jesse-0.9.2/jesse/indicators/rocr100.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/rsi.py` & `jesse-0.9.2/jesse/indicators/rsi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/sar.py` & `jesse-0.9.2/jesse/indicators/sar.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/sarext.py` & `jesse-0.9.2/jesse/indicators/sarext.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/sma.py` & `jesse-0.9.2/jesse/indicators/sma.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/smma.py` & `jesse-0.9.2/jesse/indicators/smma.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/srsi.py` & `jesse-0.9.2/jesse/indicators/srsi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/stddev.py` & `jesse-0.9.2/jesse/indicators/stddev.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/stochastic.py` & `jesse-0.9.2/jesse/indicators/stochastic.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/stochf.py` & `jesse-0.9.2/jesse/indicators/stochf.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/supersmoother.py` & `jesse-0.9.2/jesse/indicators/supersmoother.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/supertrend.py` & `jesse-0.9.2/jesse/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/t3.py` & `jesse-0.9.2/jesse/indicators/t3.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/tema.py` & `jesse-0.9.2/jesse/indicators/tema.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/trange.py` & `jesse-0.9.2/jesse/indicators/trange.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/trima.py` & `jesse-0.9.2/jesse/indicators/trima.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/trix.py` & `jesse-0.9.2/jesse/indicators/trix.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/tsf.py` & `jesse-0.9.2/jesse/indicators/tsf.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/tsi.py` & `jesse-0.9.2/jesse/indicators/tsi.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/typprice.py` & `jesse-0.9.2/jesse/indicators/typprice.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/ultosc.py` & `jesse-0.9.2/jesse/indicators/ultosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/var.py` & `jesse-0.9.2/jesse/indicators/var.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/vidya.py` & `jesse-0.9.2/jesse/indicators/vidya.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/vosc.py` & `jesse-0.9.2/jesse/indicators/vosc.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/vwma.py` & `jesse-0.9.2/jesse/indicators/vwma.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/vwmacd.py` & `jesse-0.9.2/jesse/indicators/vwmacd.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/wad.py` & `jesse-0.9.2/jesse/indicators/wad.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/wclprice.py` & `jesse-0.9.2/jesse/indicators/wclprice.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/wilders.py` & `jesse-0.9.2/jesse/indicators/wilders.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/willr.py` & `jesse-0.9.2/jesse/indicators/willr.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/wma.py` & `jesse-0.9.2/jesse/indicators/wma.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/zlema.py` & `jesse-0.9.2/jesse/indicators/zlema.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/indicators/zscore.py` & `jesse-0.9.2/jesse/indicators/zscore.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/libs/dynamic_numpy_array/__init__.py` & `jesse-0.9.2/jesse/libs/dynamic_numpy_array/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Candle.py` & `jesse-0.9.2/jesse/models/Candle.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/CompletedTrade.py` & `jesse-0.9.2/jesse/models/CompletedTrade.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Exchange.py` & `jesse-0.9.2/jesse/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Order.py` & `jesse-0.9.2/jesse/models/Order.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Orderbook.py` & `jesse-0.9.2/jesse/models/Orderbook.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Position.py` & `jesse-0.9.2/jesse/models/Position.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Ticker.py` & `jesse-0.9.2/jesse/models/Ticker.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/Trade.py` & `jesse-0.9.2/jesse/models/Trade.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/models/utils.py` & `jesse-0.9.2/jesse/models/utils.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/backtest_mode/__init__.py` & `jesse-0.9.2/jesse/modes/backtest_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/__init__.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/drivers/binance.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/drivers/binance.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/drivers/binance_futures.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/drivers/binance_futures.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/drivers/bitfinex.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/drivers/bitfinex.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/drivers/coinbase.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/drivers/coinbase.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/import_candles_mode/drivers/testnet_binance_futures.py` & `jesse-0.9.2/jesse/modes/import_candles_mode/drivers/testnet_binance_futures.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/optimize_mode/Genetics.py` & `jesse-0.9.2/jesse/modes/optimize_mode/Genetics.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/optimize_mode/__init__.py` & `jesse-0.9.2/jesse/modes/optimize_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/modes/routes_mode/__init__.py` & `jesse-0.9.2/jesse/modes/routes_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/research/__init__.py` & `jesse-0.9.2/jesse/research/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/research/get_candles.py` & `jesse-0.9.2/jesse/research/get_candles.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/routes/__init__.py` & `jesse-0.9.2/jesse/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/api.py` & `jesse-0.9.2/jesse/services/api.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/broker.py` & `jesse-0.9.2/jesse/services/broker.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/cache.py` & `jesse-0.9.2/jesse/services/cache.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/candle.py` & `jesse-0.9.2/jesse/services/candle.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/charts.py` & `jesse-0.9.2/jesse/services/charts.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/db.py` & `jesse-0.9.2/jesse/services/db.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/file.py` & `jesse-0.9.2/jesse/services/file.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/logger.py` & `jesse-0.9.2/jesse/services/logger.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/notifier.py` & `jesse-0.9.2/jesse/services/notifier.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/project_maker/__init__.py` & `jesse-0.9.2/jesse/services/project_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/project_maker/project_template/config.py` & `jesse-0.9.2/jesse/services/project_maker/project_template/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,9 +85,10 @@
         'omega_ratio': False,
         'winning_streak': False,
         'losing_streak': False,
         'largest_losing_trade': False,
         'largest_winning_trade': False,
         'total_winning_trades': False,
         'total_losing_trades': False,
+
     }
 }
```

### Comparing `jesse-0.9.1/jesse/services/report.py` & `jesse-0.9.2/jesse/services/report.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/required_candles.py` & `jesse-0.9.2/jesse/services/required_candles.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/selectors.py` & `jesse-0.9.2/jesse/services/selectors.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/statistics.py` & `jesse-0.9.2/jesse/services/statistics.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/strategy_maker/__init__.py` & `jesse-0.9.2/jesse/services/strategy_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/table.py` & `jesse-0.9.2/jesse/services/table.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/services/tradingview.py` & `jesse-0.9.2/jesse/services/tradingview.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/__init__.py` & `jesse-0.9.2/jesse/store/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_candles.py` & `jesse-0.9.2/jesse/store/state_candles.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_orderbook.py` & `jesse-0.9.2/jesse/store/state_orderbook.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_orders.py` & `jesse-0.9.2/jesse/store/state_orders.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_positions.py` & `jesse-0.9.2/jesse/store/state_positions.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_tickers.py` & `jesse-0.9.2/jesse/store/state_tickers.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/store/state_trades.py` & `jesse-0.9.2/jesse/store/state_trades.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Strategy.py` & `jesse-0.9.2/jesse/strategies/Strategy.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test01/__init__.py` & `jesse-0.9.2/jesse/strategies/Test01/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test02/__init__.py` & `jesse-0.9.2/jesse/strategies/Test02/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test03/__init__.py` & `jesse-0.9.2/jesse/strategies/Test03/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test04/__init__.py` & `jesse-0.9.2/jesse/strategies/Test04/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test05/__init__.py` & `jesse-0.9.2/jesse/strategies/Test05/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test06/__init__.py` & `jesse-0.9.2/jesse/strategies/Test06/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test07/__init__.py` & `jesse-0.9.2/jesse/strategies/Test07/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test08/__init__.py` & `jesse-0.9.2/jesse/strategies/Test08/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test10/__init__.py` & `jesse-0.9.2/jesse/strategies/Test10/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test11/__init__.py` & `jesse-0.9.2/jesse/strategies/Test11/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test12/__init__.py` & `jesse-0.9.2/jesse/strategies/Test12/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test13/__init__.py` & `jesse-0.9.2/jesse/strategies/Test13/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test14/__init__.py` & `jesse-0.9.2/jesse/strategies/Test14/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test15/__init__.py` & `jesse-0.9.2/jesse/strategies/Test15/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test16/__init__.py` & `jesse-0.9.2/jesse/strategies/Test16/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test17/__init__.py` & `jesse-0.9.2/jesse/strategies/Test17/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test18/__init__.py` & `jesse-0.9.2/jesse/strategies/Test18/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test19/__init__.py` & `jesse-0.9.2/jesse/strategies/Test19/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test20/__init__.py` & `jesse-0.9.2/jesse/strategies/Test20/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test21/__init__.py` & `jesse-0.9.2/jesse/strategies/Test21/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test23/__init__.py` & `jesse-0.9.2/jesse/strategies/Test23/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test25/__init__.py` & `jesse-0.9.2/jesse/strategies/Test25/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test27/__init__.py` & `jesse-0.9.2/jesse/strategies/Test27/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test29/__init__.py` & `jesse-0.9.2/jesse/strategies/Test29/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test30/__init__.py` & `jesse-0.9.2/jesse/strategies/Test30/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test31/__init__.py` & `jesse-0.9.2/jesse/strategies/Test31/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test32/__init__.py` & `jesse-0.9.2/jesse/strategies/Test32/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test34/__init__.py` & `jesse-0.9.2/jesse/strategies/Test34/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test35/__init__.py` & `jesse-0.9.2/jesse/strategies/Test35/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test36/__init__.py` & `jesse-0.9.2/jesse/strategies/Test36/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test37/__init__.py` & `jesse-0.9.2/jesse/strategies/Test37/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test38/__init__.py` & `jesse-0.9.2/jesse/strategies/Test38/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test39/__init__.py` & `jesse-0.9.2/jesse/strategies/Test39/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test41/__init__.py` & `jesse-0.9.2/jesse/strategies/Test41/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test42/__init__.py` & `jesse-0.9.2/jesse/strategies/Test42/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test43/__init__.py` & `jesse-0.9.2/jesse/strategies/Test43/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test45/__init__.py` & `jesse-0.9.2/jesse/strategies/Test45/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/strategies/Test47/__init__.py` & `jesse-0.9.2/jesse/strategies/Test47/__init__.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/jesse/utils.py` & `jesse-0.9.2/jesse/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     :param fee_rate:
     :return: float
     """
     risk_per_qty = abs(entry_price - stop_loss_price)
     size = risk_to_size(capital, risk_per_capital, risk_per_qty, entry_price)
 
     if fee_rate != 0:
-        size = size * (1 - fee_rate*2)
+        size = size * (1 - fee_rate*3)
 
     return size_to_qty(size, entry_price, fee_rate=fee_rate)
 
 
 def size_to_qty(position_size, entry_price, precision=3, fee_rate=0) -> float:
     """
     converts position-size to quantity
@@ -55,15 +55,15 @@
     :param fee_rate:
     :return: float
     """
     if math.isnan(position_size) or math.isnan(entry_price):
         raise TypeError()
 
     if fee_rate != 0:
-        position_size = position_size * (1 - fee_rate*2)
+        position_size = position_size * (1 - fee_rate*3)
 
     return round(position_size / entry_price, precision)
 
 
 def qty_to_size(qty, price) -> float:
     """
     converts quantity to position-size
```

### Comparing `jesse-0.9.1/jesse.egg-info/PKG-INFO` & `jesse-0.9.2/jesse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jesse
-Version: 0.9.1
+Version: 0.9.2
 Summary: A trading framework for cryptocurrencies
 Home-page: https://jesse-ai.com
 Author: Saleh Mirnezami
 Author-email: mirnezami.saleh@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://docs.jesse-ai.com
 Project-URL: Say Thanks!, http://forum.jesse-ai.com/
```

### Comparing `jesse-0.9.1/jesse.egg-info/SOURCES.txt` & `jesse-0.9.2/jesse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/setup.py` & `jesse-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.9.1'
+VERSION = '0.9.2'
 DESCRIPTION = "A trading framework for cryptocurrencies"
 REQUIRED_PACKAGES = [
     'psycopg2-binary',
     'pytest',
     'Click',
     'arrow',
     'requests',
```

### Comparing `jesse-0.9.1/tests/data/test_candles_0.py` & `jesse-0.9.2/tests/data/test_candles_0.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/data/test_candles_1.py` & `jesse-0.9.2/tests/data/test_candles_1.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/data/test_candles_indicators.py` & `jesse-0.9.2/tests/data/test_candles_indicators.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_backtest.py` & `jesse-0.9.2/tests/test_backtest.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_broker.py` & `jesse-0.9.2/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_candle_service.py` & `jesse-0.9.2/tests/test_candle_service.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_conflicting_orders.py` & `jesse-0.9.2/tests/test_conflicting_orders.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_exchange.py` & `jesse-0.9.2/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_helpers.py` & `jesse-0.9.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_import_candles.py` & `jesse-0.9.2/tests/test_import_candles.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_indicators.py` & `jesse-0.9.2/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_metrics.py` & `jesse-0.9.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_order.py` & `jesse-0.9.2/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_parent_strategy.py` & `jesse-0.9.2/tests/test_parent_strategy.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_position.py` & `jesse-0.9.2/tests/test_position.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_router.py` & `jesse-0.9.2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_candle.py` & `jesse-0.9.2/tests/test_state_candle.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_exchanges.py` & `jesse-0.9.2/tests/test_state_exchanges.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_logs.py` & `jesse-0.9.2/tests/test_state_logs.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_orderbook.py` & `jesse-0.9.2/tests/test_state_orderbook.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_orders.py` & `jesse-0.9.2/tests/test_state_orders.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_ticker.py` & `jesse-0.9.2/tests/test_state_ticker.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_state_trades.py` & `jesse-0.9.2/tests/test_state_trades.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_strategy_utils.py` & `jesse-0.9.2/tests/test_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `jesse-0.9.1/tests/test_trade.py` & `jesse-0.9.2/tests/test_trade.py`

 * *Files identical despite different names*

