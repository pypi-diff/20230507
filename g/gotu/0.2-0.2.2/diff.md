# Comparing `tmp/gotu-0.2-py3-none-any.whl.zip` & `tmp/gotu-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 30614 bytes, number of entries: 18
+Zip file size: 32404 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx      451 b- defN 22-Jun-04 19:09 gotu/__init__.py
+-rw-rw-r--  2.0 unx     3300 b- defN 23-May-07 20:39 gotu/aidss.py
 -rw-rw-r--  2.0 unx     1906 b- defN 22-Jun-04 19:09 gotu/bb.py
 -rw-rw-r--  2.0 unx     2067 b- defN 22-Jun-04 19:09 gotu/binary.py
 -rw-rw-r--  2.0 unx    16834 b- defN 22-Dec-31 15:48 gotu/dss.py
 -rw-rw-r--  2.0 unx     1240 b- defN 22-Jun-04 19:09 gotu/events.py
 -rw-rw-r--  2.0 unx     9051 b- defN 22-Dec-31 15:48 gotu/gaia.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Jun-04 19:09 gotu/grb.py
--rw-rw-r--  2.0 unx    12715 b- defN 22-Dec-31 15:48 gotu/jwst.py
--rw-rw-r--  2.0 unx      554 b- defN 22-Jun-04 19:09 gotu/quasar.py
+-rw-rw-r--  2.0 unx    13172 b- defN 23-May-07 20:39 gotu/jwst.py
+-rw-rw-r--  2.0 unx      825 b- defN 23-May-07 20:39 gotu/quasar.py
 -rw-rw-r--  2.0 unx      195 b- defN 22-Jun-04 19:09 gotu/relativity.py
--rw-rw-r--  2.0 unx    19804 b- defN 22-Dec-31 15:48 gotu/spiral.py
+-rw-rw-r--  2.0 unx    19796 b- defN 23-May-07 20:39 gotu/spiral.py
 -rw-rw-r--  2.0 unx      421 b- defN 22-Jun-04 19:09 gotu/triangle.py
 -rw-rw-r--  2.0 unx     6425 b- defN 22-Dec-31 15:48 gotu/wits.py
--rw-rw-r--  2.0 unx      849 b- defN 22-Dec-31 15:55 gotu-0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Dec-31 15:55 gotu-0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       49 b- defN 22-Dec-31 15:55 gotu-0.2.dist-info/dependency_links.txt
--rw-rw-r--  2.0 unx        5 b- defN 22-Dec-31 15:55 gotu-0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1281 b- defN 22-Dec-31 15:55 gotu-0.2.dist-info/RECORD
-18 files, 73939 bytes uncompressed, 28582 bytes compressed:  61.3%
+-rw-rw-r--  2.0 unx      851 b- defN 23-May-07 20:39 gotu-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-07 20:39 gotu-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 23-May-07 20:39 gotu-0.2.2.dist-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-May-07 20:39 gotu-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1361 b- defN 23-May-07 20:39 gotu-0.2.2.dist-info/RECORD
+19 files, 78041 bytes uncompressed, 30250 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: gotu/__init__.py
 Comment: 
 
+Filename: gotu/aidss.py
+Comment: 
+
 Filename: gotu/bb.py
 Comment: 
 
 Filename: gotu/binary.py
 Comment: 
 
 Filename: gotu/dss.py
@@ -33,23 +36,23 @@
 
 Filename: gotu/triangle.py
 Comment: 
 
 Filename: gotu/wits.py
 Comment: 
 
-Filename: gotu-0.2.dist-info/METADATA
+Filename: gotu-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: gotu-0.2.dist-info/WHEEL
+Filename: gotu-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: gotu-0.2.dist-info/dependency_links.txt
+Filename: gotu-0.2.2.dist-info/dependency_links.txt
 Comment: 
 
-Filename: gotu-0.2.dist-info/top_level.txt
+Filename: gotu-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gotu-0.2.dist-info/RECORD
+Filename: gotu-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gotu/jwst.py

