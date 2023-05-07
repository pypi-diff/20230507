# Comparing `tmp/gums-0.0.27.tar.gz` & `tmp/gums-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gums-0.0.27.tar", last modified: Fri Mar 17 02:27:32 2023, max compression
+gzip compressed data, was "gums-0.0.29.tar", last modified: Sun May  7 16:09:45 2023, max compression
```

## Comparing `gums-0.0.27.tar` & `gums-0.0.29.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-17 02:27:32.395275 gums-0.0.27/
--rw-r--r--   0 a         (1000) a         (1000)     3801 2023-03-17 02:27:32.395275 gums-0.0.27/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     3251 2023-03-17 02:26:37.000000 gums-0.0.27/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-17 02:27:32.395275 gums-0.0.27/bin/
--rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:33:17.000000 gums-0.0.27/bin/gumc
--rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:34:40.000000 gums-0.0.27/bin/gumd
--rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:33:17.000000 gums-0.0.27/bin/gums
--rw-r--r--   0 a         (1000) a         (1000)     2132 2023-03-17 02:25:51.000000 gums-0.0.27/gumc.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-03-17 02:27:32.395275 gums-0.0.27/gums.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)     3801 2023-03-17 02:27:32.000000 gums-0.0.27/gums.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      200 2023-03-17 02:27:32.000000 gums-0.0.27/gums.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-03-17 02:27:32.000000 gums-0.0.27/gums.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       19 2023-03-17 02:27:32.000000 gums-0.0.27/gums.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       15 2023-03-17 02:27:32.000000 gums-0.0.27/gums.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     4525 2023-03-17 02:27:27.000000 gums-0.0.27/gums.py
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-03-17 02:27:32.395275 gums-0.0.27/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)      923 2023-03-15 18:33:17.000000 gums-0.0.27/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-07 16:09:45.746473 gums-0.0.29/
+-rw-r--r--   0 a         (1000) a         (1000)     3801 2023-05-07 16:09:45.746473 gums-0.0.29/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     3251 2023-03-17 02:26:37.000000 gums-0.0.29/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-07 16:09:45.746473 gums-0.0.29/bin/
+-rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:33:17.000000 gums-0.0.29/bin/gumc
+-rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:34:40.000000 gums-0.0.29/bin/gumd
+-rw-r--r--   0 a         (1000) a         (1000)       54 2023-03-15 18:33:17.000000 gums-0.0.29/bin/gums
+-rw-r--r--   0 a         (1000) a         (1000)     2394 2023-03-19 20:40:45.000000 gums-0.0.29/gumc.py
+-rw-r--r--   0 a         (1000) a         (1000)   363832 2023-05-07 16:07:44.000000 gums-0.0.29/gums.c
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-07 16:09:45.746473 gums-0.0.29/gums.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     3801 2023-05-07 16:09:45.000000 gums-0.0.29/gums.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      207 2023-05-07 16:09:45.000000 gums-0.0.29/gums.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-07 16:09:45.000000 gums-0.0.29/gums.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       19 2023-05-07 16:09:45.000000 gums-0.0.29/gums.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       15 2023-05-07 16:09:45.000000 gums-0.0.29/gums.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     4906 2023-05-07 16:01:23.000000 gums-0.0.29/gums.py
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-07 16:09:45.746473 gums-0.0.29/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)      924 2023-05-07 16:09:34.000000 gums-0.0.29/setup.py
```

### Comparing `gums-0.0.27/PKG-INFO` & `gums-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gums
-Version: 0.0.27
+Version: 0.0.29
 Summary: gums, Grande Unicast Multicast Sender
 Home-page: https://github.com/futzu/gums
 Author: Adrian
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gums-0.0.27/README.md` & `gums-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `gums-0.0.27/gumc.py` & `gums-0.0.29/gumc.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,21 @@
     parser.add_argument(
         "-i",
         "--instuff",
         default='udp://@235.35.3.5:3535',
         help="""default is 'udp://@235.35.3.5:3535'
                                 """,
     )
+    
+    parser.add_argument(
+        "-o",
+        "--outstuff",
+        default='out.ts',
+        help="""default is 'out.ts'""",
+    )
 
     parser.add_argument(
         "-b",
         "--bytesize",
         default=1,
         type=int,
         help="Number of bytes to read. default is 1",
@@ -97,21 +104,24 @@
 
     optional arguments:
       -h, --help            show this help message and exit
       -i INSTUFF, --instuff INSTUFF
                             default is 'udp://@235.35.3.5:3535'
       -b BYTESIZE, --bytesize BYTESIZE
                             Number of bytes to read. default is 1
-
       -v, --version         Show version
 
     """
     args = parse_args()
     if args.version:
         print(version())
         sys.exit()
     gumc =GumC(args.instuff)
-    print(gumc.read(args.bytesize))
+    b= gumc.read(args.bytesize)
+    print(len(b))
+    with open(args.outstuff,"wb") as stuffout:
+            stuffout.write(b)
+            #outstuff.write(data)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `gums-0.0.27/gums.egg-info/PKG-INFO` & `gums-0.0.29/gums.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gums
-Version: 0.0.27
+Version: 0.0.29
 Summary: gums, Grande Unicast Multicast Sender
 Home-page: https://github.com/futzu/gums
 Author: Adrian
 Author-email: spam@iodisco.com
 Platform: all
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gums-0.0.27/gums.py` & `gums-0.0.29/gums.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 
 """
 import argparse
 import os
 import socket
 import sys
+import time
 from functools import partial
 from new_reader import reader
 
 
 DGRAM_SIZE = 1316
 
 DEFAULT_MULTICAST = "235.35.3.5:3535"
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "27"
+MAINTAINENCE = "29"
 
 
 def version():
     """
     version prints version as a string
 
     """
@@ -67,20 +68,29 @@
         return sock
 
     def iter_dgrams(self, vid):
         """
         iter_dgrams iterates over the video and sends
         self.dgram_size chunks of video to the socket.
         """
-        total_bytes=0
+        million = 1024 * 1024
+        start_time = time.time()
+        now = time.time
+        total_bytes = 0
         with reader(vid) as gum:
             for dgram in iter(partial(gum.read, DGRAM_SIZE), b""):
                 self.sock.sendto(dgram, self.dest_grp)
-                total_bytes+=len(dgram)
-                print(f"\r{total_bytes} Bytes Sent",end="\r",file=sys.stderr)
+                total_bytes += len(dgram)
+                elapsed = now() - start_time
+                rate = (total_bytes / million) / elapsed
+                print(
+                    f"\t{total_bytes/million:0.2f} MB sent in {elapsed:5.2f} seconds. {rate:3.2f} MB/Sec",
+                    end="\r",
+                    file=sys.stderr,
+                )
             print("\n", file=sys.stderr)
 
     def send_stream(self, vid):
         """
         send_stream sets multicast ttl if needed,
         prints socket address info,
         calls self.iter_dgrams,
