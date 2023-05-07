# Comparing `tmp/scoobi-0.0.1.4.tar.gz` & `tmp/scoobi-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoobi-0.0.1.4.tar", last modified: Wed May  3 18:09:20 2023, max compression
+gzip compressed data, was "scoobi-0.0.1.5.tar", last modified: Sun May  7 20:36:40 2023, max compression
```

## Comparing `scoobi-0.0.1.4.tar` & `scoobi-0.0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:09:20.817927 scoobi-0.0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 18:09:04.000000 scoobi-0.0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-03 18:09:20.817927 scoobi-0.0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-03 18:09:04.000000 scoobi-0.0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 18:09:20.817927 scoobi-0.0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-03 18:09:04.000000 scoobi-0.0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:09:20.813927 scoobi-0.0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:09:20.813927 scoobi-0.0.1.4/src/scoobi/
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-05-03 18:09:04.000000 scoobi-0.0.1.4/src/scoobi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-03 18:09:04.000000 scoobi-0.0.1.4/src/scoobi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:09:20.817927 scoobi-0.0.1.4/src/scoobi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:09:20.000000 scoobi-0.0.1.4/src/scoobi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.505818 scoobi-0.0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/src/scoobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/src/scoobi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-07 20:36:27.000000 scoobi-0.0.1.5/src/scoobi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:36:40.509817 scoobi-0.0.1.5/src/scoobi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 20:36:40.000000 scoobi-0.0.1.5/src/scoobi.egg-info/top_level.txt
```

### Comparing `scoobi-0.0.1.4/LICENSE` & `scoobi-0.0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.4/PKG-INFO` & `scoobi-0.0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `scoobi-0.0.1.4/README.md` & `scoobi-0.0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scoobi-0.0.1.4/setup.py` & `scoobi-0.0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'scoobi',
-    version = '0.0.1.4',
+    version = '0.0.1.5',
     url='https://github.com/avialxee/scoobi',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Solar Conventionality-based Organizing Observation data ( SCOOBI )',
     py_modules = ["scoobi"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
```

### Comparing `scoobi-0.0.1.4/src/scoobi/__init__.py` & `scoobi-0.0.1.5/src/scoobi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,66 +71,135 @@
     with fits.open(fitsfile, 'update') as f:
         for hdu in f:
             hdu.header.update(header_params)
             hdu.header['FILENAME'] = tifpath.name
 
 def build_foldername(fitsname, **kwargs):
     """
-    Builds folder name taking input of the fitsfile name
+    Builds folder name taking input of the fitsfile name i.e
+    destfolder + 
 
     *Parameters*
     
     :fitsname: 
         (str) (Required)
 
         This is the conventional name of the fitsfile which will be used to build the folder path.
         Ex. S-2022-11-01T02:02:20.001-HA.fits
 
     :destfolder: 
-        (str) (Optional) (Default:None) (Superseeds final)
+        (str) (Optional) (Default:None)
 
         The destination folder name where all the files will get saved.
 
     *Return*
     
-        (str) folder name for the fits file.
+        (str) complete path for the fitsfile.
 
     """
     params={'destfolder': 'processed/',
     }
     params.update(kwargs)
         
     dcf=fitsname.split('-')
     dcf_date=dcf[3].split('T')[0]
     #currentfolder=f'{params["rootfolder"]}{params["destfolder"]}{dcf[1]}/{dcf[1]}{dcf[2]}{dcf_date}/'
     currentfolder=f'{params["destfolder"]}/{dcf[1]}/{dcf[2]}/{dcf_date}/'
     if not Path(currentfolder).exists():
         Path(currentfolder).mkdir(parents=True,exist_ok=True)
     return f'{currentfolder}{fitsname}'
         
