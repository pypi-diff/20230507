# Comparing `tmp/compel-1.1.3.dev0.tar.gz` & `tmp/compel-1.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-emvysva3/compel-1.1.3.dev0.tar", last modified: Fri Apr 14 08:44:46 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-t3ns2776/compel-1.1.4.dev0.tar", last modified: Sun May  7 07:43:38 2023, max compression
```

## Comparing `compel-1.1.3.dev0.tar` & `compel-1.1.4.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6400 2023-04-14 08:44:28.000000 compel-1.1.3.dev0/README.md
--rw-r--r--   0 damian     (501) staff       (20)      766 2023-04-14 08:42:50.000000 compel-1.1.3.dev0/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.3.dev0/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14494 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.3.dev0/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.3.dev0/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    24862 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29533 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     6983 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 08:44:46.000000 compel-1.1.3.dev0/test/
--rw-r--r--   0 damian     (501) staff       (20)    14454 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-14 08:41:43.000000 compel-1.1.3.dev0/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47126 2023-04-14 08:42:01.000000 compel-1.1.3.dev0/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.4.dev0/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     7101 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     6518 2023-04-30 12:11:27.000000 compel-1.1.4.dev0/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      767 2023-05-07 07:43:20.000000 compel-1.1.4.dev0/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.4.dev0/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14678 2023-05-07 07:42:07.000000 compel-1.1.4.dev0/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.4.dev0/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.4.dev0/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)    25187 2023-05-07 07:42:07.000000 compel-1.1.4.dev0/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29533 2023-05-07 07:42:03.000000 compel-1.1.4.dev0/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     7101 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      462 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 07:43:38.000000 compel-1.1.4.dev0/test/
+-rw-r--r--   0 damian     (501) staff       (20)    14454 2023-05-07 07:40:27.000000 compel-1.1.4.dev0/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-30 12:11:27.000000 compel-1.1.4.dev0/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47126 2023-05-07 07:40:27.000000 compel-1.1.4.dev0/test/test_prompt_parser.py
```

### Comparing `compel-1.1.3.dev0/LICENSE` & `compel-1.1.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/PKG-INFO` & `compel-1.1.4.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.3.dev0
+Version: 1.1.4.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,17 +73,17 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
-To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
```

### Comparing `compel-1.1.3.dev0/README.md` & `compel-1.1.4.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
-To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
```

### Comparing `compel-1.1.3.dev0/pyproject.toml` & `compel-1.1.4.dev0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.3.dev0"
+version = "1.1.4-dev.0"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.3.dev0/src/compel/compel.py` & `compel-1.1.4.dev0/src/compel/compel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import Union, Optional, Callable, List, Tuple
 
 import torch
+from torch import Tensor
 from transformers import CLIPTokenizer, CLIPTextModel
 
 from . import cross_attention_control
 from .conditioning_scheduler import ConditioningScheduler, StaticConditioningScheduler
 from .embeddings_provider import EmbeddingsProvider, BaseTextualInversionManager, DownweightMode
 from .prompt_parser import Blend, FlattenedPrompt, PromptParser, CrossAttentionControlSubstitute, Conjunction
 
@@ -23,16 +24,16 @@
                  tokenizer: CLIPTokenizer,
                  text_encoder: CLIPTextModel,
                  textual_inversion_manager: Optional[BaseTextualInversionManager] = None,
                  dtype_for_device_getter: Callable[[torch.device], torch.dtype] = lambda device: torch.float32,
                  truncate_long_prompts: bool = True,
                  padding_attention_mask_value: int = 1,
                  downweight_mode: DownweightMode = DownweightMode.MASK,
