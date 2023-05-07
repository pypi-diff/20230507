# Comparing `tmp/miniaudio-1.8.tar.gz` & `tmp/miniaudio-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/miniaudio-1.8.tar", last modified: Mon Oct 21 18:44:22 2019, max compression
+gzip compressed data, was "dist/miniaudio-1.9.tar", last modified: Sat Jan 11 01:00:36 2020, max compression
```

## Comparing `miniaudio-1.8.tar` & `miniaudio-1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 irmen     (1000) irmendj   (1000)        0 2019-10-21 18:44:22.000000 miniaudio-1.8/
--rw-r--r--   0 irmen     (1000) irmendj   (1000)     1166 2019-06-15 12:41:25.000000 miniaudio-1.8/LICENSE
--rw-r--r--   0 irmen     (1000) irmendj   (1000)       92 2019-07-04 21:04:27.000000 miniaudio-1.8/MANIFEST.in
--rw-r--r--   0 irmen     (1000) irmendj   (1000)      612 2019-10-21 14:42:47.000000 miniaudio-1.8/Makefile
--rw-r--r--   0 irmen     (1000) irmendj   (1000)    25753 2019-10-21 18:44:22.000000 miniaudio-1.8/PKG-INFO
--rw-r--r--   0 irmen     (1000) irmendj   (1000)    21205 2019-08-12 19:16:02.000000 miniaudio-1.8/README.md
--rw-r--r--   0 irmen     (1000) irmendj   (1000)    34363 2019-10-21 18:10:38.000000 miniaudio-1.8/build_ffi_module.py
-drwxr-xr-x   0 irmen     (1000) irmendj   (1000)        0 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio/
--rw-r--r--   0 irmen     (1000) irmendj   (1000)   466760 2019-10-21 12:46:36.000000 miniaudio-1.8/miniaudio/dr_flac.h
--rw-r--r--   0 irmen     (1000) irmendj   (1000)   165665 2019-10-21 12:46:37.000000 miniaudio-1.8/miniaudio/dr_mp3.h
--rw-r--r--   0 irmen     (1000) irmendj   (1000)   201294 2019-10-21 12:46:37.000000 miniaudio-1.8/miniaudio/dr_wav.h
--rw-r--r--   0 irmen     (1000) irmendj   (1000)  1567578 2019-10-21 12:46:21.000000 miniaudio-1.8/miniaudio/miniaudio.h
--rw-r--r--   0 irmen     (1000) irmendj   (1000)   187320 2019-10-21 12:46:38.000000 miniaudio-1.8/miniaudio/stb_vorbis.c
--rw-r--r--   0 irmen     (1000) irmendj   (1000)     1768 2019-07-06 14:16:00.000000 miniaudio-1.8/miniaudio.c
-drwxr-xr-x   0 irmen     (1000) irmendj   (1000)        0 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/
--rw-r--r--   0 irmen     (1000) irmendj   (1000)    25753 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/PKG-INFO
--rw-r--r--   0 irmen     (1000) irmendj   (1000)      401 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/SOURCES.txt
--rw-r--r--   0 irmen     (1000) irmendj   (1000)        1 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/dependency_links.txt
--rw-r--r--   0 irmen     (1000) irmendj   (1000)        1 2019-07-05 01:45:15.000000 miniaudio-1.8/miniaudio.egg-info/not-zip-safe
--rw-r--r--   0 irmen     (1000) irmendj   (1000)       12 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/requires.txt
--rw-r--r--   0 irmen     (1000) irmendj   (1000)       21 2019-10-21 18:44:22.000000 miniaudio-1.8/miniaudio.egg-info/top_level.txt
--rw-r--r--   0 irmen     (1000) irmendj   (1000)    74607 2019-10-21 18:31:17.000000 miniaudio-1.8/miniaudio.py
--rw-r--r--   0 irmen     (1000) irmendj   (1000)     1055 2019-10-21 18:44:22.000000 miniaudio-1.8/setup.cfg
--rw-r--r--   0 irmen     (1000) irmendj   (1000)     3933 2019-07-07 20:55:38.000000 miniaudio-1.8/setup.py
+drwxr-xr-x   0 irmen     (1000) irmen     (1000)        0 2020-01-11 01:00:36.730367 miniaudio-1.9/
+-rw-r--r--   0 irmen     (1000) irmen     (1000)     1166 2019-06-15 12:41:25.000000 miniaudio-1.9/LICENSE
+-rw-r--r--   0 irmen     (1000) irmen     (1000)       92 2019-07-04 21:04:27.000000 miniaudio-1.9/MANIFEST.in
+-rw-r--r--   0 irmen     (1000) irmen     (1000)      752 2019-10-22 13:51:51.000000 miniaudio-1.9/Makefile
+-rw-r--r--   0 irmen     (1000) irmen     (1000)    25753 2020-01-11 01:00:36.733700 miniaudio-1.9/PKG-INFO
+-rw-r--r--   0 irmen     (1000) irmen     (1000)    21205 2019-08-12 19:16:02.000000 miniaudio-1.9/README.md
+-rw-r--r--   0 irmen     (1000) irmen     (1000)    34537 2020-01-11 00:20:34.000000 miniaudio-1.9/build_ffi_module.py
+drwxr-xr-x   0 irmen     (1000) irmen     (1000)        0 2020-01-11 01:00:36.730367 miniaudio-1.9/miniaudio/
+-rw-r--r--   0 irmen     (1000) irmen     (1000)   467789 2020-01-11 00:08:50.000000 miniaudio-1.9/miniaudio/dr_flac.h
+-rw-r--r--   0 irmen     (1000) irmen     (1000)   166116 2020-01-11 00:08:50.000000 miniaudio-1.9/miniaudio/dr_mp3.h
+-rw-r--r--   0 irmen     (1000) irmen     (1000)   202316 2020-01-11 00:08:50.000000 miniaudio-1.9/miniaudio/dr_wav.h
+-rw-r--r--   0 irmen     (1000) irmen     (1000)  1585522 2020-01-11 00:08:50.000000 miniaudio-1.9/miniaudio/miniaudio.h
+-rw-r--r--   0 irmen     (1000) irmen     (1000)   187320 2020-01-11 00:08:50.000000 miniaudio-1.9/miniaudio/stb_vorbis.c
+-rw-r--r--   0 irmen     (1000) irmen     (1000)     1768 2019-07-06 14:16:00.000000 miniaudio-1.9/miniaudio.c
+drwxr-xr-x   0 irmen     (1000) irmen     (1000)        0 2020-01-11 01:00:36.730367 miniaudio-1.9/miniaudio.egg-info/
+-rw-r--r--   0 irmen     (1000) irmen     (1000)    25753 2020-01-11 01:00:36.000000 miniaudio-1.9/miniaudio.egg-info/PKG-INFO
+-rw-r--r--   0 irmen     (1000) irmen     (1000)      401 2020-01-11 01:00:36.000000 miniaudio-1.9/miniaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 irmen     (1000) irmen     (1000)        1 2020-01-11 01:00:36.000000 miniaudio-1.9/miniaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 irmen     (1000) irmen     (1000)        1 2019-07-05 01:45:15.000000 miniaudio-1.9/miniaudio.egg-info/not-zip-safe
+-rw-r--r--   0 irmen     (1000) irmen     (1000)       12 2020-01-11 01:00:36.000000 miniaudio-1.9/miniaudio.egg-info/requires.txt
+-rw-r--r--   0 irmen     (1000) irmen     (1000)       21 2020-01-11 01:00:36.000000 miniaudio-1.9/miniaudio.egg-info/top_level.txt
+-rw-r--r--   0 irmen     (1000) irmen     (1000)    74607 2020-01-11 00:12:19.000000 miniaudio-1.9/miniaudio.py
+-rw-r--r--   0 irmen     (1000) irmen     (1000)     1055 2020-01-11 01:00:36.733700 miniaudio-1.9/setup.cfg
+-rw-r--r--   0 irmen     (1000) irmen     (1000)     3933 2019-07-07 20:55:38.000000 miniaudio-1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `miniaudio-1.8/LICENSE` & `miniaudio-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miniaudio-1.8/PKG-INFO` & `miniaudio-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniaudio
-Version: 1.8
+Version: 1.9
 Summary: python bindings for the miniaudio library and its decoders (mp3, flac, ogg vorbis, wav)
 Home-page: https://github.com/irmen/pyminiaudio
 Author: Irmen de Jong
 Author-email: irmen@razorvine.net
 License: MIT
 Description: [![saythanks](https://img.shields.io/badge/say-thanks-ff69b4.svg)](https://saythanks.io/to/irmen)
         [![Latest Version](https://img.shields.io/pypi/v/miniaudio.svg)](https://pypi.python.org/pypi/miniaudio/)
```

### Comparing `miniaudio-1.8/README.md` & `miniaudio-1.9/README.md`

 * *Files identical despite different names*