```diff
@@ -74,19 +74,20 @@
 The key number is *z* and is the ratio of the wavelenth we observe to
 what it was at the origin.
 
 There are many reports of many z>=10 in the first images.  There has
 also been some recalibration of the instrument that has generally
 reduced the red shifts observed.
 
+
 """
 
 #from astroquery.mast import Observations
 #from astroquery.simbad import Simbad
-
+import asyncio
 from astropy.table import Table
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 from glob import glob
 
 import random
@@ -102,17 +103,14 @@
 
 # make things pretty 
 from pprint import pprint
 
 import PIL.Image
 PIL.Image.MAX_IMAGE_PIXELS = None
 
-#CORS_PROXY = "https://cors-anywhere.herokuapp.com/"
-CORS_PROXY = "http://localhost:8080/"
-
 MAST_URL = "https://mast.stsci.edu/api/v0/invoke?request="
 MAST_DOWNLOAD = "https://mast.stsci.edu/api/v0.1/Download/file?uri="
 
 
 def query_region(skypos, project='JWST'):
 
     request = {'service':'Mast.Caom.Cone',
@@ -134,15 +132,14 @@
     response = mast_query(request)
     
     return response_to_table(response)
 
 def response_to_table(response):
     
     content = response_to_json(response)
-    print(content)
 
     fields = content['fields']
     names = [x['name'] for x in fields]
     dtype = [x['type'] for x in fields]
 
     typemap = dict(string=str,
                    boolean=bool)
@@ -184,15 +181,14 @@
 
     return result
 
     
 
 def open_file(uri):
 
-    target = f'{CORS_PROXY}{MAST_DOWNLOAD}{uri}'
     target = f'{MAST_DOWNLOAD}{uri}'
     print(target)
     result = requests.get(target)
 
     if result.status_code != 200:
         print('STATUS', result)
         raise IOError()
@@ -229,26 +225,28 @@
             'SMACS 0723',  #  deep field?
             'NGC 7318B',   # Stephen's Quintet?
             'M 74',       # NGC 628 Phantom Galaxy
             'NGC 3324',   # Carina Nebula
             'PGC 2248'))  # Cartwheel
 
         self.project = 'JWST'
-        self.project = None
+        self.i2d = False
 
         self.topn = 1
         self.do_product_list = False
         self.maxrows = 15
 
     async def show_stats(self, table):
 
         msg = self.table_count(table)
         print(table.colnames)
-        print('TABLELEN', len(table))
-        await self.put(msg, 'help')
+        if len(table) != 0:
+            await self.put(msg, 'help')
+        else:
+            await self.put([['no data'], ['for'], [self.locations[0]]], 'help')
         
     def table_count(self, table, maxrows=None):
         """ Do some counts on a table 
         
         pretty sure there is some sort of table.info.stats()
         """
         msg = []
@@ -270,61 +268,70 @@
 
         return msg
 
     def name_to_skycoord(self, name):
 
         return object_lookup(name)
 
-    async def get_observations(self, skypos):
+    async def get_observations(self, skypos, name='unknown'):
 
-        filename = Path(f'skypos_{skypos.ra.deg}_{skypos.dec.deg}.fits')
+        if self.project:
+            filename = Path(f'skypos_{name}_{self.project}_{skypos.ra.deg}_{skypos.dec.deg}.fits')
+        else:
+            filename = Path(f'skypos_{name}_{skypos.ra.deg}_{skypos.dec.deg}.fits')
         if filename.exists():
             results = Table.read(filename)
         else:
             print('querying mast database')
-            results = query_region(skypos)
+            #loop = asyncio.get_event_loop()
+            results = query_region(skypos, self.project)
+            #results = loop.run_in_executor(
+            #    query_region, (skypos, self.project))
             #results = Observations.query_region(skypos)
             # find the JWST ones
             if self.project:
                 mask = results['project'] == self.project
         
                 results = results[mask]
 
             await self.show_stats(results)
-            results.info()
-            results.info('stats')
+
+            #results.info()
+            #results.info('stats')
                   
             
             # save a copy of the results
             results.write(filename)
 
-        # Fileter some more -- need to make this optional
-        mask = [Path(x['dataURL']).stem.endswith('i2d') for x in results]
-        results = results[mask]
+        # Filter some more -- need to make this optional
+        if self.i2d:
+            mask = [Path(x['dataURL']).stem.endswith('i2d') for x in results]
+
+            results = results[mask]
 
         await self.show_stats(results)
 
         return results
             
     async def start(self):
 
-        skypos = self.name_to_skycoord(self.locations[0])
-        print(self.locations[0], skypos)
+        name = self.locations[0]
+        skypos = self.name_to_skycoord(name)
+        print(name, skypos)
 
         # get observations
-        results = await self.get_observations(skypos)
+        results = await self.get_observations(skypos, name=name)
 
         print('Region size:', len(results))
         names = list(results.colnames)
         products = {}
         counters = defaultdict(Counter)
 
         for x in results:
 
-            if 'JWST' in x['dataURL']:
                 print(x['dataURL'])
                 products[x['dataURL']] = x
                          
                 if self.do_product_list:
                     plist = Observations.get_product_list(x)
                     print("JJJJJJJ", len(plist))
                     for product in plist:
@@ -332,17 +339,17 @@
                         for name in product.colnames:
                             counters[name].update([str(product[name])])
                          
 
                     products[product['dataURI']] = product
                          
 
-                for key, counts in counters.items():
-                    print(key)
-                    print(counts.most_common(3))
+                #for key, counts in counters.items():
+                #    print(key)
+                #    print(counts.most_common(3))
             
         self.products = products
         self.locations.rotate()
 
     async def run(self):
                          
 
@@ -366,20 +373,14 @@
         for key in ('jpegURL',):
             
             if key not in prod.colnames:
                 continue
 
             filename = Path(prod[key])
 
-            print(filename)
-            if not filename.stem.endswith('i2d'):
-                print('skipping', filename)
-                print()
-                continue
-            
             if filename.suffix not in filetypes:
                 print('filtered out by filetype ', filename.suffix, filename)
                 if product in self.products:
                     del self.products[product]
                 continue
             
             result = download_file(str(filename))
@@ -395,15 +396,15 @@
                     print(item.size)
                 if isinstance(item.size, int):
                     print('Array size:', item.size)
                 elif item.size:
                     #await self.show_stats(item)
                     pass
                 
-                print(tab.info())
+                #print(tab.info())
 
             elif filename.suffix == '.jpg' or filename.suffix == '.png':
                 ax = await self.get()
                 ax.imshow(image.imread(filename.name),
                           cmap=modnar.random_colour())
                 ax.show()
 
@@ -419,24 +420,35 @@
 if __name__ == '__main__':
 
     from blume import magic, farm
     import argparse
     
     parser = argparse.ArgumentParser()
     parser.add_argument('--location')
+    parser.add_argument('--survey')
+    parser.add_argument('--size', type=int)
     parser.add_argument('--project', default=None)
-    parser.add_argument('--corsproxy')
+    parser.add_argument('--i2d', action='store_true')
 
     args = parser.parse_args()
 
     fm = farm.Farm()
 
     jwst = Jwst()
     if args.location:
         jwst.locations.appendleft(args.location)
 
-    if args.corsproxy:
-        CORS_PROXY = args.corsproxy
+    if args.project:
+        jwst.project = args.project
+
+    if args.survey:
+        jwst.locations.clear()
+        locations = [args.survey + str(int(x)) for x in range(1, args.size+1)]
+        random.shuffle(locations)
+        for location in locations:
+            jwst.locations.append(location)
+
+    jwst.i2d = args.i2d
         
     fm.add(jwst)
     magic.run(farm.start_and_run(fm))
```