+def fits_to_fits(fitsfile_i, header=None, **kwargs):
+    """
+    *Parameters*
+    
+    :fitsfile_i:
+        (str) (Required)
+
+        Full path of the RAW FITS file as input. This is a 3D FITS file.
+
+    :header:
+        (dict) (Optional)
+
+        If provided, it will use headers from FITS as well the supplied parameters to write to FITS.
+    
+    *kwargs*
+
+    :fitsname: 
+        (str) (Optional) (Default=None)
+
+        This is the conventional name of the fitsfile which will be used to build the folder path.
+        If not provided will build name according to the timestamp in the FITS header.
+        Ex. S-2022-11-01T02:02:20.001-HA.fits
+    
+    :initial:
+        (str) (Optional) (Default='S')
+        Convential initial for the type of file in the output filename e.g
+        - S: Science
+        - F: Flat
+        - D: Dark
+
+    :destfolder: 
+        (str) (Optional) (Default:see build_foldername())
+
+        The destination folder name where all the files will get saved.
+
+    :telescope:
+        (str) (Optional) (Default:HA)
+        The Telescope name is used to create the header info and filename
+    """
+    params={'fitsname':None, 'telescope':'HA', 'initial':'S'}
+    params.update(kwargs)
+    fitsfile_o=None
+    
+    if header:
+        pass
+    print(f'{fitsfile_i}')
+    with fits.open(fitsfile_i, 'readonly',) as hdul:
+        if len(hdul[0].data.shape)==3:hdul[0].data=hdul[0].data[0]
+        date=hdul[0].header['DATE-OBS']
+        for hdu in hdul:
+            hdu.header.update(header)
+            hdu.header['TELESCOP']=params['telescope']
+            hdu.header['FILENAME']=Path(fitsfile_i).name
+            
+        if params['fitsname'] is None:
+            # name convention : *S + DATETIME + TELESCOPE*
+            fitsfile_o=f"{params['initial']}-{date}-{params['telescope']}.fits"
+            fitsfile_o=build_foldername(fitsfile_o, **kwargs)
+        else:
+            fitsfile_o=build_foldername(params['fitsname'])
+        hdul.writeto(fitsfile_o, overwrite=True)
+    return fitsfile_o
+    # data,hdrdata=scidata[0][0], scidata[1] # taking data[0] as data is 3D
+    
 def tif_to_fits(tiffile, magick=True, header=None, **kwargs):
     """
     *Parameters*
     
     :tiffile:
         (str) (Required)
 
-        Full path of the TIFF ile that needs to be converted to FITS.
+        Full path of the TIFF file that needs to be converted to FITS.
 
     :magick:
         (boolean) (Optional)
 
         If true will execute convert utility of ImageMagick to convert from tiff to fits (faster)
         Else the python way of conversion will be used.
 
     :header:
         (dict) (Optional)
 
         If provided, it will use headers from TIFF as well the supplied parameters to write to FITS.
     
+    :telescope:
+        (str) (Optional) (Default:HA)
+        The Telescope name is used to create the header info and filename
+
     kwargs
     ------
 
     :fitsname: 
         (str) (Optional) (Default=None)
 
         This is the conventional name of the fitsfile which will be used to build the folder path.
@@ -173,21 +242,50 @@
     """
     Creates thumbnails for the fits file provided in the fits_folder path.
     """
     if fits_folder:
         allfile=search_file(f"{fits_folder}/",'.fits', recursive=True)
         
         for fitsfile in allfile:
-            if not out_folder:out_folder=Path(fitsfile).parent
+            print(f"{fitsfile} is read")
+            out_folder=Path(fitsfile).parent
             jpgfolder=f"{out_folder}/{thumb_folder}"
             jpgfile=f"{jpgfolder}/{Path(fitsfile).stem}.jpg"
-            
+            print(f"jpgfolder:{jpgfolder}")
             if not Path(jpgfolder).exists(): Path(jpgfolder).mkdir(parents=True,exist_ok=True)
             if not Path(jpgfile).exists() or force: subprocess.run(["convert", fitsfile,"-linear-stretch","1x1","-resize", "56%", jpgfile ])
-            
+
+def fits2fits_bulk(fitsfolderlist, **kwargs):
+    """
+    takes input as list of string fits folder paths and executes fits_to_fits() using for loop to each folder path.
+    see *fits_to_fits()* for the list of parameters.
+    If fits to fits conversion fails, the file is saved in "corrupt/" (can be changed from call) folder at the tiff source folder.
+    """
+    params={'failed_folder':'corrupt/'}
+    params.update(kwargs)
+        
+    if isinstance(fitsfolderlist,list):
+        for fitsfolder in fitsfolderlist:
+            listfits=search_file(fitsfolder,'.fits', recursive=True)
+            for f in listfits:
+                if not 'corrupt' in f:
+                    params['failed_folder']=f"{Path(f).parent}/corrupt/"
+                    try:
+                        fits_to_fits(f, **kwargs)
+                    except Exception as e:
+                        try:
+                            # if Path(f).stat().st_size <= desiredsize:
+                            print(e)
+                            Path(params['failed_folder']).mkdir(parents=True,exist_ok=True)
+                            shutil.copy(str(f), str(f"{params['failed_folder']}/{Path(f).name}"))
+                        except:
+                            with open('failed.scoobi','+a') as sf:
+                                sf.write(f"{f}\n")
+    else:
+        raise Exception(f'Is "{fitsfolderlist}" a list?')           
 
 def tif2fits_bulk(tiffolderlist, **kwargs):
     """
     takes input as list of string tiff folder paths and executes tif to fits using for loop to each folder path.
     see *tif_to_fits()* for the list of parameters.
     If tif to fits conversion fails, the file is saved in "corrupt/" (can be changed from call) folder at the tiff source folder.
     """
```

### Comparing `scoobi-0.0.1.4/src/scoobi/cli.py` & `scoobi-0.0.1.5/src/scoobi/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumb_gen
+from scoobi import compare_datetime, read_tif, Time, tif2fits_bulk, tif_to_fits, compare_datetime_nofolder, thumb_gen,fits2fits_bulk,fits_to_fits
 from collections import defaultdict
 from pathlib import Path
 
 def read_configfile(filepath):
     with open(filepath,'r') as f:
         params = defaultdict(list)
         pr=f.read().splitlines()
@@ -20,15 +20,16 @@
                 else:
                     params[k]=v
     return params
 
 def default_params():
     return {'fits_folder':'/data/solar_data/processed', 
         'csv_file':'/data/solar_data/raw/log.csv',
-        'tiff_folder':'/data/solar_data/raw/', 
+        'tiff_folder':'/data/solar_data/raw/',
+        'raw_folder':'/data/solar_data/raw/', 
         'month':'Jan,Feb,Mar,Apr,May,June,July,Aug,Sept,Oct,Nov,Dec', 
         'days':'1,32'}
 
 def create_config(params, out='.config'):
     with open(out, 'w') as o:
         for k,v in params.items():
             if isinstance(v,list) : 
@@ -41,15 +42,16 @@
 
 parser = argparse.ArgumentParser('scoobi',description="""
 Solar Conventionality-based Organizing Observation data ( SCOOBI )""", formatter_class=argparse.RawDescriptionHelpFormatter)
 
 # pa = parser.add_subparsers(help='compare datetimes') # subparser is used like $pip "install"
 
 parser.add_argument('-f','--fits_folder', help='source') #positionals
-parser.add_argument('-t','--tiff_folder', help='tiff folder path')
+parser.add_argument('-t','--tiff_folder', help='RAW TIFF folder path')
+parser.add_argument('-r','--raw_folder', help='RAW FITS folder path')
 parser.add_argument('-o','--output_file', help='complete path for output csv or log file.')
 parser.add_argument('-c','--config_file', help='complete path for config file with inputs', default='.config')
 # parser.add_argument('-hdr','--header', help='Input header to inject to the FITS file.')
 
 headers=parser.add_argument_group('header', """Parameters for injecting and printing headers.
 [[Work in Progress]]""")
 headers.add_argument('-hdr','--header', type=str, help="Comma separated input headers to inject to the raw file.", required=False)
@@ -61,24 +63,25 @@
 Ex --days='1,32'""")
 
 parser.add_argument('--no-datedfolder', action='store_true', dest='no_datedfolder',help='if not needed to create dated folder') 
 parser.add_argument('-rt','--read-time', action='store_true', dest='rt',help='reads time from a tiff file') 
 parser.add_argument('-ct','--compare-time', action='store_true', dest='ct',help='compares time from a fits file to a tiff file') 
 parser.add_argument('-rc','--read-config',action='store_true',dest='rc', help=" read config, bool")
 parser.add_argument('-cc','--create-config',action='store_true',dest='cc', help=" create config, if called with rc would modify from and to the CONFIG_FILE path")
