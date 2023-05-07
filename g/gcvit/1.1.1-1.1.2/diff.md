# Comparing `tmp/gcvit-1.1.1.tar.gz` & `tmp/gcvit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/gcvit-tf/gcvit-tf/dist/tmpsonuh150/gcvit-1.1.1.tar", last modified: Sat Jan 14 21:24:27 2023, max compression
+gzip compressed data, was "gcvit-1.1.2.tar", last modified: Sun May  7 03:08:34 2023, max compression
```

## Comparing `gcvit-1.1.1.tar` & `gcvit-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     7007 2023-01-14 21:24:27.000000 gcvit-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit/layers/
--rw-r--r--   0 runner    (1001) docker     (116)     4218 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/block.py
--rw-r--r--   0 runner    (1001) docker     (116)      814 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (116)     9524 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/feature.py
--rw-r--r--   0 runner    (1001) docker     (116)      609 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/window.py
--rw-r--r--   0 runner    (1001) docker     (116)     1276 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/drop.py
--rw-r--r--   0 runner    (1001) docker     (116)     3678 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/level.py
--rw-r--r--   0 runner    (1001) docker     (116)     4748 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (116)      286 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2786 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/utils/gradcam.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit/models/
--rw-r--r--   0 runner    (1001) docker     (116)     8724 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/models/gcvit.py
--rw-r--r--   0 runner    (1001) docker     (116)       95 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       21 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/version.py
--rw-r--r--   0 runner    (1001) docker     (116)      130 2023-01-14 21:24:18.000000 gcvit-1.1.1/gcvit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5917 2023-01-14 21:24:18.000000 gcvit-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-01-14 21:24:18.000000 gcvit-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)     1971 2023-01-14 21:24:18.000000 gcvit-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7007 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      491 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       42 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-14 21:24:27.000000 gcvit-1.1.1/gcvit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-14 21:24:27.000000 gcvit-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 03:08:21.000000 gcvit-1.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-07 03:08:34.559786 gcvit-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-07 03:08:21.000000 gcvit-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/gcvit/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/gcvit/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/layers/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/gcvit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/models/gcvit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/gcvit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/utils/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 03:08:21.000000 gcvit-1.1.2/gcvit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:08:34.559786 gcvit-1.1.2/gcvit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-07 03:08:34.000000 gcvit-1.1.2/gcvit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-07 03:08:34.000000 gcvit-1.1.2/gcvit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:08:34.000000 gcvit-1.1.2/gcvit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 03:08:34.000000 gcvit-1.1.2/gcvit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 03:08:34.000000 gcvit-1.1.2/gcvit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:08:34.559786 gcvit-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-07 03:08:21.000000 gcvit-1.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gcvit-1.1.1/PKG-INFO` & `gcvit-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gcvit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensorflow 2.0 Implementation of GCViT: Global Context Vision Transformer. https://github.com/awsaf49/gcvit-tf
 Home-page: https://github.com/awsaf49/gcvit-tf
 Author: Awsaf
 Author-email: awsaf49@gmail.com
 License: MIT
 Keywords: tensorflow computer_vision image classification transformer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,14 +43,15 @@
 </h2>
 </p>
 <p align="center">
 This library implements <b>GCViT</b> using Tensorflow 2.0 specifically in <code>tf.keras.Model</code> manner to get PyTorch flavor.
 </p>
 
 ## Update