## gotu/quasar.py

```diff
@@ -1,9 +1,8 @@
-"""
-=======================================================================
+"""=======================================================================
  What would light emerging at the event horizon of a quasar look like?
 =======================================================================
 
 For now that is the goal for this module, what should a quasar look like?
 
 With all fingers crossed for the `JWST`_, I think we are about to be
 surprised at how ubiquitous quasars are.
@@ -15,8 +14,16 @@
 
 In a place where the passage of time is close to zero, but not actually, zero.
 
 
 JWST
 ====
 
+The model for quasars outlined in `gotu`_ requires just two parameters.
+
+The central mass and the temperature and density of matter around the
+Eddington sphere of the quasar's black hole.
+
+There is a huge range of possible redshifts, depending on these two
+parameters.  
+
 """
```

## gotu/spiral.py

```diff
@@ -352,42 +352,42 @@
 
         self.print_parms()
         print()
 
     def sun(self):
 
         print('SUN!' * 10)
-        solar_mass = 1 * units.solMass
+        solar_mass = 1 * u.solMass
         solar_angular_velocity = (365/27) * 2 * math.pi  # radians per year
         
         # Central mass.  Mass converted to Schwartzschild radius (in light years)
         # Mass of 1 is approximately 3e12 solar masses.
         self.Mcent = solar_mass
         self.Mball = 0.
         self.Mdisc = 0.
         self.omega0 = solar_angular_velocity
 
         # astronomical unit in light years
         # au = 1 / 63241.08  ### can't remember how I calculated this
-        au = units.au
+        au = u.au
         
         self.rmin = 0.1 * au
         self.rmax = 50 * au
 
         self.K = self.Mcent
 
         # solar wind goes from 30 km/s at 3 AU to 500 km/s at 40 AU
         # so set A to 2 * 500 km/s in our units
         # ??
 
         # A = K * \omega_0.  K = M for Sciama principle
         self.A = self.K * solar_angular_velocity
 
         # magic constant determined by overall energy in the orbit
-        self.EE = 0.0
+        self.EE = 0.1
 
 
         # constant, can be read from tangential velocity for small r
         self.find_cc(tangential_velocity=self.rmin * self.omega0)
         #self.CC = -0.1
 
         # Apparent rate of precession of the roots of the spiral.
```