-parser.add_argument('-do','--do-conversion',action='store_true',dest='do', help=" create fits from tiff file and take care of the folder structure. Requires tiff_folder path")
+parser.add_argument('-do','--do-conversion',action='store_true',dest='do', help=" create fits from tiff/fits raw file and take care of the folder structure. Requires tiff_folder or raw_folder path")
 parser.add_argument('-th','--thumbnail', action='store_true', dest='th',help='True/False for creating thumbnails; The fits folder path is required but should be more specific e.g atleaset including the /processed; should not be used with -do')
 
 args=parser.parse_args()
 def cli():
     params=default_params()
     header = defaultdict(list)
     if args.fits_folder: params['fits_folder']=args.fits_folder
     if args.output_file: params['csv_file']=args.output_file
     if args.tiff_folder: params['tiff_folder']=args.tiff_folder
+    if args.raw_folder: params['raw_folder']=args.raw_folder
     if args.header_file_output: print(args.header_file_output)
     if args.header: 
         hdrin=str(args.header).replace(' ','')
         hdrdict=hdrin.split(',')
         for i in range(len(hdrdict)):
             if '=' in hdrdict[i]:
                 hdrk,hdrv=hdrdict[i].split('=')
@@ -104,15 +107,21 @@
 
     if args.ct and not args.no_datedfolder: compare_datetime(**params)
     if args.no_datedfolder and args.ct: compare_datetime_nofolder(**params)
     if args.rc: print(read_configfile(configfile))
     if args.cc: print(create_config(params,configfile))
     if args.rt: print(str(read_tif(params['tiff_folder'])['Image DateTime'].values))
     if args.do: 