-                 use_penultimate_clip_layer: bool=False
-                 ):
+                 use_penultimate_clip_layer: bool=False,
+                 device: Optional[str] = None):
         """
         Initialize Compel. The tokenizer and text_encoder can be lifted directly from any DiffusionPipeline.
 
         `textual_inversion_manager`: Optional instance to handle expanding multi-vector textual inversion tokens.
         `dtype_for_device_getter`: A Callable that returns a torch dtype for a given device. You probably don't need to
             use this.
         `truncate_long_prompts`: if True, truncate input prompts to 77 tokens long including beginning/end markers
@@ -41,30 +42,32 @@
             markers, as is necessary to encode the whole prompt. You will likely need to supply both positive and
             negative prompts in this case - use `pad_conditioning_tensors_to_same_length` to prevent having tensor
             length mismatch errors when passing the embeds on to your DiffusionPipeline for inference.
         `padding_attention_mask_value`: Value to write into the attention mask for padding tokens. Stable Diffusion needs 1.
         `downweight_mode`: Specifies whether downweighting should be applied by MASKing out the downweighted tokens
             (default) or REMOVEing them (legacy behaviour; messes up position embeddings of tokens following).
         `use_penultimate_clip_layer`: If True, use the penultimate hidden layer output of the CLIP text encoder's output,
-            rather than the final hidden layer output. For SD2.0/2.1 you should probably pass `True` here because SD2
-            is "conditioned on the penultimate text embeddings of a CLIP ViT-H/14 text encoder".
+            rather than the final hidden layer output.
+        `device`: The torch device on which the tensors should be created. If a device is not specified, it'll use the
+            device the `text_encoder` is on (at the moment of calling `build_conditioning_tensor()`).
         """
         self.conditioning_provider = EmbeddingsProvider(tokenizer=tokenizer,
                                                         text_encoder=text_encoder,
                                                         textual_inversion_manager=textual_inversion_manager,
                                                         dtype_for_device_getter=dtype_for_device_getter,
                                                         truncate=truncate_long_prompts,
                                                         padding_attention_mask_value = padding_attention_mask_value,
                                                         downweight_mode=downweight_mode,
                                                         use_penultimate_clip_layer=use_penultimate_clip_layer
                                                         )
+        self._device = device
 
     @property
     def device(self):
-        return self.conditioning_provider.text_encoder.device
+        return self._device if self._device else self.conditioning_provider.text_encoder.device
 
     def make_conditioning_scheduler(self, positive_prompt: str, negative_prompt: str='') -> ConditioningScheduler:
         positive_conditioning = self.build_conditioning_tensor(positive_prompt)
         negative_conditioning = self.build_conditioning_tensor(negative_prompt)
         [positive_conditioning, negative_conditioning] = self.pad_conditioning_tensors_to_same_length(
             [positive_conditioning, negative_conditioning]
         )
@@ -76,15 +79,15 @@
         if len(conjunction.prompts)>1:
             raise ValueError("Conjunctions of >1 prompt are currently not supported by build_conditioning_tensor()")
         prompt_object = conjunction.prompts[0]
         conditioning, _ = self.build_conditioning_tensor_for_prompt_object(prompt_object)
         return conditioning
 
     @torch.no_grad()
-    def __call__(self, text: Union[str, List[str]]) -> torch.Tensor:
+    def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
         if not isinstance(text, list):
             text = [text]
 
         cond_tensor = []
         for text_input in text:
             cond_tensor.append(self.build_conditioning_tensor(text_input))
```

### Comparing `compel-1.1.3.dev0/src/compel/conditioning_scheduler.py` & `compel-1.1.4.dev0/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/src/compel/cross_attention_control.py` & `compel-1.1.4.dev0/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/src/compel/embeddings_provider.py` & `compel-1.1.4.dev0/src/compel/embeddings_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             # "red" is to tell SD that it should almost completely *ignore* redness).
             # To do this, the embedding is lerped away from base_embedding in the direction of an embedding for a prompt
             # string from which the low-weighted fragment has been simply removed. The closer the weight is to zero, the
             # closer the resulting embedding is to an embedding for a prompt that simply lacks this fragment.
 
             # handle weights >=1
             tokens, per_token_weights, mask = self.get_token_ids_and_expand_weights(fragments, weights, device=device)
-            base_embedding = self.build_weighted_embedding_tensor(tokens, per_token_weights, mask)
+            base_embedding = self.build_weighted_embedding_tensor(tokens, per_token_weights, mask, device=device)
 
             # this is our starting point
             embeddings = base_embedding.unsqueeze(0)
             per_embedding_weights = [1.0]
 
             # now handle weights <1
             # Do this by building extra embeddings tensors that lack the words being <1 weighted. These will be lerped
@@ -134,22 +134,24 @@
                         mask_without_fragment[fragment_start_token_id:fragment_end_token_id+1] = 0
                         if not self.truncate_to_model_max_length:
                             # but don't mask chunk-delimiting eos/bos markers
                             mask_without_fragment[0::self.tokenizer.model_max_length] = 1
                             mask_without_fragment[self.tokenizer.model_max_length-1::self.tokenizer.model_max_length] = 1
                         embedding_without_this = self.build_weighted_embedding_tensor(tokens,
                                                                                       per_token_weights,
-                                                                                      mask_without_fragment)
+                                                                                      mask_without_fragment,
+                                                                                      device=device)
                     else:
                         fragments_without_this = fragments[0:index] + fragments[index+1:]
                         weights_without_this = weights[0:index] + weights[index+1:]
                         tokens_without_fragment, per_token_weights_without_fragment, mask_without_fragment = \
                             self.get_token_ids_and_expand_weights(fragments_without_this, weights_without_this, device=device)
                         embedding_without_this = self.build_weighted_embedding_tensor(tokens_without_fragment,
-                                                                                      per_token_weights_without_fragment)
+                                                                                      per_token_weights_without_fragment,
+                                                                                      device=device)
 
                     embeddings = torch.cat((embeddings, embedding_without_this.unsqueeze(0)), dim=1)
                     # weight of the embedding *without* this fragment gets *stronger* as its weight approaches 0
                     # if fragment_weight = 0, basically we want embedding_without_this to completely overwhelm base_embedding
                     # therefore:
                     # fragment_weight = 1: we are at base_z => lerp weight 0
                     # fragment_weight = 0.5: we are halfway between base_z and here => lerp weight 1