## Comparing `gotu-0.2.dist-info/METADATA` & `gotu-0.2.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotu
-Version: 0.2
+Version: 0.2.2
 Summary: The Geometry of the Universe
 Home-page: https://github.com/swfiua/gotu
 Author: Johnny Gill
 Author-email: swfiua@gmail.com
 License: GPL 3
 Keywords: astropy cosmology
 Platform: UNKNOWN
```

## Comparing `gotu-0.2.dist-info/RECORD` & `gotu-0.2.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 gotu/__init__.py,sha256=Ur2pdtD4YPI1cRxyY2lFTIRJNyN-IF9TQYV6rQgANYE,451
+gotu/aidss.py,sha256=UNITXth1HXjTLvhUW8e-xH7l8JC24ryrP00Uo_jgWoA,3300
 gotu/bb.py,sha256=wKjNjJyMGUz33G2crNKv7simcgeoUVTRbdSNO4Oork8,1906
 gotu/binary.py,sha256=rNUtu50mW-ZJ40vWJXW0Sh8ZVlFuc9rM68_8e64MeOU,2067
 gotu/dss.py,sha256=-60HJzf0fLdzsb2pEUkrc3P50ocuefrSNDVH9-yuVmk,16834
 gotu/events.py,sha256=YhNUFmkfRJoMYykvpSD5DnWAZZQ4ijr89L5uKz0A-ZY,1240
 gotu/gaia.py,sha256=aI4_4DmyKfNFKSZO0wU31iUMvkS85wai0yuKPWIVlBc,9051
 gotu/grb.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gotu/jwst.py,sha256=loRIDhzOboA0MgJK8Gu_5GM0bv3o-BjP3zsUOlna-3Q,12715
-gotu/quasar.py,sha256=HfL2F08G8GygnC2SpCfkSv2HfdLYzXGYtaDP6a-5g3M,554
+gotu/jwst.py,sha256=CaihCxpP1dQYziZmHLTCkCHoWri-Bxe5XUVNJyo4IYM,13172
+gotu/quasar.py,sha256=Lc7xY_d8ObdN5dYcOmWjbhSoowUXno28RsySBFn-u48,825
 gotu/relativity.py,sha256=hE4x1J3deptfOb5zvygs_Efx_5FjowO19l7F8V26prg,195
-gotu/spiral.py,sha256=zgcC0hZu-RUWG0iRqk19NRhJ0hMp8XhCD4J7uxPZTF0,19804
+gotu/spiral.py,sha256=-KTbdcMUTkGRVy59Fj-iLV2Vtf4Vj6hxq2zdReiXDQE,19796
 gotu/triangle.py,sha256=DHJ0BUEwnmZIviocSEmvca6tTKl9hC9mNPQS-CBJUXY,421
 gotu/wits.py,sha256=Rg3WM1LUxokyF8Y7x8RisPoZQ9rSdAYbY5uJvtVpKh0,6425
-gotu-0.2.dist-info/METADATA,sha256=OU_YahyjYhX2-VO0LNARDwEO0fgjwczeT6Th5ZV7td8,849
-gotu-0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-gotu-0.2.dist-info/dependency_links.txt,sha256=wsLZ7ZMSuUKKEBe7UoWXGovFO0DYePnQJHSgXhH78Io,49
-gotu-0.2.dist-info/top_level.txt,sha256=UmCQ_GxPnOlWVxkBinmWYiS_7dOmazT636F3OoCc3hs,5
-gotu-0.2.dist-info/RECORD,,
+gotu-0.2.2.dist-info/METADATA,sha256=ycCmNVW7MEi5GGZRqTC42LMlS_Ov1BvXft1rvgoGuXs,851
+gotu-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+gotu-0.2.2.dist-info/dependency_links.txt,sha256=wsLZ7ZMSuUKKEBe7UoWXGovFO0DYePnQJHSgXhH78Io,49
+gotu-0.2.2.dist-info/top_level.txt,sha256=UmCQ_GxPnOlWVxkBinmWYiS_7dOmazT636F3OoCc3hs,5
+gotu-0.2.2.dist-info/RECORD,,
```