@@ -89,16 +99,19 @@
         proto = "udp://"
         pre = "Unicast"
         if self.is_multicast():
             self.sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, self.ttl)
             proto = proto + "@"
             pre = "Multicast"
         src_ip, src_port = self.sock.getsockname()
-        print(f"\n\t{pre} Stream\n\t{proto}{self.dest_ip}:{self.dest_port}",file=sys.stderr)
-        print(f"\n\tSource\n\t{src_ip}:{src_port}\n",file=sys.stderr)
+        print(
+            f"\n\t{pre} Stream\n\t{proto}{self.dest_ip}:{self.dest_port}",
+            file=sys.stderr,
+        )
+        print(f"\n\tSource\n\t{src_ip}:{src_port}\n", file=sys.stderr)
 
         self.iter_dgrams(vid)
         self.sock.close()
 
 
 def parse_args():
     """
@@ -186,15 +199,15 @@
 
     """
 
     args = parse_args()
     if args.version:
         print(version())
         sys.exit()
-  #  daemonize()
+    #  daemonize()
     ttl = int(args.ttl).to_bytes(1, byteorder="big")
     dest_addr = args.addr
     gummie = GumS(dest_addr, ttl, args.bind_addr)
     gummie.send_stream(args.input)
     sys.exit()
```

### Comparing `gums-0.0.27/setup.py` & `gums-0.0.29/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import setuptools
 import gums
 
+
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="gums",
     version=gums.version(),
     author="Adrian",
```