@@ -285,25 +287,26 @@
             all_masks += chunk_mask
 
             if self.truncate_to_model_max_length or len(remaining_token_ids) == 0:
                 break
 
         all_token_ids_tensor = torch.tensor(all_token_ids, dtype=torch.long, device=device)
         all_per_token_weights_tensor = torch.tensor(all_token_weights,
-                                                    dtype=self.get_dtype_for_device(self.text_encoder.device),
+                                                    dtype=self.get_dtype_for_device(device),
                                                     device=device)
         all_masks = torch.tensor(all_masks, dtype=torch.long, device=device)
         # print(f"assembled all_token_ids_tensor with shape {all_token_ids_tensor.shape}")
         return all_token_ids_tensor, all_per_token_weights_tensor, all_masks
 
 
     def build_weighted_embedding_tensor(self,
                                         token_ids: torch.Tensor,
                                         per_token_weights: torch.Tensor,
-                                        attention_mask: Optional[torch.Tensor] = None) -> torch.Tensor:
+                                        attention_mask: Optional[torch.Tensor] = None,
+                                        device: Optional[str] = None) -> torch.Tensor:
         """
         Build a tensor that embeds the passed-in token IDs and applies the given per_token weights
 
         :param token_ids: A tensor of shape `n*[self.max_length]` containing token IDs (ints) where n is some arbitrary
             integer (i.e. n==1 for shorter prompts, or it may be >1 if there are more than max_length tokens in the
             original prompt)
         :param per_token_weights: A tensor containing weights (floats), with the same shape as token_ids
@@ -313,19 +316,22 @@
         :return: A tensor of shape `[1, token_ids.shape[0], token_dim]` representing the requested weighted embeddings
             where `token_dim` is 768 for SD1 and 1280 for SD2.
         """
         # print(f"building weighted embedding tensor for {tokens} with weights {token_weights}")
         if token_ids.shape[0] % self.max_token_count != 0:
             raise ValueError(f"token_ids has shape {token_ids.shape} - expected a multiple of {self.max_token_count}")
 
+        if device is None:
+            device = self.text_encoder.device
+
         chunk_start_index = 0
         empty_token_ids = torch.tensor([self.tokenizer.bos_token_id] +
                                        [self.tokenizer.eos_token_id] +
                                        [self.tokenizer.pad_token_id] * (self.max_token_count - 2),
-                                       dtype=torch.int, device=self.text_encoder.device).unsqueeze(0)
+                                       dtype=torch.int, device=device).unsqueeze(0)
         empty_z = self._encode_token_ids_to_embeddings(empty_token_ids)
         weighted_z = None
 
         chunk_size = self.max_token_count
         while chunk_start_index < token_ids.shape[0]:
             next_chunk_start_index = chunk_start_index+chunk_size
             chunk_per_token_weights = per_token_weights[chunk_start_index:next_chunk_start_index]
```

### Comparing `compel-1.1.3.dev0/src/compel/prompt_parser.py` & `compel-1.1.4.dev0/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/src/compel.egg-info/PKG-INFO` & `compel-1.1.4.dev0/src/compel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.3.dev0
+Version: 1.1.4.dev0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -73,17 +73,17 @@
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
 ## Changelog
 
-#### 1.1.3 - enable fetching the penultimate CLIP hidden layers (improves generation quality on SD2.1) (aka "clip skip")
+#### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
-To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance.
+To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
 
 #### 1.1.2 - fix for #21 (crash when parsing long prompts with truncation enabled if there is weighted fragments beyond the truncation boundary)
 
 #### 1.1.1 - fix for #22 (issues parsing `.` characters inside parentheses)
 
 #### 1.1.0 - support for parsing `withLora`/`useLora` on `parse_prompt_string()`.
```

### Comparing `compel-1.1.3.dev0/test/test_compel.py` & `compel-1.1.4.dev0/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/test/test_embeddings_provider.py` & `compel-1.1.4.dev0/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.3.dev0/test/test_prompt_parser.py` & `compel-1.1.4.dev0/test/test_prompt_parser.py`

 * *Files identical despite different names*