### Comparing `miniaudio-1.8/build_ffi_module.py` & `miniaudio-1.9/build_ffi_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,14 +525,16 @@
         ma_channel channelMap[MA_MAX_CHANNELS];
         ma_share_mode shareMode;
     } capture;
     struct
     {
         ma_bool32 noAutoConvertSRC;     /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_AUTOCONVERTPCM. */
         ma_bool32 noDefaultQualitySRC;  /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_SRC_DEFAULT_QUALITY. */
+        ma_bool32 noAutoStreamRouting;  /* Disables automatic stream routing. */
+        ma_bool32 noHardwareOffloading; /* Disables WASAPI's hardware offloading feature. */
     } wasapi;
     struct
     {
         ma_bool32 noMMap;  /* Disables MMap mode. */
     } alsa;
     struct
     {
```

### Comparing `miniaudio-1.8/miniaudio/dr_flac.h` & `miniaudio-1.9/miniaudio/dr_flac.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 FLAC audio decoder. Choice of public domain or MIT-0. See license statements at the end of this file.
-dr_flac - v0.12.2 - 2019-10-07
+dr_flac - v0.12.3 - 2019-12-02
 
 David Reid - mackron@gmail.com
 */
 
 /*
 RELEASE NOTES - v0.12.0
 =======================
@@ -551,19 +551,22 @@
     drflac_int32* pSamplesS32;
 } drflac_subframe;
 
 typedef struct
 {
     /*
     If the stream uses variable block sizes, this will be set to the index of the first PCM frame. If fixed block sizes are used, this will
-    always be set to 0.
+    always be set to 0. This is 64-bit because the decoded PCM frame number will be 36 bits.
     */
     drflac_uint64 pcmFrameNumber;
 
-    /* If the stream uses fixed block sizes, this will be set to the frame number. If variable block sizes are used, this will always be 0. */
+    /*
+    If the stream uses fixed block sizes, this will be set to the frame number. If variable block sizes are used, this will always be 0. This
+    is 32-bit because in fixed block sizes, the maximum frame number will be 31 bits.
+    */
     drflac_uint32 flacFrameNumber;
 
     /* The sample rate of this frame. */
     drflac_uint32 sampleRate;
 
     /* The number of PCM frames in each sub-frame within this frame. */
     drflac_uint16 blockSizeInPCMFrames;
@@ -3137,22 +3140,22 @@
 
     return DRFLAC_TRUE;
 }
 
 static drflac_bool32 drflac__decode_samples_with_residual__rice__scalar(drflac_bs* bs, drflac_uint32 bitsPerSample, drflac_uint32 count, drflac_uint8 riceParam, drflac_uint32 order, drflac_int32 shift, const drflac_int32* coefficients, drflac_int32* pSamplesOut)
 {
     drflac_uint32 t[2] = {0x00000000, 0xFFFFFFFF};
-    drflac_uint32 zeroCountPart0;
-    drflac_uint32 zeroCountPart1;
-    drflac_uint32 zeroCountPart2;
-    drflac_uint32 zeroCountPart3;
-    drflac_uint32 riceParamPart0;
-    drflac_uint32 riceParamPart1;
-    drflac_uint32 riceParamPart2;
-    drflac_uint32 riceParamPart3;
+    drflac_uint32 zeroCountPart0 = 0;
+    drflac_uint32 zeroCountPart1 = 0;
+    drflac_uint32 zeroCountPart2 = 0;
+    drflac_uint32 zeroCountPart3 = 0;
+    drflac_uint32 riceParamPart0 = 0;
+    drflac_uint32 riceParamPart1 = 0;
+    drflac_uint32 riceParamPart2 = 0;
+    drflac_uint32 riceParamPart3 = 0;
     drflac_uint32 riceParamMask;
     const drflac_int32* pSamplesOutEnd;
     drflac_uint32 i;
 
     DRFLAC_ASSERT(bs != NULL);
     DRFLAC_ASSERT(count > 0);
     DRFLAC_ASSERT(pSamplesOut != NULL);
@@ -3312,22 +3315,22 @@
 
 static drflac_bool32 drflac__decode_samples_with_residual__rice__sse41_32(drflac_bs* bs, drflac_uint32 count, drflac_uint8 riceParam, drflac_uint32 order, drflac_int32 shift, const drflac_int32* coefficients, drflac_int32* pSamplesOut)
 {
     int i;
     drflac_uint32 riceParamMask;
     drflac_int32* pDecodedSamples    = pSamplesOut;
     drflac_int32* pDecodedSamplesEnd = pSamplesOut + (count & ~3);
-    drflac_uint32 zeroCountParts0;
-    drflac_uint32 zeroCountParts1;
-    drflac_uint32 zeroCountParts2;
-    drflac_uint32 zeroCountParts3;
-    drflac_uint32 riceParamParts0;
-    drflac_uint32 riceParamParts1;
-    drflac_uint32 riceParamParts2;
-    drflac_uint32 riceParamParts3;
+    drflac_uint32 zeroCountParts0 = 0;
+    drflac_uint32 zeroCountParts1 = 0;
+    drflac_uint32 zeroCountParts2 = 0;
+    drflac_uint32 zeroCountParts3 = 0;
+    drflac_uint32 riceParamParts0 = 0;
+    drflac_uint32 riceParamParts1 = 0;
+    drflac_uint32 riceParamParts2 = 0;
+    drflac_uint32 riceParamParts3 = 0;
     __m128i coefficients128_0;
     __m128i coefficients128_4;
     __m128i coefficients128_8;
     __m128i samples128_0;
     __m128i samples128_4;
     __m128i samples128_8;
     __m128i riceParamMask128;
@@ -3517,22 +3520,22 @@
 
 static drflac_bool32 drflac__decode_samples_with_residual__rice__sse41_64(drflac_bs* bs, drflac_uint32 count, drflac_uint8 riceParam, drflac_uint32 order, drflac_int32 shift, const drflac_int32* coefficients, drflac_int32* pSamplesOut)
 {
     int i;
     drflac_uint32 riceParamMask;
     drflac_int32* pDecodedSamples    = pSamplesOut;
     drflac_int32* pDecodedSamplesEnd = pSamplesOut + (count & ~3);
-    drflac_uint32 zeroCountParts0;
-    drflac_uint32 zeroCountParts1;
-    drflac_uint32 zeroCountParts2;
-    drflac_uint32 zeroCountParts3;
-    drflac_uint32 riceParamParts0;
-    drflac_uint32 riceParamParts1;
-    drflac_uint32 riceParamParts2;
-    drflac_uint32 riceParamParts3;
+    drflac_uint32 zeroCountParts0 = 0;
+    drflac_uint32 zeroCountParts1 = 0;
+    drflac_uint32 zeroCountParts2 = 0;
+    drflac_uint32 zeroCountParts3 = 0;
+    drflac_uint32 riceParamParts0 = 0;
+    drflac_uint32 riceParamParts1 = 0;
+    drflac_uint32 riceParamParts2 = 0;
+    drflac_uint32 riceParamParts3 = 0;
     __m128i coefficients128_0;
     __m128i coefficients128_4;
     __m128i coefficients128_8;
     __m128i samples128_0;
     __m128i samples128_4;
     __m128i samples128_8;
     __m128i prediction128;
@@ -5074,18 +5077,18 @@
     drflac_uint64 firstPCMFrame;
     drflac_uint64 lastPCMFrame;
 
     DRFLAC_ASSERT(pFlac != NULL);
 
     firstPCMFrame = pFlac->currentFLACFrame.header.pcmFrameNumber;
     if (firstPCMFrame == 0) {
-        firstPCMFrame = pFlac->currentFLACFrame.header.flacFrameNumber * pFlac->maxBlockSizeInPCMFrames;
+        firstPCMFrame = ((drflac_uint64)pFlac->currentFLACFrame.header.flacFrameNumber) * pFlac->maxBlockSizeInPCMFrames;
     }
 
-    lastPCMFrame = firstPCMFrame + (pFlac->currentFLACFrame.header.blockSizeInPCMFrames);
+    lastPCMFrame = firstPCMFrame + pFlac->currentFLACFrame.header.blockSizeInPCMFrames;
     if (lastPCMFrame > 0) {
         lastPCMFrame -= 1; /* Needs to be zero based. */
     }
 
     if (pFirstPCMFrame) {
         *pFirstPCMFrame = firstPCMFrame;
     }
@@ -5345,15 +5348,15 @@
     drflac_uint64 targetByte;
     drflac_uint64 pcmRangeLo = pFlac->totalPCMFrameCount;
     drflac_uint64 pcmRangeHi = 0;
     drflac_uint64 lastSuccessfulSeekOffset = (drflac_uint64)-1;
     drflac_uint64 closestSeekOffsetBeforeTargetPCMFrame = byteRangeLo;
     drflac_uint32 seekForwardThreshold = (pFlac->maxBlockSizeInPCMFrames != 0) ? pFlac->maxBlockSizeInPCMFrames*2 : 4096;
 
-    targetByte = byteRangeLo + (drflac_uint64)((pcmFrameIndex - pFlac->currentPCMFrame) * pFlac->channels * pFlac->bitsPerSample/8 * DRFLAC_BINARY_SEARCH_APPROX_COMPRESSION_RATIO);
+    targetByte = byteRangeLo + (drflac_uint64)(((pcmFrameIndex - pFlac->currentPCMFrame) * pFlac->channels * pFlac->bitsPerSample/8.0f) * DRFLAC_BINARY_SEARCH_APPROX_COMPRESSION_RATIO);
     if (targetByte > byteRangeHi) {
         targetByte = byteRangeHi;
     }
 
     for (;;) {
         if (drflac__seek_to_approximate_flac_frame_to_byte(pFlac, targetByte, byteRangeLo, byteRangeHi, &lastSuccessfulSeekOffset)) {
             /* We found a FLAC frame. We need to check if it contains the sample we're looking for. */
@@ -5390,15 +5393,14 @@
                 if (pcmRangeLo > pcmFrameIndex) {
                     /* We seeked too far forward. We need to move our target byte backward and try again. */
                     byteRangeHi = lastSuccessfulSeekOffset;
                     if (byteRangeLo > byteRangeHi) {
                         byteRangeLo = byteRangeHi;
                     }
 
-                    /*targetByte = lastSuccessfulSeekOffset - (drflac_uint64)((pcmRangeLo-pcmFrameIndex) * pFlac->channels * pFlac->bitsPerSample/8 * approxCompressionRatio);*/
                     targetByte = byteRangeLo + ((byteRangeHi - byteRangeLo) / 2);
                     if (targetByte < byteRangeLo) {
                         targetByte = byteRangeLo;
                     }
                 } else /*if (pcmRangeHi < pcmFrameIndex)*/ {
                     /* We didn't seek far enough. We need to move our target byte forward and try again. */
 
@@ -5411,18 +5413,15 @@
                         }
                     } else {
                         byteRangeLo = lastSuccessfulSeekOffset;
                         if (byteRangeHi < byteRangeLo) {
                             byteRangeHi = byteRangeLo;
                         }
 
-                        /*targetByte = byteRangeLo + (drflac_uint64)((pcmFrameIndex-pcmRangeLo) * pFlac->channels * pFlac->bitsPerSample/8 * approxCompressionRatio);*/
-                        targetByte = lastSuccessfulSeekOffset + (drflac_uint64)((pcmFrameIndex-pcmRangeLo) * pFlac->channels * pFlac->bitsPerSample/8 * approxCompressionRatio);
-                        /*targetByte = byteRangeLo + ((byteRangeHi - byteRangeLo) / 2);*/
-
+                        targetByte = lastSuccessfulSeekOffset + (drflac_uint64)(((pcmFrameIndex-pcmRangeLo) * pFlac->channels * pFlac->bitsPerSample/8.0f) * approxCompressionRatio);
                         if (targetByte > byteRangeHi) {
                             targetByte = byteRangeHi;
                         }
 
                         if (closestSeekOffsetBeforeTargetPCMFrame < lastSuccessfulSeekOffset) {
                             closestSeekOffsetBeforeTargetPCMFrame = lastSuccessfulSeekOffset;
                         }
@@ -5456,15 +5455,15 @@
     }
 
     /*
     Our starting byte range is the byte position of the first FLAC frame and the approximate end of the file as if it were completely uncompressed. This ensures
     the entire file is included, even though most of the time it'll exceed the end of the actual stream. This is OK as the frame searching logic will handle it.
     */
     byteRangeLo = pFlac->firstFLACFramePosInBytes;
-    byteRangeHi = pFlac->firstFLACFramePosInBytes + (drflac_uint64)(pFlac->totalPCMFrameCount * pFlac->channels * pFlac->bitsPerSample/8);
+    byteRangeHi = pFlac->firstFLACFramePosInBytes + (drflac_uint64)(pFlac->totalPCMFrameCount * pFlac->channels * pFlac->bitsPerSample/8.0f);
 
     return drflac__seek_to_pcm_frame__binary_search_internal(pFlac, pcmFrameIndex, byteRangeLo, byteRangeHi);
 }
 #endif  /* !DR_FLAC_NO_CRC */
 
 static drflac_bool32 drflac__seek_to_pcm_frame__seek_table(drflac* pFlac, drflac_uint64 pcmFrameIndex)
 {
@@ -5490,15 +5489,15 @@
 
 #if !defined(DR_FLAC_NO_CRC)
     /* At this point we should know the closest seek point. We can use a binary search for this. We need to know the total sample count for this. */
     if (pFlac->totalPCMFrameCount > 0) {
         drflac_uint64 byteRangeLo;
         drflac_uint64 byteRangeHi;
 
-        byteRangeHi = pFlac->firstFLACFramePosInBytes + (drflac_uint64)(pFlac->totalPCMFrameCount * pFlac->channels * pFlac->bitsPerSample/8);
+        byteRangeHi = pFlac->firstFLACFramePosInBytes + (drflac_uint64)(pFlac->totalPCMFrameCount * pFlac->channels * pFlac->bitsPerSample/8.0f);
         byteRangeLo = pFlac->firstFLACFramePosInBytes + pFlac->pSeekpoints[iClosestSeekpoint].flacFrameOffset;
 
         if (iClosestSeekpoint < pFlac->seekpointCount-1) {
             if (pFlac->pSeekpoints[iClosestSeekpoint+1].firstPCMFrame != (((drflac_uint64)0xFFFFFFFF << 32) | 0xFFFFFFFF)) {   /* Is it a placeholder seekpoint. */
                 byteRangeHi = pFlac->firstFLACFramePosInBytes + pFlac->pSeekpoints[iClosestSeekpoint+1].flacFrameOffset-1; /* Must be zero based. */
             }
         }
@@ -5667,14 +5666,16 @@
     *blockType   = (blockHeader & 0x7F000000UL) >> 24;
     *blockSize   = (blockHeader & 0x00FFFFFFUL);
 }
 
 static DRFLAC_INLINE drflac_bool32 drflac__read_and_decode_block_header(drflac_read_proc onRead, void* pUserData, drflac_uint8* isLastBlock, drflac_uint8* blockType, drflac_uint32* blockSize)
 {
     drflac_uint32 blockHeader;
+
+    *blockSize = 0;
     if (onRead(pUserData, &blockHeader, 4) != 4) {
         return DRFLAC_FALSE;
     }
 
     drflac__decode_block_header(blockHeader, isLastBlock, blockType, blockSize);
     return DRFLAC_TRUE;
 }
@@ -5776,16 +5777,18 @@
         void* p2;
 
         p2 = pAllocationCallbacks->onMalloc(szNew, pAllocationCallbacks->pUserData);
         if (p2 == NULL) {
             return NULL;
         }
 
-        DRFLAC_COPY_MEMORY(p2, p, szOld);
-        pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        if (p != NULL) {
+            DRFLAC_COPY_MEMORY(p2, p, szOld);
+            pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        }
 
         return p2;
     }
 
     return NULL;
 }
 
@@ -5812,15 +5815,15 @@
     drflac_uint32 seektableSize  = 0;
 
     for (;;) {
         drflac_metadata metadata;
         drflac_uint8 isLastBlock = 0;
         drflac_uint8 blockType;
         drflac_uint32 blockSize;
-        if (!drflac__read_and_decode_block_header(onRead, pUserData, &isLastBlock, &blockType, &blockSize)) {
+        if (drflac__read_and_decode_block_header(onRead, pUserData, &isLastBlock, &blockType, &blockSize) == DRFLAC_FALSE) {
             return DRFLAC_FALSE;
         }
         runningFilePos += 4;
 
         metadata.type = blockType;
         metadata.pRawData = NULL;
         metadata.rawDataSize = 0;
@@ -6380,14 +6383,24 @@
     DRFLAC_ASSERT(*pCRC32 == DRFLAC_OGG_CAPTURE_PATTERN_CRC32);
 
     if (onRead(pUserData, data, 23) != 23) {
         return DRFLAC_END_OF_STREAM;
     }
     *pBytesRead += 23;
 
+    /*
+    It's not actually used, but set the capture pattern to 'OggS' for completeness. Not doing this will cause static analysers to complain about
+    us trying to access uninitialized data. We could alternatively just comment out this member of the drflac_ogg_page_header structure, but I
+    like to have it map to the structure of the underlying data.
+    */
+    pHeader->capturePattern[0] = 'O';
+    pHeader->capturePattern[1] = 'g';
+    pHeader->capturePattern[2] = 'g';
+    pHeader->capturePattern[3] = 'S';
+
     pHeader->structureVersion = data[0];
     pHeader->headerType       = data[1];
     DRFLAC_COPY_MEMORY(&pHeader->granulePosition, &data[ 2], 8);
     DRFLAC_COPY_MEMORY(&pHeader->serialNumber,    &data[10], 4);
     DRFLAC_COPY_MEMORY(&pHeader->sequenceNumber,  &data[14], 4);
     DRFLAC_COPY_MEMORY(&pHeader->checksum,        &data[18], 4);
     pHeader->segmentCount     = data[22];
@@ -7148,15 +7161,15 @@
 #endif
     }
 
     /* Unsupported container. */
     return DRFLAC_FALSE;
 }
 
-void drflac__init_from_info(drflac* pFlac, drflac_init_info* pInit)
+void drflac__init_from_info(drflac* pFlac, const drflac_init_info* pInit)
 {
     DRFLAC_ASSERT(pFlac != NULL);
     DRFLAC_ASSERT(pInit != NULL);
 
     DRFLAC_ZERO_MEMORY(pFlac, sizeof(*pFlac));
     pFlac->bs                      = pInit->bs;
     pFlac->onMeta                  = pInit->onMeta;
@@ -7276,14 +7289,18 @@
         }
 
         allocationSize += seektableSize;
     }
 
 
     pFlac = (drflac*)drflac__malloc_from_callbacks(allocationSize, &allocationCallbacks);
+    if (pFlac == NULL) {
+        return NULL;
+    }
+
     drflac__init_from_info(pFlac, &init);
     pFlac->allocationCallbacks = allocationCallbacks;
     pFlac->pDecodedSamples = (drflac_int32*)drflac_align((size_t)pFlac->pExtraData, DRFLAC_MAX_SIMD_VECTOR_SIZE);
 
 #ifndef DR_FLAC_NO_OGG
     if (init.container == drflac_container_ogg) {
         drflac_oggbs* pInternalOggbs = (drflac_oggbs*)((drflac_uint8*)pFlac->pDecodedSamples + decodedSamplesAllocationSize + seektableSize);
@@ -7310,14 +7327,17 @@
 #endif
     {
         /* If we have a seektable we need to load it now, making sure we move back to where we were previously. */
         if (seektablePos != 0) {
             pFlac->seekpointCount = seektableSize / sizeof(*pFlac->pSeekpoints);
             pFlac->pSeekpoints = (drflac_seekpoint*)((drflac_uint8*)pFlac->pDecodedSamples + decodedSamplesAllocationSize);
 
+            DRFLAC_ASSERT(pFlac->bs.onSeek != NULL);
+            DRFLAC_ASSERT(pFlac->bs.onRead != NULL);
+
             /* Seek to the seektable, then just read directly into our seektable buffer. */
             if (pFlac->bs.onSeek(pFlac->bs.pUserData, (int)seektablePos, drflac_seek_origin_start)) {
                 if (pFlac->bs.onRead(pFlac->bs.pUserData, pFlac->pSeekpoints, seektableSize) == seektableSize) {
                     /* Endian swap. */
                     drflac_uint32 iSeekpoint;
                     for (iSeekpoint = 0; iSeekpoint < pFlac->seekpointCount; ++iSeekpoint) {
                         pFlac->pSeekpoints[iSeekpoint].firstPCMFrame   = drflac__be2host_64(pFlac->pSeekpoints[iSeekpoint].firstPCMFrame);
@@ -10713,14 +10733,22 @@
 #endif
 #endif  /* DR_FLAC_IMPLEMENTATION */
 
 
 /*
 REVISION HISTORY
 ================
+v0.12.3 - 2019-12-02
+  - Fix some warnings when compiling with GCC and the -Og flag.
+  - Fix a crash in out-of-memory situations.
+  - Fix potential integer overflow bug.
+  - Fix some static analysis warnings.
+  - Fix a possible crash when using custom memory allocators without a custom realloc() implementation.
+  - Fix a bug with binary search seeking where the bits per sample is not a multiple of 8.
+
 v0.12.2 - 2019-10-07
   - Internal code clean up.
 
 v0.12.1 - 2019-09-29
   - Fix some Clang Static Analyzer warnings.
   - Fix an unused variable warning.
```

### Comparing `miniaudio-1.8/miniaudio/dr_mp3.h` & `miniaudio-1.9/miniaudio/dr_mp3.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 MP3 audio decoder. Choice of public domain or MIT-0. See license statements at the end of this file.
-dr_mp3 - v0.5.0 - 2019-10-07
+dr_mp3 - v0.5.4 - 2019-12-02
 
 David Reid - mackron@gmail.com
 
 Based off minimp3 (https://github.com/lieff/minimp3) which is where the real work was done. See the bottom of this file for
 differences between minimp3 and dr_mp3.
 */
 
@@ -37,19 +37,19 @@
     ...
 
     drmp3_allocation_callbacks allocationCallbacks;
     allocationCallbacks.pUserData = &myData;
     allocationCallbacks.onMalloc  = my_malloc;
     allocationCallbacks.onRealloc = my_realloc;
     allocationCallbacks.onFree    = my_free;
-    drmp3_init_file(&mp3, "my_file.wav", NULL, &allocationCallbacks);
+    drmp3_init_file(&mp3, "my_file.mp3", NULL, &allocationCallbacks);
 
 The advantage of this new system is that it allows you to specify user data which will be passed in to the allocation routines.
 
-Passing in null for the allocation callbacks object will cause dr_wav to use defaults which is the same as DRMP3_MALLOC,
+Passing in null for the allocation callbacks object will cause dr_mp3 to use defaults which is the same as DRMP3_MALLOC,
 DRMP3_REALLOC and DRMP3_FREE and the equivalent of how it worked in previous versions.
 
 Every API that opens a drmp3 object now takes this extra parameter. These include the following:
 
     drmp3_init()
     drmp3_init_file()
     drmp3_init_memory()
@@ -615,14 +615,15 @@
 
 end:
     return g_have_simd - 1;
 #endif
 }
 #elif defined(__ARM_NEON) || defined(__aarch64__)
 #include <arm_neon.h>
+#define DRMP3_HAVE_SSE 0
 #define DRMP3_HAVE_SIMD 1
 #define DRMP3_VSTORE vst1q_f32
 #define DRMP3_VLD vld1q_f32
 #define DRMP3_VSET vmovq_n_f32
 #define DRMP3_VADD vaddq_f32
 #define DRMP3_VSUB vsubq_f32
 #define DRMP3_VMUL vmulq_f32
@@ -632,14 +633,15 @@
 #define DRMP3_VREV(x) vcombine_f32(vget_high_f32(vrev64q_f32(x)), vget_low_f32(vrev64q_f32(x)))
 typedef float32x4_t drmp3_f4;
 static int drmp3_have_simd()
 {   /* TODO: detect neon for !DR_MP3_ONLY_SIMD */
     return 1;
 }
 #else
+#define DRMP3_HAVE_SSE 0
 #define DRMP3_HAVE_SIMD 0
 #ifdef DR_MP3_ONLY_SIMD
 #error DR_MP3_ONLY_SIMD used, but SSE/NEON not enabled
 #endif
 #endif
 
 #else
@@ -2378,14 +2380,15 @@
 static void drmp3__free_default(void* p, void* pUserData)
 {
     (void)pUserData;
     DRMP3_FREE(p);
 }
 
 
+#if 0   /* Unused, but leaving here in case I need to add it again later. */
 static void* drmp3__malloc_from_callbacks(size_t sz, const drmp3_allocation_callbacks* pAllocationCallbacks)
 {
     if (pAllocationCallbacks == NULL) {
         return NULL;
     }
 
     if (pAllocationCallbacks->onMalloc != NULL) {
@@ -2395,14 +2398,15 @@
     /* Try using realloc(). */
     if (pAllocationCallbacks->onRealloc != NULL) {
         return pAllocationCallbacks->onRealloc(NULL, sz, pAllocationCallbacks->pUserData);
     }
 
     return NULL;
 }
+#endif
 
 static void* drmp3__realloc_from_callbacks(void* p, size_t szNew, size_t szOld, const drmp3_allocation_callbacks* pAllocationCallbacks)
 {
     if (pAllocationCallbacks == NULL) {
         return NULL;
     }
 
@@ -2415,16 +2419,18 @@
         void* p2;
 
         p2 = pAllocationCallbacks->onMalloc(szNew, pAllocationCallbacks->pUserData);
         if (p2 == NULL) {
             return NULL;
         }
 
-        DRMP3_COPY_MEMORY(p2, p, szOld);
-        pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        if (p != NULL) {
+            DRMP3_COPY_MEMORY(p2, p, szOld);
+            pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        }
 
         return p2;
     }
 
     return NULL;
 }
 
@@ -3999,14 +4005,26 @@
   as a single translation unit (aka unity builds). At the time of writing this, a unity build is not possible when
   using minimp3 in conjunction with stb_vorbis. dr_mp3 addresses this.
 */
 
 /*
 REVISION HISTORY
 ================
+v0.5.4 - 2019-12-02
+  - Fix a possible null pointer dereference when using custom memory allocators for realloc().
+
+v0.5.3 - 2019-11-14
+  - Fix typos in documentation.
+
+v0.5.2 - 2019-11-02
+  - Bring up to date with minimp3.
+
+v0.5.1 - 2019-10-08
+  - Fix a warning with GCC.
+
 v0.5.0 - 2019-10-07
   - API CHANGE: Add support for user defined memory allocation routines. This system allows the program to specify their own memory allocation
     routines with a user data pointer for client-specific contextual data. This adds an extra parameter to the end of the following APIs:
     - drmp3_init()
     - drmp3_init_file()
     - drmp3_init_memory()
     - drmp3_open_and_read_pcm_frames_f32()
```

### Comparing `miniaudio-1.8/miniaudio/dr_wav.h` & `miniaudio-1.9/miniaudio/dr_wav.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 WAV audio loader and writer. Choice of public domain or MIT-0. See license statements at the end of this file.
-dr_wav - v0.11.1 - 2019-10-07
+dr_wav - v0.11.2 - 2019-12-02
 
 David Reid - mackron@gmail.com
 */
 
 /*
 RELEASE NOTES - v0.11.0
 =======================
@@ -1072,14 +1072,28 @@
         #define DRWAV_HAS_BYTESWAP64_INTRINSIC
     #endif
     #if ((__GNUC__ > 4) || (__GNUC__ == 4 && __GNUC_MINOR__ >= 8))
         #define DRWAV_HAS_BYTESWAP16_INTRINSIC
     #endif
 #endif
 
+/*
+These limits are used for basic validation when initializing the decoder. If you exceed these limits, first of all: what on Earth are
+you doing?! (Let me know, I'd be curious!) Second, you can adjust these by #define-ing them before the dr_wav implementation.
+*/
+#ifndef DRWAV_MAX_SAMPLE_RATE
+#define DRWAV_MAX_SAMPLE_RATE       384000
+#endif
+#ifndef DRWAV_MAX_CHANNELS
+#define DRWAV_MAX_CHANNELS          256
+#endif
+#ifndef DRWAV_MAX_BITS_PER_SAMPLE
+#define DRWAV_MAX_BITS_PER_SAMPLE   64
+#endif
+
 static const drwav_uint8 drwavGUID_W64_RIFF[16] = {0x72,0x69,0x66,0x66, 0x2E,0x91, 0xCF,0x11, 0xA5,0xD6, 0x28,0xDB,0x04,0xC1,0x00,0x00};    /* 66666972-912E-11CF-A5D6-28DB04C10000 */
 static const drwav_uint8 drwavGUID_W64_WAVE[16] = {0x77,0x61,0x76,0x65, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 65766177-ACF3-11D3-8CD1-00C04F8EDB8A */
 static const drwav_uint8 drwavGUID_W64_JUNK[16] = {0x6A,0x75,0x6E,0x6B, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 6B6E756A-ACF3-11D3-8CD1-00C04F8EDB8A */
 static const drwav_uint8 drwavGUID_W64_FMT [16] = {0x66,0x6D,0x74,0x20, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 20746D66-ACF3-11D3-8CD1-00C04F8EDB8A */
 static const drwav_uint8 drwavGUID_W64_FACT[16] = {0x66,0x61,0x63,0x74, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 74636166-ACF3-11D3-8CD1-00C04F8EDB8A */
 static const drwav_uint8 drwavGUID_W64_DATA[16] = {0x64,0x61,0x74,0x61, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 61746164-ACF3-11D3-8CD1-00C04F8EDB8A */
 static const drwav_uint8 drwavGUID_W64_SMPL[16] = {0x73,0x6D,0x70,0x6C, 0xF3,0xAC, 0xD3,0x11, 0x8C,0xD1, 0x00,0xC0,0x4F,0x8E,0xDB,0x8A};    /* 6C706D73-ACF3-11D3-8CD1-00C04F8EDB8A */
@@ -1442,16 +1456,18 @@
         void* p2;
 
         p2 = pAllocationCallbacks->onMalloc(szNew, pAllocationCallbacks->pUserData);
         if (p2 == NULL) {
             return NULL;
         }
 
-        DRWAV_COPY_MEMORY(p2, p, szOld);
-        pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        if (p != NULL) {
+            DRWAV_COPY_MEMORY(p2, p, szOld);
+            pAllocationCallbacks->onFree(p, pAllocationCallbacks->pUserData);
+        }
 
         return p2;
     }
 
     return NULL;
 }
 
@@ -1858,16 +1874,19 @@
 
     /* The next bytes should be the "fmt " chunk. */
     if (!drwav__read_fmt(pWav->onRead, pWav->onSeek, pWav->pUserData, pWav->container, &cursor, &fmt)) {
         return DRWAV_FALSE;    /* Failed to read the "fmt " chunk. */
     }
 
     /* Basic validation. */
-    if (fmt.sampleRate == 0 || fmt.channels == 0 || fmt.bitsPerSample == 0 || fmt.blockAlign == 0) {
-        return DRWAV_FALSE; /* Invalid channel count. Probably an invalid WAV file. */
+    if ((fmt.sampleRate    == 0 || fmt.sampleRate    > DRWAV_MAX_SAMPLE_RATE)     ||
+        (fmt.channels      == 0 || fmt.channels      > DRWAV_MAX_CHANNELS)        ||
+        (fmt.bitsPerSample == 0 || fmt.bitsPerSample > DRWAV_MAX_BITS_PER_SAMPLE) ||
+        fmt.blockAlign == 0) {
+        return DRWAV_FALSE; /* Probably an invalid WAV file. */
     }
 
 
     /* Translate the internal format. */
     translatedFormatTag = fmt.formatTag;
     if (translatedFormatTag == DR_WAVE_FORMAT_EXTENSIBLE) {
         translatedFormatTag = drwav__bytes_to_u16(fmt.subFormat + 0);
@@ -2922,19 +2941,20 @@
     return DRWAV_TRUE;
 }
 
 drwav_bool32 drwav_seek_to_pcm_frame(drwav* pWav, drwav_uint64 targetFrameIndex)
 {
     /* Seeking should be compatible with wave files > 2GB. */
 
-    if (pWav->onWrite != NULL) {
-        return DRWAV_FALSE; /* No seeking in write mode. */
+    if (pWav == NULL || pWav->onSeek == NULL) {
+        return DRWAV_FALSE;
     }
 
-    if (pWav == NULL || pWav->onSeek == NULL) {
+    /* No seeking in write mode. */
+    if (pWav->onWrite != NULL) {
         return DRWAV_FALSE;
     }
 
     /* If there are no samples, just return DRWAV_TRUE without doing anything. */
     if (pWav->totalPCMFrameCount == 0) {
         return DRWAV_TRUE;
     }
@@ -3056,18 +3076,18 @@
     }
 
     bytesWritten = 0;
     pRunningData = (const drwav_uint8*)pData;
 
     while (bytesToWrite > 0) {
         size_t bytesJustWritten;
-        drwav_uint64 bytesToWriteThisIteration = bytesToWrite;
-        if (bytesToWriteThisIteration > DRWAV_SIZE_MAX) {
-            bytesToWriteThisIteration = DRWAV_SIZE_MAX;
-        }
+        drwav_uint64 bytesToWriteThisIteration;
+
+        bytesToWriteThisIteration = bytesToWrite;
+        DRWAV_ASSERT(bytesToWriteThisIteration <= DRWAV_SIZE_MAX);  /* <-- This is checked above. */
 
         bytesJustWritten = drwav_write_raw(pWav, (size_t)bytesToWriteThisIteration, pRunningData);
         if (bytesJustWritten == 0) {
             break;
         }
 
         bytesToWrite -= bytesJustWritten;
@@ -3102,26 +3122,24 @@
     while (bytesToWrite > 0) {
         drwav_uint8 temp[4096];
         drwav_uint32 sampleCount;
         size_t bytesJustWritten;
         drwav_uint64 bytesToWriteThisIteration;
 
         bytesToWriteThisIteration = bytesToWrite;
-        if (bytesToWriteThisIteration > DRWAV_SIZE_MAX) {
-            bytesToWriteThisIteration = DRWAV_SIZE_MAX;
-        }
+        DRWAV_ASSERT(bytesToWriteThisIteration <= DRWAV_SIZE_MAX);  /* <-- This is checked above. */
 
         /*
         WAV files are always little-endian. We need to byte swap on big-endian architectures. Since our input buffer is read-only we need
         to use an intermediary buffer for the conversion.
         */
         sampleCount = sizeof(temp)/bytesPerSample;
 
-        if (bytesToWriteThisIteration > sampleCount*bytesPerSample) {
-            bytesToWriteThisIteration = sampleCount*bytesPerSample;
+        if (bytesToWriteThisIteration > ((drwav_uint64)sampleCount)*bytesPerSample) {
+            bytesToWriteThisIteration = ((drwav_uint64)sampleCount)*bytesPerSample;
         }
 
         DRWAV_COPY_MEMORY(temp, pRunningData, (size_t)bytesToWriteThisIteration);
         drwav__bswap_samples(temp, sampleCount, bytesPerSample, pWav->translatedFormatTag);
 
         bytesJustWritten = drwav_write_raw(pWav, (size_t)bytesToWriteThisIteration, temp);
         if (bytesJustWritten == 0) {
@@ -5029,14 +5047,20 @@
 }
 
 #endif  /* DR_WAV_IMPLEMENTATION */
 
 /*
 REVISION HISTORY
 ================
+v0.11.2 - 2019-12-02
+  - Fix a possible crash when using custom memory allocators without a custom realloc() implementation.
+  - Fix an integer overflow bug.
+  - Fix a null pointer dereference bug.
+  - Add limits to sample rate, channels and bits per sample to tighten up some validation.
+
 v0.11.1 - 2019-10-07
   - Internal code clean up.
 
 v0.11.0 - 2019-10-06
   - API CHANGE: Add support for user defined memory allocation routines. This system allows the program to specify their own memory allocation
     routines with a user data pointer for client-specific contextual data. This adds an extra parameter to the end of the following APIs:
     - drwav_init()
```

### Comparing `miniaudio-1.8/miniaudio/miniaudio.h` & `miniaudio-1.9/miniaudio/miniaudio.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 Audio playback and capture library. Choice of public domain or MIT-0. See license statements at the end of this file.
-miniaudio (formerly mini_al) - v0.9.8 - 2019-10-07
+miniaudio (formerly mini_al) - v0.9.9 - 2020-01-09
 
 David Reid - davidreidsoftware@gmail.com
 
 https://github.com/dr-soft/miniaudio
 */
 
 /*
@@ -257,30 +257,30 @@
 The Emscripten build emits Web Audio JavaScript directly and should Just Work without any configuration.
 
 
 NOTES
 =====
 - This library uses an asynchronous API for delivering and requesting audio data. Each device will have
   it's own worker thread which is managed by the library.
-- If ma_device_init() is called with a device that's not aligned to the 4 bytes on 32-bit or 8 bytes on
-  64-bit it will _not_ be thread-safe. The reason for this is that it depends on members of ma_device being
-  correctly aligned for atomic assignments.
 - Sample data is always native-endian and interleaved. For example, ma_format_s16 means signed 16-bit
-  integer samples, interleaved. Let me know if you need non-interleaved and I'll look into it.
-- The sndio backend is currently only enabled on OpenBSD builds.
-- The audio(4) backend is supported on OpenBSD, but you may need to disable sndiod before you can use it.
+  integer samples, interleaved.
 - Automatic stream routing is enabled on a per-backend basis. Support is explicitly enabled for WASAPI
   and Core Audio, however other backends such as PulseAudio may naturally support it, though not all have
   been tested.
 - The contents of the output buffer passed into the data callback will always be pre-initialized to zero
   unless the noPreZeroedOutputBuffer config variable in ma_device_config is set to true, in which case
   it'll be undefined which will require you to write something to the entire buffer.
 - By default miniaudio will automatically clip samples. This only applies when the playback sample format
   is configured as ma_format_f32. If you are doing clipping yourself, you can disable this overhead by
   setting noClip to true in the device config.
+- If ma_device_init() is called with a device that's not aligned to the 4 bytes on 32-bit or 8 bytes on
+  64-bit it will _not_ be thread-safe. The reason for this is that it depends on members of ma_device being
+  correctly aligned for atomic assignments.
+- The sndio backend is currently only enabled on OpenBSD builds.
+- The audio(4) backend is supported on OpenBSD, but you may need to disable sndiod before you can use it.
 
 
 BACKEND NUANCES
 ===============
 
 WASAPI
 ------
@@ -488,14 +488,15 @@
         #define MA_WIN32_UWP
     #else
         #define MA_WIN32_DESKTOP
     #endif
 #else
     #define MA_POSIX
     #include <pthread.h>    /* Unfortunate #include, but needed for pthread_t, pthread_mutex_t and pthread_cond_t types. */
+    #include <semaphore.h>
 
     #ifdef __unix__
         #define MA_UNIX
         #if defined(__DragonFly__) || defined(__FreeBSD__) || defined(__NetBSD__) || defined(__OpenBSD__)
             #define MA_BSD
         #endif
     #endif
@@ -740,15 +741,16 @@
 #define MA_FAILED_TO_SEND_DATA_TO_DEVICE               -306
 #define MA_FAILED_TO_OPEN_BACKEND_DEVICE               -307
 #define MA_FAILED_TO_START_BACKEND_DEVICE              -308
 #define MA_FAILED_TO_STOP_BACKEND_DEVICE               -309
 #define MA_FAILED_TO_CONFIGURE_BACKEND_DEVICE          -310
 #define MA_FAILED_TO_CREATE_MUTEX                      -311
 #define MA_FAILED_TO_CREATE_EVENT                      -312
-#define MA_FAILED_TO_CREATE_THREAD                     -313
+#define MA_FAILED_TO_CREATE_SEMAPHORE                  -313
+#define MA_FAILED_TO_CREATE_THREAD                     -314
 
 
 /* Standard sample rates. */
 #define MA_SAMPLE_RATE_8000                            8000
 #define MA_SAMPLE_RATE_11025                           11025
 #define MA_SAMPLE_RATE_16000                           16000
 #define MA_SAMPLE_RATE_22050                           22050
@@ -1794,14 +1796,36 @@
             ma_uint32 value;
         } posix;
 #endif
         int _unused;
     };
 } ma_event;
 
+typedef struct
+{
+    ma_context* pContext;
+
+    union
+    {
+#ifdef MA_WIN32
+        struct
+        {
+            /*HANDLE*/ ma_handle hSemaphore;
+        } win32;
+#endif
+#ifdef MA_POSIX
+        struct
+        {
+            sem_t semaphore;
+        } posix;
+#endif
+        int _unused;
+    };
+} ma_semaphore;
+
 
 /*
 The callback for processing audio data from the device.
 
 pOutput is a pointer to a buffer that will receive audio data that will later be played back through the speakers. This will be non-null
 for a playback or full-duplex device and null for a capture device.
 
@@ -1852,14 +1876,39 @@
 
 typedef enum
 {
     ma_share_mode_shared = 0,
     ma_share_mode_exclusive
 } ma_share_mode;
 
+/* iOS/tvOS/watchOS session categories. */
+typedef enum
+{
+    ma_ios_session_category_default = 0,        /* AVAudioSessionCategoryPlayAndRecord with AVAudioSessionCategoryOptionDefaultToSpeaker. */
+    ma_ios_session_category_none,               /* Leave the session category unchanged. */
+    ma_ios_session_category_ambient,            /* AVAudioSessionCategoryAmbient */
+    ma_ios_session_category_solo_ambient,       /* AVAudioSessionCategorySoloAmbient */
+    ma_ios_session_category_playback,           /* AVAudioSessionCategoryPlayback */
+    ma_ios_session_category_record,             /* AVAudioSessionCategoryRecord */
+    ma_ios_session_category_play_and_record,    /* AVAudioSessionCategoryPlayAndRecord */
+    ma_ios_session_category_multi_route         /* AVAudioSessionCategoryMultiRoute */
+} ma_ios_session_category;
+
+/* iOS/tvOS/watchOS session category options */
+typedef enum
+{
+    ma_ios_session_category_option_mix_with_others                            = 0x01,   /* AVAudioSessionCategoryOptionMixWithOthers */
+    ma_ios_session_category_option_duck_others                                = 0x02,   /* AVAudioSessionCategoryOptionDuckOthers */
+    ma_ios_session_category_option_allow_bluetooth                            = 0x04,   /* AVAudioSessionCategoryOptionAllowBluetooth */
+    ma_ios_session_category_option_default_to_speaker                         = 0x08,   /* AVAudioSessionCategoryOptionDefaultToSpeaker */
+    ma_ios_session_category_option_interrupt_spoken_audio_and_mix_with_others = 0x11,   /* AVAudioSessionCategoryOptionInterruptSpokenAudioAndMixWithOthers */
+    ma_ios_session_category_option_allow_bluetooth_a2dp                       = 0x20,   /* AVAudioSessionCategoryOptionAllowBluetoothA2DP */
+    ma_ios_session_category_option_allow_air_play                             = 0x40,   /* AVAudioSessionCategoryOptionAllowAirPlay */
+} ma_ios_session_category_option;
+
 typedef union
 {
 #ifdef MA_SUPPORT_WASAPI
     wchar_t wasapi[64];             /* WASAPI uses a wchar_t string for identification. */
 #endif
 #ifdef MA_SUPPORT_DSOUND
     ma_uint8 dsound[16];            /* DirectSound uses a GUID for identification. */
@@ -1960,14 +2009,16 @@
         ma_share_mode shareMode;
     } capture;
 
     struct
     {
         ma_bool32 noAutoConvertSRC;     /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_AUTOCONVERTPCM. */
         ma_bool32 noDefaultQualitySRC;  /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_SRC_DEFAULT_QUALITY. */
+        ma_bool32 noAutoStreamRouting;  /* Disables automatic stream routing. */
+        ma_bool32 noHardwareOffloading; /* Disables WASAPI's hardware offloading feature. */
     } wasapi;
     struct
     {
         ma_bool32 noMMap;  /* Disables MMap mode. */
     } alsa;
     struct
     {
@@ -1990,14 +2041,19 @@
     {
         const char* pApplicationName;
         const char* pServerName;
         ma_bool32 tryAutoSpawn; /* Enables autospawning of the PulseAudio daemon if necessary. */
     } pulse;
     struct
     {
+        ma_ios_session_category sessionCategory;
+        ma_uint32 sessionCategoryOptions;
+    } coreaudio;
+    struct
+    {
         const char* pClientName;
         ma_bool32 tryStartServer;
     } jack;
 } ma_context_config;
 
 typedef ma_bool32 (* ma_enum_devices_callback_proc)(ma_context* pContext, ma_device_type deviceType, const ma_device_info* pInfo, void* pUserData);
 
@@ -2286,14 +2342,15 @@
             ma_proc AAudioStreamBuilder_setSharingMode;
             ma_proc AAudioStreamBuilder_setFormat;
             ma_proc AAudioStreamBuilder_setChannelCount;
             ma_proc AAudioStreamBuilder_setSampleRate;
             ma_proc AAudioStreamBuilder_setBufferCapacityInFrames;
             ma_proc AAudioStreamBuilder_setFramesPerDataCallback;
             ma_proc AAudioStreamBuilder_setDataCallback;
+            ma_proc AAudioStreamBuilder_setErrorCallback;
             ma_proc AAudioStreamBuilder_setPerformanceMode;
             ma_proc AAudioStreamBuilder_openStream;
             ma_proc AAudioStream_close;
             ma_proc AAudioStream_getState;
             ma_proc AAudioStream_waitForStateChange;
             ma_proc AAudioStream_getFormat;
             ma_proc AAudioStream_getChannelCount;
@@ -2458,14 +2515,15 @@
             ma_bool32 hasDefaultCaptureDeviceChanged;          /* <-- Make sure this is always a whole 32-bits because we use atomic assignments. */
             ma_uint32 periodSizeInFramesPlayback;
             ma_uint32 periodSizeInFramesCapture;
             ma_bool32 isStartedCapture;
             ma_bool32 isStartedPlayback;
             ma_bool32 noAutoConvertSRC;     /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_AUTOCONVERTPCM. */
             ma_bool32 noDefaultQualitySRC;  /* When set to true, disables the use of AUDCLNT_STREAMFLAGS_SRC_DEFAULT_QUALITY. */
+            ma_bool32 noHardwareOffloading;
         } wasapi;
 #endif
 #ifdef MA_SUPPORT_DSOUND
         struct
         {
             /*LPDIRECTSOUND*/ ma_ptr pPlayback;
             /*LPDIRECTSOUNDBUFFER*/ ma_ptr pPlaybackPrimaryBuffer;
@@ -2545,14 +2603,15 @@
             ma_uint32 originalBufferSizeInMilliseconds;
             ma_uint32 originalPeriods;
             ma_bool32 isDefaultPlaybackDevice;
             ma_bool32 isDefaultCaptureDevice;
             ma_bool32 isSwitchingPlaybackDevice;   /* <-- Set to true when the default device has changed and miniaudio is in the process of switching. */
             ma_bool32 isSwitchingCaptureDevice;    /* <-- Set to true when the default device has changed and miniaudio is in the process of switching. */
             ma_pcm_rb duplexRB;
+            void* pRouteChangeHandler;             /* Only used on mobile platforms. Obj-C object for handling route changes. */
         } coreaudio;
 #endif
 #ifdef MA_SUPPORT_SNDIO
         struct
         {
             ma_ptr handlePlayback;
             ma_ptr handleCapture;
@@ -3152,14 +3211,18 @@
 
 
 
 
 /************************************************************************************************************************************************************
 
 Decoding
+========
+
+Decoders are independent of the main device API. Decoding APIs can be called freely inside the device's data callback, but they are not thread safe unless
+you do your own synchronization.
 
 ************************************************************************************************************************************************************/
 #ifndef MA_NO_DECODING
 
 typedef struct ma_decoder ma_decoder;
 
 typedef enum
@@ -3254,19 +3317,32 @@
 Do not call this on streams of an undefined length, such as internet radio.
 
 If the length is unknown or an error occurs, 0 will be returned.
 
 This will always return 0 for Vorbis decoders. This is due to a limitation with stb_vorbis in push mode which is what miniaudio
 uses internally.
 
-This will run in linear time for MP3 decoders. Do not call this in time critical scenarios.
+For MP3's, this will decode the entire file. Do not call this in time critical scenarios.
+
+This function is not thread safe without your own synchronization.
 */
 ma_uint64 ma_decoder_get_length_in_pcm_frames(ma_decoder* pDecoder);
 
+/*
+Reads PCM frames from the given decoder.
+
+This is not thread safe without your own synchronization.
+*/
 ma_uint64 ma_decoder_read_pcm_frames(ma_decoder* pDecoder, void* pFramesOut, ma_uint64 frameCount);
+
+/*
+Seeks to a PCM frame based on it's absolute index.
+
+This is not thread safe without your own synchronization.
+*/
 ma_result ma_decoder_seek_to_pcm_frame(ma_decoder* pDecoder, ma_uint64 frameIndex);
 
 /*
 Helper for opening and decoding a file into a heap allocated block of memory. Free the returned pointer with ma_free(). On input,
 pConfig should be set to what you want. On output it will be set to what you got.
 */
 #ifndef MA_NO_STDIO
@@ -3309,16 +3385,19 @@
 *************************************************************************************************************************************************************
 ************************************************************************************************************************************************************/
 #if defined(MINIAUDIO_IMPLEMENTATION) || defined(MA_IMPLEMENTATION)
 #include <assert.h>
 #include <limits.h> /* For INT_MAX */
 #include <math.h>   /* sin(), etc. */
 
-#if defined(MA_DEBUG_OUTPUT)
-#include <stdio.h>  /* for printf() for debug output */
+#if !defined(MA_NO_STDIO) || defined(MA_DEBUG_OUTPUT)
+#include <stdio.h>
+#if !defined(_MSC_VER) && !defined(__DMC__)
+#include <strings.h>    /* For strcasecmp(). */
+#include <wchar.h>      /* For wcslen(), wcsrtombs() */
 #endif
 
 #ifdef MA_WIN32
 #include <windows.h>
 #include <objbase.h>
 #include <mmreg.h>
 #include <mmsystem.h>
@@ -3690,15 +3769,15 @@
 static MA_INLINE ma_bool32 ma_is_big_endian()
 {
     return !ma_is_little_endian();
 }
 
 
 #ifndef MA_COINIT_VALUE
-#define MA_COINIT_VALUE    0   /* 0 = COINIT_MULTITHREADED*/
+#define MA_COINIT_VALUE    0   /* 0 = COINIT_MULTITHREADED */
 #endif
 
 
 
 #ifndef MA_PI
 #define MA_PI      3.14159265358979323846264f
 #endif
@@ -3829,19 +3908,21 @@
 #ifdef MA_WIN32
 #define MA_ASSERT(condition) assert(condition)
 #else
 #define MA_ASSERT(condition) assert(condition)
 #endif
 #endif
 
+#define MA_ZERO_OBJECT(p) MA_ZERO_MEMORY((p), sizeof(*(p)))
+
 #define ma_zero_memory MA_ZERO_MEMORY
+#define ma_zero_object MA_ZERO_OBJECT
 #define ma_copy_memory MA_COPY_MEMORY
 #define ma_assert      MA_ASSERT
 
-#define ma_zero_object(p)          ma_zero_memory((p), sizeof(*(p)))
 #define ma_countof(x)              (sizeof(x) / sizeof(x[0]))
 #define ma_max(x, y)               (((x) > (y)) ? (x) : (y))
 #define ma_min(x, y)               (((x) < (y)) ? (x) : (y))
 #define ma_clamp(x, lo, hi)        (ma_max(lo, ma_min(x, hi)))
 #define ma_offset_ptr(p, offset)   (((ma_uint8*)(p)) + (offset))
 
 #define ma_buffer_frame_capacity(buffer, channels, format) (sizeof(buffer) / ma_get_bytes_per_sample(format) / (channels))
@@ -4986,14 +5067,42 @@
     return WaitForSingleObject(pEvent->win32.hEvent, INFINITE) == WAIT_OBJECT_0;
 }
 
 ma_bool32 ma_event_signal__win32(ma_event* pEvent)
 {
     return SetEvent(pEvent->win32.hEvent);
 }
+
+
+ma_result ma_semaphore_init__win32(ma_context* pContext, int initialValue, ma_semaphore* pSemaphore)
+{
+    (void)pContext;
+
+    pSemaphore->win32.hSemaphore = CreateSemaphoreA(NULL, (LONG)initialValue, LONG_MAX, NULL);
+    if (pSemaphore->win32.hSemaphore == NULL) {
+        return MA_FAILED_TO_CREATE_SEMAPHORE;
+    }
+
+    return MA_SUCCESS;
+}
+
+void ma_semaphore_uninit__win32(ma_semaphore* pSemaphore)
+{
+    CloseHandle((HANDLE)pSemaphore->win32.hSemaphore);
+}
+
+ma_bool32 ma_semaphore_wait__win32(ma_semaphore* pSemaphore)
+{
+    return WaitForSingleObject((HANDLE)pSemaphore->win32.hSemaphore, INFINITE) == WAIT_OBJECT_0;
+}
+
+ma_bool32 ma_semaphore_release__win32(ma_semaphore* pSemaphore)
+{
+    return ReleaseSemaphore((HANDLE)pSemaphore->win32.hSemaphore, 1, NULL) != 0;
+}
 #endif
 
 
 #ifdef MA_POSIX
 #include <sched.h>
 
 typedef int (* ma_pthread_create_proc)(pthread_t *thread, const pthread_attr_t *attr, void *(*start_routine) (void *), void *arg);
@@ -5172,14 +5281,46 @@
         pEvent->posix.value = 1;
         ((ma_pthread_cond_signal_proc)pEvent->pContext->posix.pthread_cond_signal)(&pEvent->posix.condition);
     }
     ((ma_pthread_mutex_unlock_proc)pEvent->pContext->posix.pthread_mutex_unlock)(&pEvent->posix.mutex);
 
     return MA_TRUE;
 }
+
+
+ma_result ma_semaphore_init__posix(ma_context* pContext, int initialValue, ma_semaphore* pSemaphore)
+{
+    (void)pContext;
+
+#if defined(MA_APPLE)
+    /* Not yet implemented for Apple platforms since sem_init() is deprecated. Need to use a named semaphore via sem_open() instead. */
+    return MA_INVALID_OPERATION;
+#else
+    if (sem_init(&pSemaphore->posix.semaphore, 0, (unsigned int)initialValue) == 0) {
+        return MA_FAILED_TO_CREATE_SEMAPHORE;
+    }
+#endif
+
+    return MA_SUCCESS;
+}
+
+void ma_semaphore_uninit__posix(ma_semaphore* pSemaphore)
+{
+    sem_close(&pSemaphore->posix.semaphore);
+}
+
+ma_bool32 ma_semaphore_wait__posix(ma_semaphore* pSemaphore)
+{
+    return sem_wait(&pSemaphore->posix.semaphore) != -1;
+}
+
+ma_bool32 ma_semaphore_release__posix(ma_semaphore* pSemaphore)
+{
+    return sem_post(&pSemaphore->posix.semaphore) != -1;
+}
 #endif
 
 ma_result ma_thread_create(ma_context* pContext, ma_thread* pThread, ma_thread_entry_proc entryProc, void* pData)
 {
     if (pContext == NULL || pThread == NULL || entryProc == NULL) {
         return MA_FALSE;
     }
@@ -5333,14 +5474,71 @@
 #endif
 #ifdef MA_POSIX
     return ma_event_signal__posix(pEvent);
 #endif
 }
 
 
+ma_result ma_semaphore_init(ma_context* pContext, int initialValue, ma_semaphore* pSemaphore)
+{
+    if (pContext == NULL || pSemaphore == NULL) {
+        return MA_INVALID_ARGS;
+    }
+
+#ifdef MA_WIN32
+    return ma_semaphore_init__win32(pContext, initialValue, pSemaphore);
+#endif
+#ifdef MA_POSIX
+    return ma_semaphore_init__posix(pContext, initialValue, pSemaphore);
+#endif
+}
+
+void ma_semaphore_uninit(ma_semaphore* pSemaphore)
+{
+    if (pSemaphore == NULL) {
+        return;
+    }
+
+#ifdef MA_WIN32
+    ma_semaphore_uninit__win32(pSemaphore);
+#endif
+#ifdef MA_POSIX
+    ma_semaphore_uninit__posix(pSemaphore);
+#endif
+}
+
+ma_bool32 ma_semaphore_wait(ma_semaphore* pSemaphore)
+{
+    if (pSemaphore == NULL) {
+        return MA_FALSE;
+    }
+
+#ifdef MA_WIN32
+    return ma_semaphore_wait__win32(pSemaphore);
+#endif
+#ifdef MA_POSIX
+    return ma_semaphore_wait__posix(pSemaphore);
+#endif
+}
+
+ma_bool32 ma_semaphore_release(ma_semaphore* pSemaphore)
+{
+    if (pSemaphore == NULL) {
+        return MA_FALSE;
+    }
+
+#ifdef MA_WIN32
+    return ma_semaphore_release__win32(pSemaphore);
+#endif
+#ifdef MA_POSIX
+    return ma_semaphore_release__posix(pSemaphore);
+#endif
+}
+
+
 ma_uint32 ma_get_best_sample_rate_within_range(ma_uint32 sampleRateMin, ma_uint32 sampleRateMax)
 {
     /* Normalize the range in case we were given something stupid. */
     if (sampleRateMin < MA_MIN_SAMPLE_RATE) {
         sampleRateMin = MA_MIN_SAMPLE_RATE;
     }
     if (sampleRateMax > MA_MAX_SAMPLE_RATE) {
@@ -8225,14 +8423,15 @@
     ma_bool32 usingDefaultFormat;
     ma_bool32 usingDefaultChannels;
     ma_bool32 usingDefaultSampleRate;
     ma_bool32 usingDefaultChannelMap;
     ma_share_mode shareMode;
     ma_bool32 noAutoConvertSRC;
     ma_bool32 noDefaultQualitySRC;
+    ma_bool32 noHardwareOffloading;
 
     /* Output. */
     ma_IAudioClient* pAudioClient;
     ma_IAudioRenderClient* pRenderClient;
     ma_IAudioCaptureClient* pCaptureClient;
     ma_format formatOut;
     ma_uint32 channelsOut;
@@ -8285,28 +8484,30 @@
     result = ma_context_get_IAudioClient__wasapi(pContext, deviceType, pDeviceID, &pData->pAudioClient, &pDeviceInterface);
     if (result != MA_SUCCESS) {
         goto done;
     }
 
 
     /* Try enabling hardware offloading. */
-    hr = ma_IAudioClient_QueryInterface(pData->pAudioClient, &MA_IID_IAudioClient2, (void**)&pAudioClient2);
-    if (SUCCEEDED(hr)) {
-        BOOL isHardwareOffloadingSupported = 0;
-        hr = ma_IAudioClient2_IsOffloadCapable(pAudioClient2, MA_AudioCategory_Other, &isHardwareOffloadingSupported);
-        if (SUCCEEDED(hr) && isHardwareOffloadingSupported) {
-            ma_AudioClientProperties clientProperties;
-            ma_zero_object(&clientProperties);
-            clientProperties.cbSize = sizeof(clientProperties);
-            clientProperties.bIsOffload = 1;
-            clientProperties.eCategory = MA_AudioCategory_Other;
-            ma_IAudioClient2_SetClientProperties(pAudioClient2, &clientProperties);
-        }
+    if (!pData->noHardwareOffloading) {
+        hr = ma_IAudioClient_QueryInterface(pData->pAudioClient, &MA_IID_IAudioClient2, (void**)&pAudioClient2);
+        if (SUCCEEDED(hr)) {
+            BOOL isHardwareOffloadingSupported = 0;
+            hr = ma_IAudioClient2_IsOffloadCapable(pAudioClient2, MA_AudioCategory_Other, &isHardwareOffloadingSupported);
+            if (SUCCEEDED(hr) && isHardwareOffloadingSupported) {
+                ma_AudioClientProperties clientProperties;
+                ma_zero_object(&clientProperties);
+                clientProperties.cbSize = sizeof(clientProperties);
+                clientProperties.bIsOffload = 1;
+                clientProperties.eCategory = MA_AudioCategory_Other;
+                ma_IAudioClient2_SetClientProperties(pAudioClient2, &clientProperties);
+            }
 
-        pAudioClient2->lpVtbl->Release(pAudioClient2);
+            pAudioClient2->lpVtbl->Release(pAudioClient2);
+        }
     }
 
     /* Here is where we try to determine the best format to use with the device. If the client if wanting exclusive mode, first try finding the best format for that. If this fails, fall back to shared mode. */
     result = MA_FORMAT_NOT_SUPPORTED;
     if (pData->shareMode == ma_share_mode_exclusive) {
     #ifdef MA_WIN32_DESKTOP
         /* In exclusive mode on desktop we always use the backend's native format. */
@@ -8663,14 +8864,15 @@
     data.sampleRateIn               = pDevice->sampleRate;
     data.usingDefaultSampleRate     = pDevice->usingDefaultSampleRate;
     data.bufferSizeInFramesIn       = pDevice->wasapi.originalBufferSizeInFrames;
     data.bufferSizeInMillisecondsIn = pDevice->wasapi.originalBufferSizeInMilliseconds;
     data.periodsIn                  = pDevice->wasapi.originalPeriods;
     data.noAutoConvertSRC           = pDevice->wasapi.noAutoConvertSRC;
     data.noDefaultQualitySRC        = pDevice->wasapi.noDefaultQualitySRC;
+    data.noHardwareOffloading       = pDevice->wasapi.noHardwareOffloading;
     result = ma_device_init_internal__wasapi(pDevice->pContext, deviceType, NULL, &data);
     if (result != MA_SUCCESS) {
         return result;
     }
 
     /* At this point we have some new objects ready to go. We need to uninitialize the previous ones and then set the new ones. */
     if (deviceType == ma_device_type_capture || deviceType == ma_device_type_loopback) {
@@ -8757,16 +8959,17 @@
     ma_assert(pContext != NULL);
     ma_assert(pDevice != NULL);
 
     ma_zero_object(&pDevice->wasapi);
     pDevice->wasapi.originalBufferSizeInFrames       = pConfig->bufferSizeInFrames;
     pDevice->wasapi.originalBufferSizeInMilliseconds = pConfig->bufferSizeInMilliseconds;
     pDevice->wasapi.originalPeriods                  = pConfig->periods;
-    pDevice->wasapi.noAutoConvertSRC                 = pDevice->wasapi.noAutoConvertSRC;
-    pDevice->wasapi.noDefaultQualitySRC              = pDevice->wasapi.noDefaultQualitySRC;
+    pDevice->wasapi.noAutoConvertSRC                 = pConfig->wasapi.noAutoConvertSRC;
+    pDevice->wasapi.noDefaultQualitySRC              = pConfig->wasapi.noDefaultQualitySRC;
+    pDevice->wasapi.noHardwareOffloading             = pConfig->wasapi.noHardwareOffloading;
 
     /* Exclusive mode is not allowed with loopback. */
     if (pConfig->deviceType == ma_device_type_loopback && pConfig->playback.shareMode == ma_share_mode_exclusive) {
         return MA_INVALID_DEVICE_CONFIG;
     }
 
     if (pConfig->deviceType == ma_device_type_capture || pConfig->deviceType == ma_device_type_duplex || pConfig->deviceType == ma_device_type_loopback) {
@@ -8781,14 +8984,15 @@
         data.usingDefaultChannelMap     = pDevice->capture.usingDefaultChannelMap;
         data.shareMode                  = pConfig->capture.shareMode;
         data.bufferSizeInFramesIn       = pConfig->bufferSizeInFrames;
         data.bufferSizeInMillisecondsIn = pConfig->bufferSizeInMilliseconds;
         data.periodsIn                  = pConfig->periods;
         data.noAutoConvertSRC           = pConfig->wasapi.noAutoConvertSRC;
         data.noDefaultQualitySRC        = pConfig->wasapi.noDefaultQualitySRC;
+        data.noHardwareOffloading       = pConfig->wasapi.noHardwareOffloading;
 
         result = ma_device_init_internal__wasapi(pDevice->pContext, (pConfig->deviceType == ma_device_type_loopback) ? ma_device_type_loopback : ma_device_type_capture, pConfig->capture.pDeviceID, &data);
         if (result != MA_SUCCESS) {
             return result;
         }
 
         pDevice->wasapi.pAudioClientCapture         = data.pAudioClient;
@@ -8837,14 +9041,15 @@
         data.usingDefaultChannelMap     = pDevice->playback.usingDefaultChannelMap;
         data.shareMode                  = pConfig->playback.shareMode;
         data.bufferSizeInFramesIn       = pConfig->bufferSizeInFrames;
         data.bufferSizeInMillisecondsIn = pConfig->bufferSizeInMilliseconds;
         data.periodsIn                  = pConfig->periods;
         data.noAutoConvertSRC           = pConfig->wasapi.noAutoConvertSRC;
         data.noDefaultQualitySRC        = pConfig->wasapi.noDefaultQualitySRC;
+        data.noHardwareOffloading       = pConfig->wasapi.noHardwareOffloading;
 
         result = ma_device_init_internal__wasapi(pDevice->pContext, ma_device_type_playback, pConfig->playback.pDeviceID, &data);
         if (result != MA_SUCCESS) {
             if (pConfig->deviceType == ma_device_type_duplex) {
                 if (pDevice->wasapi.pCaptureClient != NULL) {
                     ma_IAudioCaptureClient_Release((ma_IAudioCaptureClient*)pDevice->wasapi.pCaptureClient);
                     pDevice->wasapi.pCaptureClient = NULL;
@@ -8912,15 +9117,15 @@
     }
 
     /*
     We need to get notifications of when the default device changes. We do this through a device enumerator by
     registering a IMMNotificationClient with it. We only care about this if it's the default device.
     */
 #ifdef MA_WIN32_DESKTOP
-    {
+    if (pConfig->wasapi.noAutoStreamRouting == MA_FALSE) {
         ma_IMMDeviceEnumerator* pDeviceEnumerator;
         HRESULT hr = ma_CoCreateInstance(pContext, MA_CLSID_MMDeviceEnumerator, NULL, CLSCTX_ALL, MA_IID_IMMDeviceEnumerator, (void**)&pDeviceEnumerator);
         if (FAILED(hr)) {
             ma_device_uninit__wasapi(pDevice);
             return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[WASAPI] Failed to create device enumerator.", MA_FAILED_TO_OPEN_BACKEND_DEVICE);
         }
 
@@ -16573,16 +16778,19 @@
 
     totalFramesRead = 0;
     while (totalFramesRead < frameCount) {
         if (ma_device__get_state(pDevice) != MA_STATE_STARTED) {
             return MA_DEVICE_NOT_STARTED;
         }
 
-        /* If a buffer is mapped we need to write to that first. Once it's consumed we reset the event and unmap it. */
-        if (pDevice->pulse.pMappedBufferCapture != NULL && pDevice->pulse.mappedBufferFramesRemainingCapture > 0) {
+        /*
+        If a buffer is mapped we need to read from that first. Once it's consumed we need to drop it. Note that pDevice->pulse.pMappedBufferCapture can be null in which
+        case it could be a hole. In this case we just write zeros into the output buffer.
+        */
+        if (pDevice->pulse.mappedBufferFramesRemainingCapture > 0) {
             ma_uint32 bpf = ma_get_bytes_per_frame(pDevice->capture.internalFormat, pDevice->capture.internalChannels);
             ma_uint32 mappedBufferFramesConsumed = pDevice->pulse.mappedBufferFramesCapacityCapture - pDevice->pulse.mappedBufferFramesRemainingCapture;
 
             ma_uint32  framesToCopy = ma_min(pDevice->pulse.mappedBufferFramesRemainingCapture, (frameCount - totalFramesRead));
             void* pDst = (ma_uint8*)pPCMFrames + (totalFramesRead * bpf);
 
             /*
@@ -16590,26 +16798,35 @@
             when the current fragment is a hole. For a hole we just output silence.
             */
             if (pDevice->pulse.pMappedBufferCapture != NULL) {
                 const void* pSrc = (const ma_uint8*)pDevice->pulse.pMappedBufferCapture + (mappedBufferFramesConsumed * bpf);
                 ma_copy_memory(pDst, pSrc, framesToCopy * bpf);
             } else {
                 ma_zero_memory(pDst, framesToCopy * bpf);
+            #if defined(MA_DEBUG_OUTPUT)
+                printf("[PulseAudio] ma_device_read__pulse: Filling hole with silence.\n");
+            #endif
             }
 
             pDevice->pulse.mappedBufferFramesRemainingCapture -= framesToCopy;
             totalFramesRead += framesToCopy;
         }
 
         /*
         Getting here means we've run out of data in the currently mapped chunk. We need to drop this from the device and then try
         mapping another chunk. If this fails we need to wait for data to become available.
         */
         if (pDevice->pulse.mappedBufferFramesCapacityCapture > 0 && pDevice->pulse.mappedBufferFramesRemainingCapture == 0) {
-            int error = ((ma_pa_stream_drop_proc)pDevice->pContext->pulse.pa_stream_drop)((ma_pa_stream*)pDevice->pulse.pStreamCapture);
+            int error;
+
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[PulseAudio] ma_device_read__pulse: Call pa_stream_drop()\n");
+        #endif
+
+            error = ((ma_pa_stream_drop_proc)pDevice->pContext->pulse.pa_stream_drop)((ma_pa_stream*)pDevice->pulse.pStreamCapture);
             if (error != 0) {
                 return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[PulseAudio] Failed to drop fragment.", ma_result_from_pulse(error));
             }
 
             pDevice->pulse.pMappedBufferCapture = NULL;
             pDevice->pulse.mappedBufferFramesRemainingCapture = 0;
             pDevice->pulse.mappedBufferFramesCapacityCapture = 0;
@@ -16618,67 +16835,78 @@
         ma_assert(totalFramesRead <= frameCount);
         if (totalFramesRead == frameCount) {
             break;
         }
 
         /* Getting here means we need to map a new buffer. If we don't have enough data we wait for more. */
         for (;;) {
-            size_t readableSizeInBytes;
+            int error;
+            size_t bytesMapped;
 
             if (ma_device__get_state(pDevice) != MA_STATE_STARTED) {
                 break;
             }
 
             /* If the device has been corked, don't try to continue. */
             if (((ma_pa_stream_is_corked_proc)pDevice->pContext->pulse.pa_stream_is_corked)((ma_pa_stream*)pDevice->pulse.pStreamCapture)) {
+            #if defined(MA_DEBUG_OUTPUT)
+                printf("[PulseAudio] ma_device_read__pulse: Corked.\n");
+            #endif
                 break;
             }
 
-            readableSizeInBytes = ((ma_pa_stream_readable_size_proc)pDevice->pContext->pulse.pa_stream_readable_size)((ma_pa_stream*)pDevice->pulse.pStreamCapture);
-            if (readableSizeInBytes != (size_t)-1) {
-                /*size_t periodSizeInBytes = (pDevice->capture.internalBufferSizeInFrames / pDevice->capture.internalPeriods) * ma_get_bytes_per_frame(pDevice->capture.internalFormat, pDevice->capture.internalChannels);*/
-                if (readableSizeInBytes > 0) {
-                    /* Data is avaialable. */
-                    size_t bytesMapped = (size_t)-1;
-                    int error = ((ma_pa_stream_peek_proc)pDevice->pContext->pulse.pa_stream_peek)((ma_pa_stream*)pDevice->pulse.pStreamCapture, &pDevice->pulse.pMappedBufferCapture, &bytesMapped);
-                    if (error < 0) {
-                        return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[PulseAudio] Failed to peek capture buffer.", ma_result_from_pulse(error));
-                    }
+            ma_assert(pDevice->pulse.pMappedBufferCapture == NULL); /* <-- We're about to map a buffer which means we shouldn't have an existing mapping. */
 
-                    if (pDevice->pulse.pMappedBufferCapture == NULL && bytesMapped == 0) {
-                        /* Nothing available. This shouldn't happen because we checked earlier with pa_stream_readable_size(). I'm going to throw an error in this case. */
-                        return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[PulseAudio] Nothing available after peeking capture buffer.", MA_ERROR);
-                    }
+            error = ((ma_pa_stream_peek_proc)pDevice->pContext->pulse.pa_stream_peek)((ma_pa_stream*)pDevice->pulse.pStreamCapture, &pDevice->pulse.pMappedBufferCapture, &bytesMapped);
+            if (error < 0) {
+                return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[PulseAudio] Failed to peek capture buffer.", ma_result_from_pulse(error));
+            }
 
-                    pDevice->pulse.mappedBufferFramesCapacityCapture  = bytesMapped / ma_get_bytes_per_frame(pDevice->capture.internalFormat, pDevice->capture.internalChannels);
-                    pDevice->pulse.mappedBufferFramesRemainingCapture = pDevice->pulse.mappedBufferFramesCapacityCapture;
+            if (bytesMapped > 0) {
+                pDevice->pulse.mappedBufferFramesCapacityCapture  = bytesMapped / ma_get_bytes_per_frame(pDevice->capture.internalFormat, pDevice->capture.internalChannels);
+                pDevice->pulse.mappedBufferFramesRemainingCapture = pDevice->pulse.mappedBufferFramesCapacityCapture;
 
-                    break;
-                } else {
-                    /* No data available. Need to wait for more. */
+                #if defined(MA_DEBUG_OUTPUT)
+                    printf("[PulseAudio] ma_device_read__pulse: Mapped. mappedBufferFramesCapacityCapture=%d, mappedBufferFramesRemainingCapture=%d\n", pDevice->pulse.mappedBufferFramesCapacityCapture, pDevice->pulse.mappedBufferFramesRemainingCapture);
+                #endif
+
+                if (pDevice->pulse.pMappedBufferCapture == NULL) {
+                    /* It's a hole. */
+                    #if defined(MA_DEBUG_OUTPUT)
+                        printf("[PulseAudio] ma_device_read__pulse: Call pa_stream_peek(). Hole.\n");
+                    #endif
+                }
+
+                break;
+            } else {
+                if (pDevice->pulse.pMappedBufferCapture == NULL) {
+                    /* Nothing available yet. Need to wait for more. */
 
                     /*
                     I have had reports of a deadlock in this part of the code. I have reproduced this when using the "Built-in Audio Analogue Stereo" device without
                     an actual microphone connected. I'm experimenting here by not blocking in pa_mainloop_iterate() and instead sleep for a bit when there are no
                     dispatches.
                     */
-                    int error = ((ma_pa_mainloop_iterate_proc)pDevice->pContext->pulse.pa_mainloop_iterate)((ma_pa_mainloop*)pDevice->pulse.pMainLoop, 0, NULL);
+                    error = ((ma_pa_mainloop_iterate_proc)pDevice->pContext->pulse.pa_mainloop_iterate)((ma_pa_mainloop*)pDevice->pulse.pMainLoop, 0, NULL);
                     if (error < 0) {
                         return ma_result_from_pulse(error);
                     }
 
                     /* Sleep for a bit if nothing was dispatched. */
                     if (error == 0) {
                         ma_sleep(1);
                     }
 
-                    continue;
+                #if defined(MA_DEBUG_OUTPUT)
+                    printf("[PulseAudio] ma_device_read__pulse: No data available. Waiting. mappedBufferFramesCapacityCapture=%d, mappedBufferFramesRemainingCapture=%d\n", pDevice->pulse.mappedBufferFramesCapacityCapture, pDevice->pulse.mappedBufferFramesRemainingCapture);
+                #endif
+                } else {
+                    /* Getting here means we mapped 0 bytes, but have a non-NULL buffer. I don't think this should ever happen. */
+                    MA_ASSERT(MA_FALSE);
                 }
-            } else {
-                return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[PulseAudio] Failed to query the stream's readable size.", MA_ERROR);
             }
         }
     }
 
     if (pFramesRead != NULL) {
         *pFramesRead = totalFramesRead;
     }
@@ -17268,15 +17496,15 @@
 
     pDeviceInfo->minSampleRate = ((ma_jack_get_sample_rate_proc)pContext->jack.jack_get_sample_rate)((ma_jack_client_t*)pClient);
     pDeviceInfo->maxSampleRate = pDeviceInfo->minSampleRate;
 
     pDeviceInfo->minChannels = 0;
     pDeviceInfo->maxChannels = 0;
 
-    ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pClient, NULL, NULL, ma_JackPortIsPhysical | ((deviceType == ma_device_type_playback) ? ma_JackPortIsInput : ma_JackPortIsOutput));
+    ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pClient, NULL, MA_JACK_DEFAULT_AUDIO_TYPE, ma_JackPortIsPhysical | ((deviceType == ma_device_type_playback) ? ma_JackPortIsInput : ma_JackPortIsOutput));
     if (ppPorts == NULL) {
         ((ma_jack_client_close_proc)pContext->jack.jack_client_close)((ma_jack_client_t*)pClient);
         return ma_context_post_error(pContext, NULL, MA_LOG_LEVEL_ERROR, "[JACK] Failed to query physical ports.", MA_FAILED_TO_OPEN_BACKEND_DEVICE);
     }
 
     while (ppPorts[pDeviceInfo->minChannels] != NULL) {
         pDeviceInfo->minChannels += 1;
@@ -17466,15 +17694,15 @@
         const char** ppPorts;
 
         pDevice->capture.internalFormat = ma_format_f32;
         pDevice->capture.internalChannels = 0;
         pDevice->capture.internalSampleRate = ((ma_jack_get_sample_rate_proc)pContext->jack.jack_get_sample_rate)((ma_jack_client_t*)pDevice->jack.pClient);
         ma_get_standard_channel_map(ma_standard_channel_map_alsa, pDevice->capture.internalChannels, pDevice->capture.internalChannelMap);
 
-        ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, NULL, ma_JackPortIsPhysical | ma_JackPortIsOutput);
+        ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, MA_JACK_DEFAULT_AUDIO_TYPE, ma_JackPortIsPhysical | ma_JackPortIsOutput);
         if (ppPorts == NULL) {
             return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[JACK] Failed to query physical ports.", MA_FAILED_TO_OPEN_BACKEND_DEVICE);
         }
 
         while (ppPorts[pDevice->capture.internalChannels] != NULL) {
             char name[64];
             ma_strcpy_s(name, sizeof(name), "capture");
@@ -17506,15 +17734,15 @@
         const char** ppPorts;
 
         pDevice->playback.internalFormat = ma_format_f32;
         pDevice->playback.internalChannels = 0;
         pDevice->playback.internalSampleRate = ((ma_jack_get_sample_rate_proc)pContext->jack.jack_get_sample_rate)((ma_jack_client_t*)pDevice->jack.pClient);
         ma_get_standard_channel_map(ma_standard_channel_map_alsa, pDevice->playback.internalChannels, pDevice->playback.internalChannelMap);
 
-        ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, NULL, ma_JackPortIsPhysical | ma_JackPortIsInput);
+        ppPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, MA_JACK_DEFAULT_AUDIO_TYPE, ma_JackPortIsPhysical | ma_JackPortIsInput);
         if (ppPorts == NULL) {
             return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[JACK] Failed to query physical ports.", MA_FAILED_TO_OPEN_BACKEND_DEVICE);
         }
 
         while (ppPorts[pDevice->playback.internalChannels] != NULL) {
             char name[64];
             ma_strcpy_s(name, sizeof(name), "playback");
@@ -17574,15 +17802,15 @@
 
     resultJACK = ((ma_jack_activate_proc)pContext->jack.jack_activate)((ma_jack_client_t*)pDevice->jack.pClient);
     if (resultJACK != 0) {
         return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[JACK] Failed to activate the JACK client.", MA_FAILED_TO_START_BACKEND_DEVICE);
     }
 
     if (pDevice->type == ma_device_type_capture || pDevice->type == ma_device_type_duplex) {
-        const char** ppServerPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, NULL, ma_JackPortIsPhysical | ma_JackPortIsOutput);
+        const char** ppServerPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, MA_JACK_DEFAULT_AUDIO_TYPE, ma_JackPortIsPhysical | ma_JackPortIsOutput);
         if (ppServerPorts == NULL) {
             ((ma_jack_deactivate_proc)pContext->jack.jack_deactivate)((ma_jack_client_t*)pDevice->jack.pClient);
             return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[JACK] Failed to retrieve physical ports.", MA_ERROR);
         }
 
         for (i = 0; ppServerPorts[i] != NULL; ++i) {
             const char* pServerPort = ppServerPorts[i];
@@ -17596,15 +17824,15 @@
             }
         }
 
         ((ma_jack_free_proc)pContext->jack.jack_free)((void*)ppServerPorts);
     }
     
     if (pDevice->type == ma_device_type_playback || pDevice->type == ma_device_type_duplex) {
-        const char** ppServerPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, NULL, ma_JackPortIsPhysical | ma_JackPortIsInput);
+        const char** ppServerPorts = ((ma_jack_get_ports_proc)pContext->jack.jack_get_ports)((ma_jack_client_t*)pDevice->jack.pClient, NULL, MA_JACK_DEFAULT_AUDIO_TYPE, ma_JackPortIsPhysical | ma_JackPortIsInput);
         if (ppServerPorts == NULL) {
             ((ma_jack_deactivate_proc)pContext->jack.jack_deactivate)((ma_jack_client_t*)pDevice->jack.pClient);
             return ma_post_error(pDevice, MA_LOG_LEVEL_ERROR, "[JACK] Failed to retrieve physical ports.", MA_ERROR);
         }
 
         for (i = 0; ppServerPorts[i] != NULL; ++i) {
             const char* pServerPort = ppServerPorts[i];
@@ -17783,14 +18011,20 @@
 
 ******************************************************************************/
 #ifdef MA_HAS_COREAUDIO
 #include <TargetConditionals.h>
 
 #if defined(TARGET_OS_IPHONE) && TARGET_OS_IPHONE == 1
     #define MA_APPLE_MOBILE
+    #if defined(TARGET_OS_TV) && TARGET_OS_TV == 1
+        #define MA_APPLE_TV
+    #endif
+    #if defined(TARGET_OS_WATCH) && TARGET_OS_WATCH == 1
+        #define MA_APPLE_WATCH
+    #endif
 #else
     #define MA_APPLE_DESKTOP
 #endif
 
 #if defined(MA_APPLE_DESKTOP)
 #include <CoreAudio/CoreAudio.h>
 #else
@@ -19245,41 +19479,49 @@
             #if defined(MA_DEBUG_OUTPUT)
                 printf("  WARNING: Outputting silence. frameCount=%d, mNumberChannels=%d, mDataByteSize=%d\n", frameCount, pBufferList->mBuffers[iBuffer].mNumberChannels, pBufferList->mBuffers[iBuffer].mDataByteSize);
             #endif
             }
         }
     } else {
         /* This is the deinterleaved case. We need to update each buffer in groups of internalChannels. This assumes each buffer is the same size. */
-        ma_uint8 tempBuffer[4096];
-        UInt32 iBuffer;
-        for (iBuffer = 0; iBuffer < pBufferList->mNumberBuffers; iBuffer += pDevice->playback.internalChannels) {
-            ma_uint32 frameCountPerBuffer = pBufferList->mBuffers[iBuffer].mDataByteSize / ma_get_bytes_per_sample(pDevice->playback.internalFormat);
-            ma_uint32 framesRemaining = frameCountPerBuffer;
+        
+        /*
+        For safety we'll check that the internal channels is a multiple of the buffer count. If it's not it means something
+        very strange has happened and we're not going to support it.
+        */
+        if ((pBufferList->mNumberBuffers % pDevice->playback.internalChannels) == 0) {
+            ma_uint8 tempBuffer[4096];
+            UInt32 iBuffer;
+        
+            for (iBuffer = 0; iBuffer < pBufferList->mNumberBuffers; iBuffer += pDevice->playback.internalChannels) {
+                ma_uint32 frameCountPerBuffer = pBufferList->mBuffers[iBuffer].mDataByteSize / ma_get_bytes_per_sample(pDevice->playback.internalFormat);
+                ma_uint32 framesRemaining = frameCountPerBuffer;
 
-            while (framesRemaining > 0) {
-                void* ppDeinterleavedBuffers[MA_MAX_CHANNELS];
-                ma_uint32 iChannel;
-                ma_uint32 framesToRead = sizeof(tempBuffer) / ma_get_bytes_per_frame(pDevice->playback.internalFormat, pDevice->playback.internalChannels);
-                if (framesToRead > framesRemaining) {
-                    framesToRead = framesRemaining;
-                }
-                
-                if (pDevice->type == ma_device_type_duplex) {
-                    ma_device__handle_duplex_callback_playback(pDevice, framesToRead, tempBuffer, &pDevice->coreaudio.duplexRB);
-                } else {
-                    ma_device__read_frames_from_client(pDevice, framesToRead, tempBuffer);
-                }
-                
-                for (iChannel = 0; iChannel < pDevice->playback.internalChannels; ++iChannel) {
-                    ppDeinterleavedBuffers[iChannel] = (void*)ma_offset_ptr(pBufferList->mBuffers[iBuffer].mData, (frameCountPerBuffer - framesRemaining) * ma_get_bytes_per_sample(pDevice->playback.internalFormat));
+                while (framesRemaining > 0) {
+                    void* ppDeinterleavedBuffers[MA_MAX_CHANNELS];
+                    ma_uint32 iChannel;
+                    ma_uint32 framesToRead = sizeof(tempBuffer) / ma_get_bytes_per_frame(pDevice->playback.internalFormat, pDevice->playback.internalChannels);
+                    if (framesToRead > framesRemaining) {
+                        framesToRead = framesRemaining;
+                    }
+                    
+                    if (pDevice->type == ma_device_type_duplex) {
+                        ma_device__handle_duplex_callback_playback(pDevice, framesToRead, tempBuffer, &pDevice->coreaudio.duplexRB);
+                    } else {
+                        ma_device__read_frames_from_client(pDevice, framesToRead, tempBuffer);
+                    }
+                    
+                    for (iChannel = 0; iChannel < pDevice->playback.internalChannels; ++iChannel) {
+                        ppDeinterleavedBuffers[iChannel] = (void*)ma_offset_ptr(pBufferList->mBuffers[iBuffer+iChannel].mData, (frameCountPerBuffer - framesRemaining) * ma_get_bytes_per_sample(pDevice->playback.internalFormat));
+                    }
+                    
+                    ma_deinterleave_pcm_frames(pDevice->playback.internalFormat, pDevice->playback.internalChannels, framesToRead, tempBuffer, ppDeinterleavedBuffers);
+                    
+                    framesRemaining -= framesToRead;
                 }
-                
-                ma_deinterleave_pcm_frames(pDevice->playback.internalFormat, pDevice->playback.internalChannels, framesToRead, tempBuffer, ppDeinterleavedBuffers);
-                
-                framesRemaining -= framesToRead;
             }
         }
     }
     
     (void)pActionFlags;
     (void)pTimeStamp;
     (void)busNumber;
@@ -19358,39 +19600,46 @@
             #if defined(MA_DEBUG_OUTPUT)
                 printf("  WARNING: Outputting silence. frameCount=%d, mNumberChannels=%d, mDataByteSize=%d\n", frameCount, pRenderedBufferList->mBuffers[iBuffer].mNumberChannels, pRenderedBufferList->mBuffers[iBuffer].mDataByteSize);
             #endif
             }
         }
     } else {
         /* This is the deinterleaved case. We need to interleave the audio data before sending it to the client. This assumes each buffer is the same size. */
-        ma_uint8 tempBuffer[4096];
-        UInt32 iBuffer;
-        for (iBuffer = 0; iBuffer < pRenderedBufferList->mNumberBuffers; iBuffer += pDevice->capture.internalChannels) {
-            ma_uint32 framesRemaining = frameCount;
-            while (framesRemaining > 0) {
-                void* ppDeinterleavedBuffers[MA_MAX_CHANNELS];
-                ma_uint32 iChannel;
-                ma_uint32 framesToSend = sizeof(tempBuffer) / ma_get_bytes_per_sample(pDevice->capture.internalFormat);
-                if (framesToSend > framesRemaining) {
-                    framesToSend = framesRemaining;
-                }
-                
-                for (iChannel = 0; iChannel < pDevice->capture.internalChannels; ++iChannel) {
-                    ppDeinterleavedBuffers[iChannel] = (void*)ma_offset_ptr(pRenderedBufferList->mBuffers[iBuffer].mData, (frameCount - framesRemaining) * ma_get_bytes_per_sample(pDevice->capture.internalFormat));
-                }
-                
-                ma_interleave_pcm_frames(pDevice->capture.internalFormat, pDevice->capture.internalChannels, framesToSend, (const void**)ppDeinterleavedBuffers, tempBuffer);
+        
+        /*
+        For safety we'll check that the internal channels is a multiple of the buffer count. If it's not it means something
+        very strange has happened and we're not going to support it.
+        */
+        if ((pRenderedBufferList->mNumberBuffers % pDevice->capture.internalChannels) == 0) {
+            ma_uint8 tempBuffer[4096];
+            UInt32 iBuffer;
+            for (iBuffer = 0; iBuffer < pRenderedBufferList->mNumberBuffers; iBuffer += pDevice->capture.internalChannels) {
+                ma_uint32 framesRemaining = frameCount;
+                while (framesRemaining > 0) {
+                    void* ppDeinterleavedBuffers[MA_MAX_CHANNELS];
+                    ma_uint32 iChannel;
+                    ma_uint32 framesToSend = sizeof(tempBuffer) / ma_get_bytes_per_sample(pDevice->capture.internalFormat);
+                    if (framesToSend > framesRemaining) {
+                        framesToSend = framesRemaining;
+                    }
+                    
+                    for (iChannel = 0; iChannel < pDevice->capture.internalChannels; ++iChannel) {
+                        ppDeinterleavedBuffers[iChannel] = (void*)ma_offset_ptr(pRenderedBufferList->mBuffers[iBuffer+iChannel].mData, (frameCount - framesRemaining) * ma_get_bytes_per_sample(pDevice->capture.internalFormat));
+                    }
+                    
+                    ma_interleave_pcm_frames(pDevice->capture.internalFormat, pDevice->capture.internalChannels, framesToSend, (const void**)ppDeinterleavedBuffers, tempBuffer);
 
-                if (pDevice->type == ma_device_type_duplex) {
-                    ma_device__handle_duplex_callback_capture(pDevice, framesToSend, tempBuffer, &pDevice->coreaudio.duplexRB);
-                } else {
-                    ma_device__send_frames_to_client(pDevice, framesToSend, tempBuffer);
-                }
+                    if (pDevice->type == ma_device_type_duplex) {
+                        ma_device__handle_duplex_callback_capture(pDevice, framesToSend, tempBuffer, &pDevice->coreaudio.duplexRB);
+                    } else {
+                        ma_device__send_frames_to_client(pDevice, framesToSend, tempBuffer);
+                    }
 
-                framesRemaining -= framesToSend;
+                    framesRemaining -= framesToSend;
+                }
             }
         }
     }
 
     (void)pActionFlags;
     (void)pTimeStamp;
     (void)busNumber;
@@ -19672,26 +19921,131 @@
         return result;
     }
     
     return MA_SUCCESS;
 }
 #endif
 
+#if defined(MA_APPLE_MOBILE)
+@interface ma_router_change_handler:NSObject {
+    ma_device* m_pDevice;
+}
+@end
+
+@implementation ma_router_change_handler
+-(id)init:(ma_device*)pDevice
+{
+    self = [super init];
+    m_pDevice = pDevice;
+
+    [[NSNotificationCenter defaultCenter] addObserver:self selector:@selector(handle_route_change:) name:AVAudioSessionRouteChangeNotification object:[AVAudioSession sharedInstance]];
+
+    return self;
+}
+
+-(void)dealloc
+{
+    [self remove_handler];
+}
+
+-(void)remove_handler
+{
+    [[NSNotificationCenter defaultCenter] removeObserver:self name:@"AVAudioSessionRouteChangeNotification" object:nil];
+}
+
+-(void)handle_route_change:(NSNotification*)pNotification
+{
+    AVAudioSession* pSession = [AVAudioSession sharedInstance];
+
+    NSInteger reason = [[[pNotification userInfo] objectForKey:AVAudioSessionRouteChangeReasonKey] integerValue];
+    switch (reason)
+    {
+        case AVAudioSessionRouteChangeReasonOldDeviceUnavailable:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonOldDeviceUnavailable\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonNewDeviceAvailable:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonNewDeviceAvailable\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonNoSuitableRouteForCategory:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonNoSuitableRouteForCategory\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonWakeFromSleep:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonWakeFromSleep\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonOverride:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonOverride\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonCategoryChange:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonCategoryChange\n");
+        #endif
+        } break;
+
+        case AVAudioSessionRouteChangeReasonUnknown:
+        default:
+        {
+        #if defined(MA_DEBUG_OUTPUT)
+            printf("[Core Audio] Route Changed: AVAudioSessionRouteChangeReasonUnknown\n");
+        #endif
+        } break;
+    }
+
+    m_pDevice->sampleRate = (ma_uint32)pSession.sampleRate;
+
+    if (m_pDevice->type == ma_device_type_capture || m_pDevice->type == ma_device_type_duplex) {
+        m_pDevice->capture.channels = (ma_uint32)pSession.inputNumberOfChannels;
+        ma_device__post_init_setup(m_pDevice, ma_device_type_capture);
+    }
+    if (m_pDevice->type == ma_device_type_playback || m_pDevice->type == ma_device_type_duplex) {
+        m_pDevice->playback.channels = (ma_uint32)pSession.outputNumberOfChannels;
+        ma_device__post_init_setup(m_pDevice, ma_device_type_playback);
+    }
+}
+@end
+#endif
+
 void ma_device_uninit__coreaudio(ma_device* pDevice)
 {
     ma_assert(pDevice != NULL);
     ma_assert(ma_device__get_state(pDevice) == MA_STATE_UNINITIALIZED);
     
 #if defined(MA_APPLE_DESKTOP)
     /*
     Make sure we're no longer tracking the device. It doesn't matter if we call this for a non-default device because it'll
     just gracefully ignore it.
     */
     ma_device__untrack__coreaudio(pDevice);
 #endif
+#if defined(MA_APPLE_MOBILE)
+    if (pDevice->coreaudio.pRouteChangeHandler != NULL) {
+        ma_router_change_handler* pRouteChangeHandler = (__bridge ma_router_change_handler*)pDevice->coreaudio.pRouteChangeHandler;
+        [pRouteChangeHandler remove_handler];
+    }
+#endif
     
     if (pDevice->coreaudio.audioUnitCapture != NULL) {
         ((ma_AudioComponentInstanceDispose_proc)pDevice->pContext->coreaudio.AudioComponentInstanceDispose)((AudioUnit)pDevice->coreaudio.audioUnitCapture);
     }
     if (pDevice->coreaudio.audioUnitPlayback != NULL) {
         ((ma_AudioComponentInstanceDispose_proc)pDevice->pContext->coreaudio.AudioComponentInstanceDispose)((AudioUnit)pDevice->coreaudio.audioUnitPlayback);
     }
@@ -19882,14 +20236,25 @@
         */
         @autoreleasepool {
             AVAudioSession* pAudioSession = [AVAudioSession sharedInstance];
             ma_assert(pAudioSession != NULL);
             
             [pAudioSession setPreferredSampleRate:(double)pData->sampleRateIn error:nil];
             bestFormat.mSampleRate = pAudioSession.sampleRate;
+
+            /*
+            I've had a report that the channel count returned by AudioUnitGetProperty above is inconsistent with
+            AVAudioSession outputNumberOfChannels. I'm going to try using the AVAudioSession values instead.
+            */
+            if (deviceType == ma_device_type_playback) {
+                bestFormat.mChannelsPerFrame = (UInt32)pAudioSession.outputNumberOfChannels;
+            }
+            if (deviceType == ma_device_type_capture) {
+                bestFormat.mChannelsPerFrame = (UInt32)pAudioSession.inputNumberOfChannels;
+            }
         }
         
         status = ((ma_AudioUnitSetProperty_proc)pContext->coreaudio.AudioUnitSetProperty)(pData->audioUnit, kAudioUnitProperty_StreamFormat, formatScope, formatElement, &bestFormat, sizeof(bestFormat));
         if (status != noErr) {
             ((ma_AudioComponentInstanceDispose_proc)pContext->coreaudio.AudioComponentInstanceDispose)(pData->audioUnit);
             return ma_result_from_OSStatus(status);
         }
@@ -20321,14 +20686,22 @@
             {
                 ma_zero_memory(pBufferData, bufferSizeInFrames * ma_get_bytes_per_frame(pDevice->capture.format, pDevice->capture.channels));
             }
             ma_pcm_rb_commit_write(&pDevice->coreaudio.duplexRB, bufferSizeInFrames, pBufferData);
         }
     }
 
+    /*
+    We need to detect when a route has changed so we can update the data conversion pipeline accordingly. This is done
+    differently on non-Desktop Apple platforms.
+    */
+#if defined(MA_APPLE_MOBILE)
+    pDevice->coreaudio.pRouteChangeHandler = (__bridge void*)[[ma_router_change_handler alloc] init:pDevice];
+#endif
+
     return MA_SUCCESS;
 }
 
 
 ma_result ma_device_start__coreaudio(ma_device* pDevice)
 {
     ma_assert(pDevice != NULL);
@@ -20388,43 +20761,83 @@
     ma_dlclose(pContext, pContext->coreaudio.hCoreFoundation);
 #endif
 
     (void)pContext;
     return MA_SUCCESS;
 }
 
+#if defined(MA_APPLE_MOBILE)
+static AVAudioSessionCategory ma_to_AVAudioSessionCategory(ma_ios_session_category category)
+{
+    /* The "default" and "none" categories are treated different and should not be used as an input into this function. */
+    ma_assert(category != ma_ios_session_category_default);
+    ma_assert(category != ma_ios_session_category_none);
+
+    switch (category) {
+        case ma_ios_session_category_ambient:         return AVAudioSessionCategoryAmbient;
+        case ma_ios_session_category_solo_ambient:    return AVAudioSessionCategorySoloAmbient;
+        case ma_ios_session_category_playback:        return AVAudioSessionCategoryPlayback;
+        case ma_ios_session_category_record:          return AVAudioSessionCategoryRecord;
+        case ma_ios_session_category_play_and_record: return AVAudioSessionCategoryPlayAndRecord;
+        case ma_ios_session_category_multi_route:     return AVAudioSessionCategoryMultiRoute;
+        case ma_ios_session_category_none:            return AVAudioSessionCategoryAmbient;
+        case ma_ios_session_category_default:         return AVAudioSessionCategoryAmbient;
+        default:                                      return AVAudioSessionCategoryAmbient;
+    }
+}
+#endif
+
 ma_result ma_context_init__coreaudio(const ma_context_config* pConfig, ma_context* pContext)
 {
+    ma_assert(pConfig != NULL);
     ma_assert(pContext != NULL);
 
-    (void)pConfig;
-
 #if defined(MA_APPLE_MOBILE)
     @autoreleasepool {
         AVAudioSession* pAudioSession = [AVAudioSession sharedInstance];
+        AVAudioSessionCategoryOptions options = pConfig->coreaudio.sessionCategoryOptions;
+
         ma_assert(pAudioSession != NULL);
 
-        [pAudioSession setCategory: AVAudioSessionCategoryPlayAndRecord error:nil];
-        
-        /* By default we want miniaudio to use the speakers instead of the receiver. In the future this may be customizable. */
-        ma_bool32 useSpeakers = MA_TRUE;
-        if (useSpeakers) {
-            [pAudioSession overrideOutputAudioPort:AVAudioSessionPortOverrideSpeaker error:nil];
+        if (pConfig->coreaudio.sessionCategory == ma_ios_session_category_default) {
+            /*
+            I'm going to use trial and error to determine our default session category. First we'll try PlayAndRecord. If that fails
+            we'll try Playback and if that fails we'll try record. If all of these fail we'll just not set the category.
+            */
+        #if !defined(MA_APPLE_TV) && !defined(MA_APPLE_WATCH)
+            options |= AVAudioSessionCategoryOptionDefaultToSpeaker;
+        #endif
+
+            if ([pAudioSession setCategory: AVAudioSessionCategoryPlayAndRecord withOptions:options error:nil]) {
+                /* Using PlayAndRecord */
+            } else if ([pAudioSession setCategory: AVAudioSessionCategoryPlayback withOptions:options error:nil]) {
+                /* Using Playback */
+            } else if ([pAudioSession setCategory: AVAudioSessionCategoryRecord withOptions:options error:nil]) {
+                /* Using Record */
+            } else {
+                /* Leave as default? */
+            }
+        } else {
+            if (pConfig->coreaudio.sessionCategory != ma_ios_session_category_none) {
+                if (![pAudioSession setCategory: ma_to_AVAudioSessionCategory(pConfig->coreaudio.sessionCategory) withOptions:options error:nil]) {
+                    return MA_INVALID_OPERATION;    /* Failed to set session category. */
+                }
+            }
         }
     }
 #endif
     
 #if !defined(MA_NO_RUNTIME_LINKING) && !defined(MA_APPLE_MOBILE)
     pContext->coreaudio.hCoreFoundation = ma_dlopen(pContext, "CoreFoundation.framework/CoreFoundation");
     if (pContext->coreaudio.hCoreFoundation == NULL) {
         return MA_API_NOT_FOUND;
     }
     
-    pContext->coreaudio.CFStringGetCString             = ma_dlsym(pContext, pContext->coreaudio.hCoreFoundation, "CFStringGetCString");
-    pContext->coreaudio.CFRelease                      = ma_dlsym(pContext, pContext->coreaudio.hCoreFoundation, "CFRelease");
+    pContext->coreaudio.CFStringGetCString = ma_dlsym(pContext, pContext->coreaudio.hCoreFoundation, "CFStringGetCString");
+    pContext->coreaudio.CFRelease          = ma_dlsym(pContext, pContext->coreaudio.hCoreFoundation, "CFRelease");
     
     
     pContext->coreaudio.hCoreAudio = ma_dlopen(pContext, "CoreAudio.framework/CoreAudio");
     if (pContext->coreaudio.hCoreAudio == NULL) {
         ma_dlclose(pContext, pContext->coreaudio.hCoreFoundation);
         return MA_API_NOT_FOUND;
     }
@@ -23247,27 +23660,29 @@
 #define MA_AAUDIO_CALLBACK_RESULT_CONTINUE         0
 #define MA_AAUDIO_CALLBACK_RESULT_STOP             1
 
 /* Objects. */
 typedef struct ma_AAudioStreamBuilder_t* ma_AAudioStreamBuilder;
 typedef struct ma_AAudioStream_t*        ma_AAudioStream;
 
-typedef ma_aaudio_data_callback_result_t (*ma_AAudioStream_dataCallback)(ma_AAudioStream* pStream, void* pUserData, void* pAudioData, int32_t numFrames);
+typedef ma_aaudio_data_callback_result_t (* ma_AAudioStream_dataCallback) (ma_AAudioStream* pStream, void* pUserData, void* pAudioData, int32_t numFrames);
+typedef void                             (* ma_AAudioStream_errorCallback)(ma_AAudioStream *pStream, void *pUserData, ma_aaudio_result_t error);
 
 typedef ma_aaudio_result_t       (* MA_PFN_AAudio_createStreamBuilder)                   (ma_AAudioStreamBuilder** ppBuilder);
 typedef ma_aaudio_result_t       (* MA_PFN_AAudioStreamBuilder_delete)                   (ma_AAudioStreamBuilder* pBuilder);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setDeviceId)              (ma_AAudioStreamBuilder* pBuilder, int32_t deviceId);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setDirection)             (ma_AAudioStreamBuilder* pBuilder, ma_aaudio_direction_t direction);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setSharingMode)           (ma_AAudioStreamBuilder* pBuilder, ma_aaudio_sharing_mode_t sharingMode);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setFormat)                (ma_AAudioStreamBuilder* pBuilder, ma_aaudio_format_t format);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setChannelCount)          (ma_AAudioStreamBuilder* pBuilder, int32_t channelCount);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setSampleRate)            (ma_AAudioStreamBuilder* pBuilder, int32_t sampleRate);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setBufferCapacityInFrames)(ma_AAudioStreamBuilder* pBuilder, int32_t numFrames);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setFramesPerDataCallback) (ma_AAudioStreamBuilder* pBuilder, int32_t numFrames);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setDataCallback)          (ma_AAudioStreamBuilder* pBuilder, ma_AAudioStream_dataCallback callback, void* pUserData);
+typedef void                     (* MA_PFN_AAudioStreamBuilder_setErrorCallback)         (ma_AAudioStreamBuilder* pBuilder, ma_AAudioStream_errorCallback callback, void* pUserData);
 typedef void                     (* MA_PFN_AAudioStreamBuilder_setPerformanceMode)       (ma_AAudioStreamBuilder* pBuilder, ma_aaudio_performance_mode_t mode);
 typedef ma_aaudio_result_t       (* MA_PFN_AAudioStreamBuilder_openStream)               (ma_AAudioStreamBuilder* pBuilder, ma_AAudioStream** ppStream);
 typedef ma_aaudio_result_t       (* MA_PFN_AAudioStream_close)                           (ma_AAudioStream* pStream);
 typedef ma_aaudio_stream_state_t (* MA_PFN_AAudioStream_getState)                        (ma_AAudioStream* pStream);
 typedef ma_aaudio_result_t       (* MA_PFN_AAudioStream_waitForStateChange)              (ma_AAudioStream* pStream, ma_aaudio_stream_state_t inputState, ma_aaudio_stream_state_t* pNextState, int64_t timeoutInNanoseconds);
 typedef ma_aaudio_format_t       (* MA_PFN_AAudioStream_getFormat)                       (ma_AAudioStream* pStream);
 typedef int32_t                  (* MA_PFN_AAudioStream_getChannelCount)                 (ma_AAudioStream* pStream);
@@ -23285,14 +23700,36 @@
         case MA_AAUDIO_OK: return MA_SUCCESS;
         default: break;
     }
 
     return MA_ERROR;
 }
 
+void ma_stream_error_callback__aaudio(ma_AAudioStream* pStream, void* pUserData, ma_aaudio_result_t error)
+{
+    ma_device* pDevice = (ma_device*)pUserData;
+    ma_assert(pDevice != NULL);
+
+    (void)error;
+
+#if defined(MA_DEBUG_OUTPUT)
+    printf("[AAudio] ERROR CALLBACK: error=%d, AAudioStream_getState()=%d\n", error, ((MA_PFN_AAudioStream_getState)pDevice->pContext->aaudio.AAudioStream_getState)(pStream));
+#endif
+
+    /*
+    From the documentation for AAudio, when a device is disconnected all we can do is stop it. However, we cannot stop it from the callback - we need
+    to do it from another thread. Therefore we are going to use an event thread for the AAudio backend to do this cleanly and safely.
+    */
+    if (((MA_PFN_AAudioStream_getState)pDevice->pContext->aaudio.AAudioStream_getState)(pStream) == MA_AAUDIO_STREAM_STATE_DISCONNECTED) {
+#if defined(MA_DEBUG_OUTPUT)
+        printf("[AAudio] Device Disconnected.\n");
+#endif
+    }
+}
+
 ma_aaudio_data_callback_result_t ma_stream_data_callback_capture__aaudio(ma_AAudioStream* pStream, void* pUserData, void* pAudioData, int32_t frameCount)
 {
     ma_device* pDevice = (ma_device*)pUserData;
     ma_assert(pDevice != NULL);
 
     if (pDevice->type == ma_device_type_duplex) {
         ma_device__handle_duplex_callback_capture(pDevice, frameCount, pAudioData, &pDevice->aaudio.duplexRB);
@@ -23378,14 +23815,16 @@
             ((MA_PFN_AAudioStreamBuilder_setDataCallback)pContext->aaudio.AAudioStreamBuilder_setDataCallback)(pBuilder, ma_stream_data_callback_playback__aaudio, (void*)pDevice);
         }
 
         /* Not sure how this affects things, but since there's a mapping between miniaudio's performance profiles and AAudio's performance modes, let go ahead and set it. */
         ((MA_PFN_AAudioStreamBuilder_setPerformanceMode)pContext->aaudio.AAudioStreamBuilder_setPerformanceMode)(pBuilder, (pConfig->performanceProfile == ma_performance_profile_low_latency) ? MA_AAUDIO_PERFORMANCE_MODE_LOW_LATENCY : MA_AAUDIO_PERFORMANCE_MODE_NONE);
     }
 
+    ((MA_PFN_AAudioStreamBuilder_setErrorCallback)pContext->aaudio.AAudioStreamBuilder_setErrorCallback)(pBuilder, ma_stream_error_callback__aaudio, (void*)pDevice);
+
     resultAA = ((MA_PFN_AAudioStreamBuilder_openStream)pContext->aaudio.AAudioStreamBuilder_openStream)(pBuilder, ppStream);
     if (resultAA != MA_AAUDIO_OK) {
         *ppStream = NULL;
         ((MA_PFN_AAudioStreamBuilder_delete)pContext->aaudio.AAudioStreamBuilder_delete)(pBuilder);
         return ma_result_from_aaudio(resultAA);
     }
 
@@ -23783,14 +24222,15 @@
     pContext->aaudio.AAudioStreamBuilder_setSharingMode            = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setSharingMode");
     pContext->aaudio.AAudioStreamBuilder_setFormat                 = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setFormat");
     pContext->aaudio.AAudioStreamBuilder_setChannelCount           = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setChannelCount");
     pContext->aaudio.AAudioStreamBuilder_setSampleRate             = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setSampleRate");
     pContext->aaudio.AAudioStreamBuilder_setBufferCapacityInFrames = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setBufferCapacityInFrames");
     pContext->aaudio.AAudioStreamBuilder_setFramesPerDataCallback  = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setFramesPerDataCallback");
     pContext->aaudio.AAudioStreamBuilder_setDataCallback           = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setDataCallback");
+    pContext->aaudio.AAudioStreamBuilder_setErrorCallback          = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setErrorCallback");
     pContext->aaudio.AAudioStreamBuilder_setPerformanceMode        = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_setPerformanceMode");
     pContext->aaudio.AAudioStreamBuilder_openStream                = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStreamBuilder_openStream");
     pContext->aaudio.AAudioStream_close                            = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStream_close");
     pContext->aaudio.AAudioStream_getState                         = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStream_getState");
     pContext->aaudio.AAudioStream_waitForStateChange               = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStream_waitForStateChange");
     pContext->aaudio.AAudioStream_getFormat                        = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStream_getFormat");
     pContext->aaudio.AAudioStream_getChannelCount                  = (ma_proc)ma_dlsym(pContext, pContext->aaudio.hAAudio, "AAudioStream_getChannelCount");
@@ -26273,15 +26713,15 @@
         ma_mutex_uninit(&pDevice->lock);
         return ma_context_post_error(pContext, NULL, MA_LOG_LEVEL_ERROR, "Failed to create worker thread stop event.", MA_FAILED_TO_CREATE_EVENT);
     }
 
 
     result = pContext->onDeviceInit(pContext, &config, pDevice);
     if (result != MA_SUCCESS) {
-        return MA_NO_BACKEND;  /* The error message will have been posted with ma_post_error() by the source of the error so don't bother calling it here. */
+        return result;
     }
 
     ma_device__post_init_setup(pDevice, pConfig->deviceType);
 
 
     /* If the backend did not fill out a name for the device, try a generic method. */
     if (pDevice->type == ma_device_type_capture || pDevice->type == ma_device_type_duplex) {
@@ -34650,21 +35090,14 @@
     if (result != MA_SUCCESS) {
         return result;
     }
 
     return ma_decoder_init_raw__internal(pConfigIn, &config, pDecoder);
 }
 
-#ifndef MA_NO_STDIO
-#include <stdio.h>
-#if !defined(_MSC_VER) && !defined(__DMC__)
-#include <strings.h>    /* For strcasecmp(). */
-#include <wchar.h>      /* For wcsrtombs() */
-#endif
-
 const char* ma_path_file_name(const char* path)
 {
     const char* fileName;
 
     if (path == NULL) {
         return NULL;
     }
@@ -34867,29 +35300,46 @@
     /* We need to manually set the user data so the calls to ma_decoder__on_seek_stdio() succeed. */
     pDecoder->pUserData = pFile;
 
     (void)pConfig;
     return MA_SUCCESS;
 }
 
+/*
+_wfopen() isn't always available in all compilation environments.
+
+    * Windows only.
+    * MSVC seems to support it universally as far back as VC6 from what I can tell (haven't checked further back).
+    * MinGW-64 (both 32- and 64-bit) seems to support it.
+    * MinGW wraps it in !defined(__STRICT_ANSI__).
+
+This can be reviewed as compatibility issues arise. The preference is to use _wfopen_s() and _wfopen() as opposed to the wcsrtombs()
+fallback, so if you notice your compiler not detecting this properly I'm happy to look at adding support.
+*/
+#if defined(_WIN32)
+    #if defined(_MSC_VER) || defined(__MINGW64__) || !defined(__STRICT_ANSI__)
+        #define MA_HAS_WFOPEN
+    #endif
+#endif
+
 ma_result ma_decoder__preinit_file_w(const wchar_t* pFilePath, const ma_decoder_config* pConfig, ma_decoder* pDecoder)
 {
     FILE* pFile;
 
     if (pDecoder == NULL) {
         return MA_INVALID_ARGS;
     }
 
     ma_zero_object(pDecoder);
 
     if (pFilePath == NULL || pFilePath[0] == '\0') {
         return MA_INVALID_ARGS;
     }
 
-#if defined(_WIN32)
+#if defined(MA_HAS_WFOPEN)
     /* Use _wfopen() on Windows. */
     #if defined(_MSC_VER) && _MSC_VER >= 1400
         if (_wfopen_s(&pFile, pFilePath, L"rb") != 0) {
             return MA_ERROR;
         }
     #else
         pFile = _wfopen(pFilePath, L"rb");
@@ -35400,14 +35850,23 @@
   - bufferSizeInFrames
   - periods
 */
 
 /*
 REVISION HISTORY
 ================
+v0.9.9 - 2020-01-09
+  - Fix compilation errors with MinGW.
+  - Fix compilation errors when compiling on Apple platforms.
+  - WASAPI: Add support for disabling hardware offloading.
+  - WASAPI: Add support for disabling automatic stream routing.
+  - Core Audio: Fix bugs in the case where the internal device uses deinterleaved buffers.
+  - Core Audio: Add support for controlling the session category (AVAudioSessionCategory) and options (AVAudioSessionCategoryOptions).
+  - JACK: Fix bug where incorrect ports are connected.
+
 v0.9.8 - 2019-10-07
   - WASAPI: Fix a potential deadlock when starting a full-duplex device.
   - WASAPI: Enable automatic resampling by default. Disable with config.wasapi.noAutoConvertSRC.
   - Core Audio: Fix bugs with automatic stream routing.
   - Add support for controlling whether or not the content of the output buffer passed in to the data callback is pre-initialized
     to zero. By default it will be initialized to zero, but this can be changed by setting noPreZeroedOutputBuffer in the device
     config. Setting noPreZeroedOutputBuffer to true will leave the contents undefined.
@@ -35789,15 +36248,15 @@
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <http://unlicense.org/>
 
 ===============================================================================
 ALTERNATIVE 2 - MIT No Attribution
 ===============================================================================
-Copyright 2019 David Reid
+Copyright 2020 David Reid
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so.
```

### Comparing `miniaudio-1.8/miniaudio/stb_vorbis.c` & `miniaudio-1.9/miniaudio/stb_vorbis.c`

 * *Files identical despite different names*

### Comparing `miniaudio-1.8/miniaudio.c` & `miniaudio-1.9/miniaudio.c`

 * *Files identical despite different names*

### Comparing `miniaudio-1.8/miniaudio.egg-info/PKG-INFO` & `miniaudio-1.9/miniaudio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniaudio
-Version: 1.8
+Version: 1.9
 Summary: python bindings for the miniaudio library and its decoders (mp3, flac, ogg vorbis, wav)
 Home-page: https://github.com/irmen/pyminiaudio
 Author: Irmen de Jong
 Author-email: irmen@razorvine.net
 License: MIT
 Description: [![saythanks](https://img.shields.io/badge/say-thanks-ff69b4.svg)](https://saythanks.io/to/irmen)
         [![Latest Version](https://img.shields.io/pypi/v/miniaudio.svg)](https://pypi.python.org/pypi/miniaudio/)
```

### Comparing `miniaudio-1.8/miniaudio.py` & `miniaudio-1.9/miniaudio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Python interface to the miniaudio library (https://github.com/dr-soft/miniaudio)
 
 Author: Irmen de Jong (irmen@razorvine.net)
 Software license: "MIT software license". See http://opensource.org/licenses/MIT
 """
 
-__version__ = "1.8"
+__version__ = "1.9"
 
 
 import abc
 import sys
 import os
 import io
 import array
```

### Comparing `miniaudio-1.8/setup.cfg` & `miniaudio-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `miniaudio-1.8/setup.py` & `miniaudio-1.9/setup.py`

 * *Files identical despite different names*