-        if '.tif' not in params['tiff_folder']: 
-            print(tif2fits_bulk(params['tiff_folder'].split(','), destfolder=params['fits_folder']))
-        else:
-            print(tif_to_fits(params['tiff_folder'], destfolder=params['fits_folder']))
+        if args.tiff_folder:
+            if '.tif' not in params['tiff_folder']: 
+                print(tif2fits_bulk(params['tiff_folder'].split(','), destfolder=params['fits_folder']))
+            else:
+                print(tif_to_fits(params['tiff_folder'], destfolder=params['fits_folder']))
+        if args.raw_folder:
+            if not any(fts in params['raw_folder'] for fts in ['.fits', '.fts']): 
+                print(fits2fits_bulk(params['raw_folder'].split(','), destfolder=params['fits_folder']))
+            else:
+                print(fits_to_fits(params['raw_folder'], destfolder=params['fits_folder']))
     if args.th: thumb_gen(params['fits_folder'])
         
 if __name__=='__main__':
     cli()
```

### Comparing `scoobi-0.0.1.4/src/scoobi.egg-info/PKG-INFO` & `scoobi-0.0.1.5/src/scoobi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoobi
-Version: 0.0.1.4
+Version: 0.0.1.5
 Summary: Solar Conventionality-based Organizing Observation data ( SCOOBI )
 Home-page: https://github.com/avialxee/scoobi
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/scoobi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