+* **15 Jan 2023** : `GCViTLarge` model added with ckpt.
 * **3 Sept 2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on this project won [Kaggle ML Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/349817).
 * **19 Aug 2022** : This project got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-party-implementations-and-resources)
 
 ## Model
 * Architecture:
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG">
@@ -121,14 +121,21 @@
 print(feature.shape)
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
+## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+```py
+from gcvit import GCViTTiny
+model = GCViTTiny(pretrain=True, from_kaggle=True)
+```
+
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
 
 <a href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="image/gradio_demo.JPG" height=500></a>
 
 ## Example
 For working training example checkout these notebooks on **Google Colab** <a href="https://colab.research.google.com/github/awsaf49/gcvit-tf/blob/main/notebooks/GCViT_Flower_Classification.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> & **Kaggle** <a href="https://www.kaggle.com/awsaf49/flower-classification-gcvit-global-context-vit"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>.
@@ -136,15 +143,17 @@
 Here is grad-cam result after training on Flower Classification Dataset,
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
+- [ ] Remove `tensorflow_addons`
 - [ ] Segmentation Pipeline
+- [ ] Support for `Kaggle Models`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
 - [x] Support for `TPU`.
@@ -161,9 +170,7 @@
 @article{hatamizadeh2022global,
   title={Global Context Vision Transformers},
   author={Hatamizadeh, Ali and Yin, Hongxu and Kautz, Jan and Molchanov, Pavlo},
   journal={arXiv preprint arXiv:2206.09959},
   year={2022}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,72 +1,78 @@
-Metadata-Version: 2.1 Name: gcvit Version: 1.1.1 Summary: Tensorflow 2.0
+Metadata-Version: 2.1 Name: gcvit Version: 1.1.2 Summary: Tensorflow 2.0
 Implementation of GCViT: Global Context Vision Transformer. https://github.com/
 awsaf49/gcvit-tf Home-page: https://github.com/awsaf49/gcvit-tf Author: Awsaf
 Author-email: awsaf49@gmail.com License: MIT Keywords: tensorflow
-computer_vision image classification transformer Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.6 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+computer_vision image classification transformer Classifier: Development Status
+:: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE.md
             ****** GCViT:_Global_Context_Vision_Transformer ******
  [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_arch.PNG]
   [https://img.shields.io/badge/License-MIT-yellow.svg] [python] [tensorflow]
 [https://img.shields.io/badge/ð¤%20Hugging%20Face-Spaces-yellow.svg] [Open_In
                             Colab] [Open_In_Kaggle]
               ***** Tensorflow 2.0 Implementation of GCViT *****
       This library implements GCViT using Tensorflow 2.0 specifically in
                  tf.keras.Model manner to get PyTorch flavor.
-## Update * **3 Sept 2022** : Annotated [kaggle-notebook](https://
-www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on
-this project won [Kaggle ML Research Spotlight: August 2022](https://
-www.kaggle.com/discussions/general/349817). * **19 Aug 2022** : This project
-got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here]
-(https://github.com/NVlabs/GCVit#third-party-implementations-and-resources) ##
-Model * Architecture: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
-image/arch.PNG] * Local Vs Global Attention: [https://
-raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_msa.PNG] ## Result
-[https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/result.PNG]
-Official codebase had some issue which has been fixed recently (12 August
-2022). Here's the result of ported weights on **ImageNetV2-Test** data, | Model
-| Acc@1 | Acc@5 | #Params | |--------------|-------|-------|---------| | GCViT-
-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 | 0.885 | 20M | | GCViT-
-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 | 0.901 | 51M | | GCViT-Base
-| 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 | 0.913 | 202M | ## Installation
-```bash pip install -U gcvit # or # pip install -U git+https://github.com/
-awsaf49/gcvit-tf ``` ## Usage Load model using following codes, ```py from
-gcvit import GCViTTiny model = GCViTTiny(pretrain=True) ``` Simple code to
-check model's prediction, ```py from skimage.data import chelsea img =
+## Update * **15 Jan 2023** : `GCViTLarge` model added with ckpt. * **3 Sept
+2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-
+global-context-vision-transformer) based on this project won [Kaggle ML
+Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/
+349817). * **19 Aug 2022** : This project got acknowledged by [Official](https:
+//github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-
+party-implementations-and-resources) ## Model * Architecture: [https://
+raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG] * Local Vs
+Global Attention: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
+image/lvg_msa.PNG] ## Result [https://raw.githubusercontent.com/awsaf49/gcvit-
+tf/main/image/result.PNG] Official codebase had some issue which has been fixed
+recently (12 August 2022). Here's the result of ported weights on **ImageNetV2-
+Test** data, | Model | Acc@1 | Acc@5 | #Params | |--------------|-------|------
+-|---------| | GCViT-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 |
+0.885 | 20M | | GCViT-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 |
+0.901 | 51M | | GCViT-Base | 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 |
+0.913 | 202M | ## Installation ```bash pip install -U gcvit # or # pip install
+-U git+https://github.com/awsaf49/gcvit-tf ``` ## Usage Load model using
+following codes, ```py from gcvit import GCViTTiny model = GCViTTiny
+(pretrain=True) ``` Simple code to check model's prediction, ```py from
+skimage.data import chelsea img =
 tf.keras.applications.imagenet_utils.preprocess_input(chelsea(), mode='torch')
 # Chelsea the cat img = tf.image.resize(img, (224, 224))[None,] # resize &
 create batch pred = model(img).numpy() print
 (tf.keras.applications.imagenet_utils.decode_predictions(pred)[0]) ```
 Prediction: ```py [('n02124075', 'Egyptian_cat', 0.9194835), ('n02123045',
 'tabby', 0.009686623), ('n02123159', 'tiger_cat', 0.0061576385), ('n02127052',
 'lynx', 0.0011503297), ('n02883205', 'bow_tie', 0.00042479983)] ``` For feature
 extraction: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
-(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Live-Demo * For
-live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click
-[https://img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and
-Gradio. here's an example, [image/gradio_demo.JPG] ## Example For working
-training example checkout these notebooks on **Google Colab** [Open_In_Colab] &
+(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://
+www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
+enforce model to load weights from Kaggle Models with downloading, thus can be
+used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
+Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
+img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
+here's an example, [image/gradio_demo.JPG] ## Example For working training
+example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x] New
-updated weights have been added. - [x] Working training example in Colab &
-Kaggle. - [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
+main/image/flower_gradcam.PNG] ## To Do - [ ] Remove `tensorflow_addons` - [ ]
+Segmentation Pipeline - [ ] Support for `Kaggle Models` - [x] New updated
+weights have been added. - [x] Working training example in Colab & Kaggle. -
+[x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
 [keras_cv_attention_models](https://github.com/leondgarse/
 keras_cv_attention_model) ## Citation ```bibtex @article{hatamizadeh2022global,
 title={Global Context Vision Transformers}, author={Hatamizadeh, Ali and Yin,
```

### Comparing `gcvit-1.1.1/gcvit/layers/block.py` & `gcvit-1.1.2/gcvit/layers/block.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/layers/embedding.py` & `gcvit-1.1.2/gcvit/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/layers/feature.py` & `gcvit-1.1.2/gcvit/layers/feature.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/layers/window.py` & `gcvit-1.1.2/gcvit/layers/window.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/layers/drop.py` & `gcvit-1.1.2/gcvit/layers/drop.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     def call(self, x, training=None):
         if self.drop_prob==0. or not training:
             return x
         keep_prob = 1 - self.drop_prob
         shape = (tf.shape(x)[0],) + (1,) * (len(tf.shape(x)) - 1)
         random_tensor = keep_prob + tf.random.uniform(shape, 0, 1)
         random_tensor = tf.floor(random_tensor)
+        if random_tensor.dtype != x.dtype:
+            random_tensor = tf.cast(random_tensor, dtype=x.dtype)
         if keep_prob > 0.0 and self.scale_by_keep:
             x = (x / keep_prob) 
         return x * random_tensor
 
     def get_config(self):
         config = super().get_config()
         config.update({
```

### Comparing `gcvit-1.1.1/gcvit/layers/level.py` & `gcvit-1.1.2/gcvit/layers/level.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/layers/attention.py` & `gcvit-1.1.2/gcvit/layers/attention.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/utils/gradcam.py` & `gcvit-1.1.2/gcvit/utils/gradcam.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit/models/gcvit.py` & `gcvit-1.1.2/gcvit/models/gcvit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 import numpy as np
 import tensorflow as tf
 
 from ..layers import Stem, GCViTLevel, Identity
 
-                  
+# Params for pretrained models                 
 BASE_URL = 'https://github.com/awsaf49/gcvit-tf/releases/download'
 TAG = 'v1.1.1'
+
+# Params for Kaggle Models (KM)
+KM_DIR = '/kaggle/input/gcvit-tf/tensorflow2'
+KM_VERSION = '1'
+NAME2TITLE = {
+    'gcvit_xxtiny': 'GCViT-XXTiny',
+    'gcvit_xtiny': 'GCViT-XTiny',
+    'gcvit_tiny': 'GCViT-Tiny',
+    'gcvit_small': 'GCViT-Small',
+    'gcvit_base': 'GCViT-Base',
+    'gcvit_large': 'GCViT-Large',
+}
+
 NAME2CONFIG = {
     'gcvit_xxtiny': {'window_size': (7, 7, 14, 7),
                     'dim': 64,
                     'depths': (2, 2, 6, 2),
                     'num_heads': (2, 4, 8, 16),
                     'mlp_ratio': 3.,
                     'path_drop': 0.2},
@@ -87,27 +100,27 @@
             self.pool = tf.keras.layers.GlobalAveragePooling2D(name='pool')
         elif global_pool == 'max':
             self.pool = tf.keras.layers.GlobalMaxPooling2D(name='pool')
         elif global_pool is None:
             self.pool = Identity(name='pool')
         else:
             raise ValueError(f'Expecting pooling to be one of None/avg/max. Found: {global_pool}')
-        self.head = tf.keras.layers.Dense(num_classes, name='head', activation=head_act)
+        self.head = tf.keras.layers.Dense(num_classes, name='head', activation=head_act, dtype="float32")
 
     def reset_classifier(self, num_classes, head_act, global_pool=None, in_channels=3):
         self.num_classes = num_classes
         if global_pool is not None:
             self.global_pool = global_pool
-        self.head = tf.keras.layers.Dense(num_classes, name='head', activation=head_act) if num_classes else Identity(name='head')
+        self.head = tf.keras.layers.Dense(num_classes, name='head', activation=head_act, dtype="float32") if num_classes else Identity(name='head')
         super().build((1, 224, 224, in_channels)) # for head we only need info from the input channel
         
     def forward_features(self, inputs):
         x = self.patch_embed(inputs)
         x = self.pos_drop(x)
-        x = tf.cast(x, dtype=tf.float32)
+        # x = tf.cast(x, dtype=tf.float32)
         for level in self.levels:
             x = level(x)
         x = self.norm(x)
         return x
 
     def forward_head(self, inputs, pre_logits=False):
         x = inputs
@@ -127,72 +140,96 @@
         x = tf.keras.Input(shape=input_shape)
         return tf.keras.Model(inputs=[x], outputs=self.call(x), name=self.name)
 
     def summary(self, input_shape=(224, 224, 3)):
         return self.build_graph(input_shape).summary()
 
 # load standard models
-def GCViTXXTiny(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTXXTiny(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_xxtiny'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config,  **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+            print("Loading ckpt from {}".format(ckpt_path))
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
 
-def GCViTXTiny(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTXTiny(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_xtiny'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config,  **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+            print("Loading ckpt from {}".format(ckpt_path))
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
 
-def GCViTTiny(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTTiny(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_tiny'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config,  **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+            print("Loading ckpt from {}".format(ckpt_path))
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
 
-def GCViTSmall(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTSmall(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_small'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config, **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+            print("Loading ckpt from {}".format(ckpt_path))
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
 
-def GCViTBase(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTBase(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_base'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config, **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+            print("Loading ckpt from {}".format(ckpt_path))
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
 
-def GCViTLarge(input_shape=(224, 224, 3), pretrain=False, resize_query=False, **kwargs):
+def GCViTLarge(input_shape=(224, 224, 3), pretrain=False, from_kaggle=False, resize_query=False, **kwargs):
     name = 'gcvit_large'
     config = NAME2CONFIG[name]
     ckpt_link = '{}/{}/{}_weights.h5'.format(BASE_URL, TAG, name)
     model = GCViT(name=name, resize_query=resize_query, **config, **kwargs)
     model(tf.random.uniform(shape=input_shape)[tf.newaxis,])
     if pretrain:
-        ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
+        if from_kaggle:
+            print("Loading ckpt from {}".format(ckpt_path))
+            ckpt_path = '{}/{}/{}/{}_weights.h5'.format(KM_DIR, NAME2TITLE[name], KM_VERSION, name)
+        else:
+            ckpt_path = tf.keras.utils.get_file('{}_weights.h5'.format(name), ckpt_link)
         model.load_weights(ckpt_path)
     return model
```

### Comparing `gcvit-1.1.1/README.md` & `gcvit-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 </h2>
 </p>
 <p align="center">
 This library implements <b>GCViT</b> using Tensorflow 2.0 specifically in <code>tf.keras.Model</code> manner to get PyTorch flavor.
 </p>
 
 ## Update
+* **15 Jan 2023** : `GCViTLarge` model added with ckpt.
 * **3 Sept 2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on this project won [Kaggle ML Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/349817).
 * **19 Aug 2022** : This project got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-party-implementations-and-resources)
 
 ## Model
 * Architecture:
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG">
@@ -95,14 +96,21 @@
 print(feature.shape)
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
+## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+```py
+from gcvit import GCViTTiny
+model = GCViTTiny(pretrain=True, from_kaggle=True)
+```
+
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
 
 <a href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="image/gradio_demo.JPG" height=500></a>
 
 ## Example
 For working training example checkout these notebooks on **Google Colab** <a href="https://colab.research.google.com/github/awsaf49/gcvit-tf/blob/main/notebooks/GCViT_Flower_Classification.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> & **Kaggle** <a href="https://www.kaggle.com/awsaf49/flower-classification-gcvit-global-context-vit"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>.
@@ -110,15 +118,17 @@
 Here is grad-cam result after training on Flower Classification Dataset,
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
+- [ ] Remove `tensorflow_addons`
 - [ ] Segmentation Pipeline
+- [ ] Support for `Kaggle Models`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
 - [x] Support for `TPU`.
```

#### html2text {}

```diff
@@ -2,56 +2,63 @@
  [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_arch.PNG]
   [https://img.shields.io/badge/License-MIT-yellow.svg] [python] [tensorflow]
 [https://img.shields.io/badge/ð¤%20Hugging%20Face-Spaces-yellow.svg] [Open_In
                             Colab] [Open_In_Kaggle]
               ***** Tensorflow 2.0 Implementation of GCViT *****
       This library implements GCViT using Tensorflow 2.0 specifically in
                  tf.keras.Model manner to get PyTorch flavor.
-## Update * **3 Sept 2022** : Annotated [kaggle-notebook](https://
-www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on
-this project won [Kaggle ML Research Spotlight: August 2022](https://
-www.kaggle.com/discussions/general/349817). * **19 Aug 2022** : This project
-got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here]
-(https://github.com/NVlabs/GCVit#third-party-implementations-and-resources) ##
-Model * Architecture: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
-image/arch.PNG] * Local Vs Global Attention: [https://
-raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_msa.PNG] ## Result
-[https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/result.PNG]
-Official codebase had some issue which has been fixed recently (12 August
-2022). Here's the result of ported weights on **ImageNetV2-Test** data, | Model
-| Acc@1 | Acc@5 | #Params | |--------------|-------|-------|---------| | GCViT-
-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 | 0.885 | 20M | | GCViT-
-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 | 0.901 | 51M | | GCViT-Base
-| 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 | 0.913 | 202M | ## Installation
-```bash pip install -U gcvit # or # pip install -U git+https://github.com/
-awsaf49/gcvit-tf ``` ## Usage Load model using following codes, ```py from
-gcvit import GCViTTiny model = GCViTTiny(pretrain=True) ``` Simple code to
-check model's prediction, ```py from skimage.data import chelsea img =
+## Update * **15 Jan 2023** : `GCViTLarge` model added with ckpt. * **3 Sept
+2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-
+global-context-vision-transformer) based on this project won [Kaggle ML
+Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/
+349817). * **19 Aug 2022** : This project got acknowledged by [Official](https:
+//github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-
+party-implementations-and-resources) ## Model * Architecture: [https://
+raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG] * Local Vs
+Global Attention: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
+image/lvg_msa.PNG] ## Result [https://raw.githubusercontent.com/awsaf49/gcvit-
+tf/main/image/result.PNG] Official codebase had some issue which has been fixed
+recently (12 August 2022). Here's the result of ported weights on **ImageNetV2-
+Test** data, | Model | Acc@1 | Acc@5 | #Params | |--------------|-------|------
+-|---------| | GCViT-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 |
+0.885 | 20M | | GCViT-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 |
+0.901 | 51M | | GCViT-Base | 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 |
+0.913 | 202M | ## Installation ```bash pip install -U gcvit # or # pip install
+-U git+https://github.com/awsaf49/gcvit-tf ``` ## Usage Load model using
+following codes, ```py from gcvit import GCViTTiny model = GCViTTiny
+(pretrain=True) ``` Simple code to check model's prediction, ```py from
+skimage.data import chelsea img =
 tf.keras.applications.imagenet_utils.preprocess_input(chelsea(), mode='torch')
 # Chelsea the cat img = tf.image.resize(img, (224, 224))[None,] # resize &
 create batch pred = model(img).numpy() print
 (tf.keras.applications.imagenet_utils.decode_predictions(pred)[0]) ```
 Prediction: ```py [('n02124075', 'Egyptian_cat', 0.9194835), ('n02123045',
 'tabby', 0.009686623), ('n02123159', 'tiger_cat', 0.0061576385), ('n02127052',
 'lynx', 0.0011503297), ('n02883205', 'bow_tie', 0.00042479983)] ``` For feature
 extraction: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
-(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Live-Demo * For
-live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click
-[https://img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and
-Gradio. here's an example, [image/gradio_demo.JPG] ## Example For working
-training example checkout these notebooks on **Google Colab** [Open_In_Colab] &
+(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://
+www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
+enforce model to load weights from Kaggle Models with downloading, thus can be
+used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
+Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
+img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
+here's an example, [image/gradio_demo.JPG] ## Example For working training
+example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x] New
-updated weights have been added. - [x] Working training example in Colab &
-Kaggle. - [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
+main/image/flower_gradcam.PNG] ## To Do - [ ] Remove `tensorflow_addons` - [ ]
+Segmentation Pipeline - [ ] Support for `Kaggle Models` - [x] New updated
+weights have been added. - [x] Working training example in Colab & Kaggle. -
+[x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
 [keras_cv_attention_models](https://github.com/leondgarse/
 keras_cv_attention_model) ## Citation ```bibtex @article{hatamizadeh2022global,
 title={Global Context Vision Transformers}, author={Hatamizadeh, Ali and Yin,
```

### Comparing `gcvit-1.1.1/LICENSE.md` & `gcvit-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/setup.py` & `gcvit-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `gcvit-1.1.1/gcvit.egg-info/PKG-INFO` & `gcvit-1.1.2/gcvit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gcvit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tensorflow 2.0 Implementation of GCViT: Global Context Vision Transformer. https://github.com/awsaf49/gcvit-tf
 Home-page: https://github.com/awsaf49/gcvit-tf
 Author: Awsaf
 Author-email: awsaf49@gmail.com
 License: MIT
 Keywords: tensorflow computer_vision image classification transformer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,14 +43,15 @@
 </h2>
 </p>
 <p align="center">
 This library implements <b>GCViT</b> using Tensorflow 2.0 specifically in <code>tf.keras.Model</code> manner to get PyTorch flavor.
 </p>
 
 ## Update
+* **15 Jan 2023** : `GCViTLarge` model added with ckpt.
 * **3 Sept 2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on this project won [Kaggle ML Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/349817).
 * **19 Aug 2022** : This project got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-party-implementations-and-resources)
 
 ## Model
 * Architecture:
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG">
@@ -121,14 +121,21 @@
 print(feature.shape)
 ```
 Feature map:
 ```py
 (None, 7, 7, 512)
 ```
 
+## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will enforce model to load weights from Kaggle Models with downloading, thus can be used without internet in Kaggle.
+```py
+from gcvit import GCViTTiny
+model = GCViTTiny(pretrain=True, from_kaggle=True)
+```
+
 ## Live-Demo
 * For live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click <a target="_blank" href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="https://img.shields.io/badge/Try%20on-Gradio-orange"></a> powered by 🤗 Space and Gradio. here's an example,
 
 <a href="https://huggingface.co/spaces/awsaf49/gcvit-tf"><img src="image/gradio_demo.JPG" height=500></a>
 
 ## Example
 For working training example checkout these notebooks on **Google Colab** <a href="https://colab.research.google.com/github/awsaf49/gcvit-tf/blob/main/notebooks/GCViT_Flower_Classification.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> & **Kaggle** <a href="https://www.kaggle.com/awsaf49/flower-classification-gcvit-global-context-vit"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>.
@@ -136,15 +143,17 @@
 Here is grad-cam result after training on Flower Classification Dataset,
 
 <img src="https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/flower_gradcam.PNG" height=500>
 
 
 
 ## To Do
+- [ ] Remove `tensorflow_addons`
 - [ ] Segmentation Pipeline
+- [ ] Support for `Kaggle Models`
 - [x] New updated weights have been added.
 - [x] Working training example in Colab & Kaggle.
 - [x] GradCAM showcase.
 - [x] Gradio Demo.
 - [x] Build model with `tf.keras.Model`.
 - [x] Port weights from official repo.
 - [x] Support for `TPU`.
@@ -161,9 +170,7 @@
 @article{hatamizadeh2022global,
   title={Global Context Vision Transformers},
   author={Hatamizadeh, Ali and Yin, Hongxu and Kautz, Jan and Molchanov, Pavlo},
   journal={arXiv preprint arXiv:2206.09959},
   year={2022}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,72 +1,78 @@
-Metadata-Version: 2.1 Name: gcvit Version: 1.1.1 Summary: Tensorflow 2.0
+Metadata-Version: 2.1 Name: gcvit Version: 1.1.2 Summary: Tensorflow 2.0
 Implementation of GCViT: Global Context Vision Transformer. https://github.com/
 awsaf49/gcvit-tf Home-page: https://github.com/awsaf49/gcvit-tf Author: Awsaf
 Author-email: awsaf49@gmail.com License: MIT Keywords: tensorflow
-computer_vision image classification transformer Platform: UNKNOWN Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.6 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+computer_vision image classification transformer Classifier: Development Status
+:: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE.md
             ****** GCViT:_Global_Context_Vision_Transformer ******
  [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_arch.PNG]
   [https://img.shields.io/badge/License-MIT-yellow.svg] [python] [tensorflow]
 [https://img.shields.io/badge/ð¤%20Hugging%20Face-Spaces-yellow.svg] [Open_In
                             Colab] [Open_In_Kaggle]
               ***** Tensorflow 2.0 Implementation of GCViT *****
       This library implements GCViT using Tensorflow 2.0 specifically in
                  tf.keras.Model manner to get PyTorch flavor.
-## Update * **3 Sept 2022** : Annotated [kaggle-notebook](https://
-www.kaggle.com/code/awsaf49/gcvit-global-context-vision-transformer) based on
-this project won [Kaggle ML Research Spotlight: August 2022](https://
-www.kaggle.com/discussions/general/349817). * **19 Aug 2022** : This project
-got acknowledged by [Official](https://github.com/NVlabs/GCVit) repo [here]
-(https://github.com/NVlabs/GCVit#third-party-implementations-and-resources) ##
-Model * Architecture: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
-image/arch.PNG] * Local Vs Global Attention: [https://
-raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/lvg_msa.PNG] ## Result
-[https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/result.PNG]
-Official codebase had some issue which has been fixed recently (12 August
-2022). Here's the result of ported weights on **ImageNetV2-Test** data, | Model
-| Acc@1 | Acc@5 | #Params | |--------------|-------|-------|---------| | GCViT-
-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 | 0.885 | 20M | | GCViT-
-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 | 0.901 | 51M | | GCViT-Base
-| 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 | 0.913 | 202M | ## Installation
-```bash pip install -U gcvit # or # pip install -U git+https://github.com/
-awsaf49/gcvit-tf ``` ## Usage Load model using following codes, ```py from
-gcvit import GCViTTiny model = GCViTTiny(pretrain=True) ``` Simple code to
-check model's prediction, ```py from skimage.data import chelsea img =
+## Update * **15 Jan 2023** : `GCViTLarge` model added with ckpt. * **3 Sept
+2022** : Annotated [kaggle-notebook](https://www.kaggle.com/code/awsaf49/gcvit-
+global-context-vision-transformer) based on this project won [Kaggle ML
+Research Spotlight: August 2022](https://www.kaggle.com/discussions/general/
+349817). * **19 Aug 2022** : This project got acknowledged by [Official](https:
+//github.com/NVlabs/GCVit) repo [here](https://github.com/NVlabs/GCVit#third-
+party-implementations-and-resources) ## Model * Architecture: [https://
+raw.githubusercontent.com/awsaf49/gcvit-tf/main/image/arch.PNG] * Local Vs
+Global Attention: [https://raw.githubusercontent.com/awsaf49/gcvit-tf/main/
+image/lvg_msa.PNG] ## Result [https://raw.githubusercontent.com/awsaf49/gcvit-
+tf/main/image/result.PNG] Official codebase had some issue which has been fixed
+recently (12 August 2022). Here's the result of ported weights on **ImageNetV2-
+Test** data, | Model | Acc@1 | Acc@5 | #Params | |--------------|-------|------
+-|---------| | GCViT-XXTiny | 0.663 | 0.873 | 12M | | GCViT-XTiny | 0.685 |
+0.885 | 20M | | GCViT-Tiny | 0.708 | 0.899 | 28M | | GCViT-Small | 0.720 |
+0.901 | 51M | | GCViT-Base | 0.731 | 0.907 | 90M | | GCViT-Large | 0.734 |
+0.913 | 202M | ## Installation ```bash pip install -U gcvit # or # pip install
+-U git+https://github.com/awsaf49/gcvit-tf ``` ## Usage Load model using
+following codes, ```py from gcvit import GCViTTiny model = GCViTTiny
+(pretrain=True) ``` Simple code to check model's prediction, ```py from
+skimage.data import chelsea img =
 tf.keras.applications.imagenet_utils.preprocess_input(chelsea(), mode='torch')
 # Chelsea the cat img = tf.image.resize(img, (224, 224))[None,] # resize &
 create batch pred = model(img).numpy() print
 (tf.keras.applications.imagenet_utils.decode_predictions(pred)[0]) ```
 Prediction: ```py [('n02124075', 'Egyptian_cat', 0.9194835), ('n02123045',
 'tabby', 0.009686623), ('n02123159', 'tiger_cat', 0.0061576385), ('n02127052',
 'lynx', 0.0011503297), ('n02883205', 'bow_tie', 0.00042479983)] ``` For feature
 extraction: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 model.reset_classifier(num_classes=0, head_act=None)
 feature = model(img) print(feature.shape) ``` Feature: ```py (None, 512) ```
 For feature map: ```py model = GCViTTiny(pretrain=True) # when pretrain=True,
 num_classes must be 1000 feature = model.forward_features(img) print
-(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Live-Demo * For
-live demo on Image Classification & Grad-CAM, with **ImageNet** weights, click
-[https://img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and
-Gradio. here's an example, [image/gradio_demo.JPG] ## Example For working
-training example checkout these notebooks on **Google Colab** [Open_In_Colab] &
+(feature.shape) ``` Feature map: ```py (None, 7, 7, 512) ``` ## Kaggle Models
+These pre-trained models can also be loaded using [Kaggle Models](https://
+www.kaggle.com/models/awsaf49/gcvit-tf). Setting `from_kaggle=True` will
+enforce model to load weights from Kaggle Models with downloading, thus can be
+used without internet in Kaggle. ```py from gcvit import GCViTTiny model =
+GCViTTiny(pretrain=True, from_kaggle=True) ``` ## Live-Demo * For live demo on
+Image Classification & Grad-CAM, with **ImageNet** weights, click [https://
+img.shields.io/badge/Try%20on-Gradio-orange] powered by ð¤ Space and Gradio.
+here's an example, [image/gradio_demo.JPG] ## Example For working training
+example checkout these notebooks on **Google Colab** [Open_In_Colab] &
 **Kaggle** [Open_In_Kaggle]. Here is grad-cam result after training on Flower
 Classification Dataset, [https://raw.githubusercontent.com/awsaf49/gcvit-tf/
-main/image/flower_gradcam.PNG] ## To Do - [ ] Segmentation Pipeline - [x] New
-updated weights have been added. - [x] Working training example in Colab &
-Kaggle. - [x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
+main/image/flower_gradcam.PNG] ## To Do - [ ] Remove `tensorflow_addons` - [ ]
+Segmentation Pipeline - [ ] Support for `Kaggle Models` - [x] New updated
+weights have been added. - [x] Working training example in Colab & Kaggle. -
+[x] GradCAM showcase. - [x] Gradio Demo. - [x] Build model with
 `tf.keras.Model`. - [x] Port weights from official repo. - [x] Support for
 `TPU`. ## Acknowledgement * [GCVit](https://github.com/NVlabs/GCVit) (Official)
 * [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF) *
 [tfgcvit](https://github.com/shkarupa-alex/tfgcvit/tree/develop/tfgcvit) *
 [keras_cv_attention_models](https://github.com/leondgarse/
 keras_cv_attention_model) ## Citation ```bibtex @article{hatamizadeh2022global,
 title={Global Context Vision Transformers}, author={Hatamizadeh, Ali and Yin,
```

