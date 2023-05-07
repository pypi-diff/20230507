# Comparing `tmp/pyllms-0.2.0.tar.gz` & `tmp/pyllms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.2.0.tar", last modified: Tue Apr 25 01:27:17 2023, max compression
+gzip compressed data, was "pyllms-0.2.1.tar", last modified: Sun May  7 04:01:34 2023, max compression
```

## Comparing `pyllms-0.2.0.tar` & `pyllms-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.287240 pyllms-0.2.0/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.0/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    16542 2023-04-25 01:27:17.286931 pyllms-0.2.0/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    15229 2023-04-25 00:51:55.000000 pyllms-0.2.0/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.283096 pyllms-0.2.0/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.0/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    18832 2023-04-25 01:23:34.000000 pyllms-0.2.0/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.285346 pyllms-0.2.0/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.2.0/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2336 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2672 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/aleph.py
--rw-r--r--   0 prelovac   (502) staff       (20)     8069 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)      950 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/base_provider.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3664 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/cohere.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2514 2023-04-25 01:23:39.000000 pyllms-0.2.0/llms/providers/huggingface.py
--rw-r--r--   0 prelovac   (502) staff       (20)     5692 2023-04-25 00:51:55.000000 pyllms-0.2.0/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-25 01:27:17.286612 pyllms-0.2.0/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    16542 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      419 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       85 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-25 01:27:17.000000 pyllms-0.2.0/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-25 01:27:17.287307 pyllms-0.2.0/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1882 2023-04-25 01:24:12.000000 pyllms-0.2.0/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-07 04:01:34.472844 pyllms-0.2.1/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.2.1/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    16541 2023-05-07 04:01:34.472571 pyllms-0.2.1/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    15228 2023-04-29 05:43:17.000000 pyllms-0.2.1/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-07 04:01:34.468803 pyllms-0.2.1/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.2.1/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    18384 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-07 04:01:34.470981 pyllms-0.2.1/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      228 2023-04-23 02:39:46.000000 pyllms-0.2.1/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2159 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3769 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     9105 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1565 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/base_provider.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4701 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2989 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     7943 2023-05-07 04:00:58.000000 pyllms-0.2.1/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-05-07 04:01:34.472242 pyllms-0.2.1/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    16541 2023-05-07 04:01:34.000000 pyllms-0.2.1/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      419 2023-05-07 04:01:34.000000 pyllms-0.2.1/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-05-07 04:01:34.000000 pyllms-0.2.1/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       85 2023-05-07 04:01:34.000000 pyllms-0.2.1/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-05-07 04:01:34.000000 pyllms-0.2.1/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-05-07 04:01:34.472913 pyllms-0.2.1/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1882 2023-05-07 04:01:09.000000 pyllms-0.2.1/setup.py
```

### Comparing `pyllms-0.2.0/LICENSE` & `pyllms-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.2.0/PKG-INFO` & `pyllms-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
@@ -40,15 +40,15 @@
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
-pip3 install pyllms
+pip install pyllms
 ```
 
 
 ## Usage
 
 
 ```
```

### Comparing `pyllms-0.2.0/README.md` & `pyllms-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
-pip3 install pyllms
+pip install pyllms
 ```
 
 
 ## Usage
 
 
 ```
```

### Comparing `pyllms-0.2.0/llms/llms.py` & `pyllms-0.2.1/llms/llms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 import statistics
 from prettytable import PrettyTable
 from .providers import OpenAIProvider
 from .providers import AnthropicProvider
 from .providers import AI21Provider
 from .providers import CohereProvider
@@ -14,23 +15,25 @@
 
 class Result:
     def __init__(self, results):
         self._results = results
 
     @property
     def text(self):
-        if len(self._results) == 1:
-            return self._results[0]["text"]
-        return [result["text"] for result in self._results]
+        if isinstance(self._results, list):
+            return [result["text"] for result in self._results]
+        else:
+            return self._results["text"]
 
     @property
     def meta(self):
-        if len(self._results) == 1:
-            return self._results[0]["meta"]
-        return [result["meta"] for result in self._results]
+        if isinstance(self._results, list):
+            return [result["meta"] for result in self._results]
+        else:
+            return self._results["meta"]
 
 
 class LLMS:
     def __init__(
         self,
         model=None,
         openai_api_key=None,
@@ -108,14 +111,18 @@
                 )
             else:
                 raise ValueError("Invalid API key and model combination", single_model)
 
     def __repr__(self) -> str:
         return f"LLMS({self.model})"
 
+    @property
+    def n_provider(self):
+        return len(self._providers)
+
     def list(self, query=None):
         model_info_list = []
 
         all_providers = [
             OpenAIProvider,
             AI21Provider,
             AnthropicProvider,
@@ -143,71 +150,53 @@
         )
         return sorted_list
 
     def count_tokens(self, content):
         results = []
         for provider in self._providers:
             results.append(provider.count_tokens(content))
-        if len(self._providers) > 1:
+        if self.n_provider > 1:
             return results
         else:
             return results[0]
 
     def complete(self, prompt, **kwargs):
         def _generate(provider):
-            response = provider.complete(prompt, **kwargs)
+            result = provider.complete(prompt, **kwargs)
+            return result
 
-            formatted_cost = format(response["meta"]["cost"], ".5f")
-            formatted_latency = round(response["meta"]["latency"], 2)
-
-            response["meta"]["cost"] = formatted_cost
-            response["meta"]["latency"] = formatted_latency
-
-            return {
-                "text": response["text"],
-                "meta": response["meta"],
-                "provider": provider,
-            }
-
-        results = []
-        with ThreadPoolExecutor() as executor:
-            futures = {
-                executor.submit(_generate, provider): provider
-                for provider in self._providers
-            }
-            for future in as_completed(futures):
-                results.append(future.result())
+        if self.n_provider > 1:
+            results = []
+            with ThreadPoolExecutor() as executor:
+                futures = {
+                    executor.submit(_generate, provider): provider
+                    for provider in self._providers
+                }
+                for future in as_completed(futures):
+                    results.append(future.result())
 
-        return Result(results)
+            return Result(results)
+        else:
+            result = self._providers[0].complete(prompt, **kwargs)
+            return Result(result)
 
     async def acomplete(
         self,
         prompt: str,
         **kwargs,
     ):
-        if len(self._providers) > 1:
-            raise NotImplementedError("acomplete not supported for multi-models yet.")
-        provider = self._providers[0]
-        response = await provider.acomplete(prompt, **kwargs)
-
-        formatted_cost = format(response["meta"]["cost"], ".5f")
-        formatted_latency = round(response["meta"]["latency"], 2)
-
-        response["meta"]["cost"] = formatted_cost
-        response["meta"]["latency"] = formatted_latency
-
-        return Result(
-            [
-                {
-                    "text": response["text"],
-                    "meta": response["meta"],
-                    "provider": provider,
-                }
-            ]
-        )
+        if self.n_provider > 1:
+            tasks = [provider.acomplete(prompt, **kwargs) for provider in self._providers]
+            results = await asyncio.gather(*tasks, return_exceptions=False)
+            return Result(results)
+
+        else:
+            provider = self._providers[0]
+            result = await provider.acomplete(prompt, **kwargs)
+            return Result(result)
 
     def complete_stream(self, prompt, **kwargs):
         if len(self._providers) > 1:
             raise ValueError("Streaming is possible only with a single model")
 
         yield from self._providers[0].complete_stream(prompt, **kwargs)
 
@@ -259,21 +248,18 @@
 
 
 Your only output should be a list of comma seperated integers representing your evaluation score for each answer. No other output is allowed. For example above your output will be:
 0, 1
 
 """
 
-            prompt = ""
-            for i, (query, answer) in enumerate(query_answer_pairs):
-                prompt += f"Query #{i + 1}: {query}\nAnswer #{i + 1}: {answer}\n\n"
-            # print(prompt)
+            prompt = "".join(f"Query #{i}: {query}\nAnswer #{i}: {answer}\n\n"
+                             for i, (query, answer) in enumerate(query_answer_pairs, start=1))
 
             evaluator_result = evaluator.complete(prompt, system_message=system).text
-            # print(evaluator_result)
             scores = evaluator_result.split(",")
             return [int(score.strip()) for score in scores]
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
             print(model, index)
```

### Comparing `pyllms-0.2.0/llms/providers/ai21.py` & `pyllms-0.2.1/llms/providers/huggingface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,105 @@
-# llms/providers/anthropic.py
+# llms/providers/huggingface.py
 
-import ai21
-import time
-import itertools
-from typing import List, Optional
+import os
+
+from huggingface_hub.inference_api import InferenceApi
 
 from .base_provider import BaseProvider
 
 
-class AI21Provider(BaseProvider):
-    # per million tokens
+class HuggingfaceHubProvider(BaseProvider):
     MODEL_INFO = {
-        "j2-grande-instruct": {"prompt": 10.0, "completion": 10.0, "token_limit": 8192},
-        "j2-jumbo-instruct": {"prompt": 15.0, "completion": 15.0, "token_limit": 8192},
+        "hf_pythia": {
+            "full": "OpenAssistant/oasst-sft-4-pythia-12b-epoch-3.5",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": 2048,
+        },
+        "hf_dolly": {
+            "full": "databricks/dolly-v2-12b",
+            "prompt": 0,
+            "completion": 0,
+            "token_limit": -1,
+        },
     }
 
-    def __init__(self, api_key, model=None):
-        ai21.api_key = api_key
+    def __init__(self, api_key=None, model=None):
         if model is None:
             model = list(self.MODEL_INFO.keys())[0]
+
         self.model = model
 
-    def complete(
+        if api_key is None:
+            api_key = os.getenv("HUGGINFACEHUB_API_KEY")
+
+        self.client = InferenceApi(
+            repo_id=self.MODEL_INFO[model]["full"], token=api_key
+        )
+
+    def _prepare_model_input(
         self,
         prompt: str,
-        history: Optional[List[tuple]] = None,
-        temperature: float = 0,
+        temperature: float = 0.01,
         max_tokens: int = 300,
         **kwargs,
     ):
-        HUMAN_PROMPT = "\n\nHuman:"
-        AI_PROMPT = "\n\nAssistant:"
+        if self.model == "hf_pythia":
+            prompt = "<|prompter|" + prompt + "<|endoftext|><|assistant|>"
+        temperature = max(temperature, 0.01)
+        max_new_tokens = kwargs.pop("max_new_tokens", max_tokens)
+        params = {
+            "temperature": temperature,
+            "max_new_tokens": max_new_tokens,
+            **kwargs,
+        }
+        return prompt, params
 
-        if history is not None:
-            role_cycle = itertools.cycle((HUMAN_PROMPT, AI_PROMPT))
-            history_messages = itertools.chain.from_iterable(history)
-            history_prompt = "".join(
-                itertools.chain.from_iterable(zip(role_cycle, history_messages))
-            )
-            prompt = f"{history_prompt}{prompt}"
-
-        if "maxTokens" not in kwargs:
-            kwargs["maxTokens"] = max_tokens  # Add maxTokens to kwargs if not present
-
-        start_time = time.time()
-        response = ai21.Completion.execute(
-            model=self.model, prompt=prompt, temperature=temperature, **kwargs
+    def complete(
+        self,
+        prompt: str,
+        temperature: float = 0.01,
+        max_tokens: int = 300,
+        **kwargs,
+    ):
+        prompt, params = self._prepare_model_input(
+            prompt=prompt,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            **kwargs,
         )
-        latency = time.time() - start_time
+        with self.track_latency as latency:
+            response = self.client(inputs=prompt, params=params)
+
+        if "error" in response:
+            print("Error: ", response["error"])
+            return {}
+
+        completion = response[0]["generated_text"][len(prompt) :]
+
+        # Calculate tokens and cost
+        prompt_tokens = -1
+        completion_tokens = -1
 
-        completion = response.completions[0].data.text.strip()
-        prompt_tokens = len(response.prompt.tokens)
-        completion_tokens = len(response.completions[0].data.tokens)
         total_tokens = prompt_tokens + completion_tokens
 
+        cost = self.compute_cost(prompt_tokens=prompt_tokens,
+                                 completion_tokens=completion_tokens
+                                 )
         cost_per_token = self.MODEL_INFO[self.model]
-        cost = (prompt_tokens * cost_per_token["prompt"] / 1000000) + (
-            completion_tokens * cost_per_token["completion"] / 1000000
-        )
+        cost = (
+            (prompt_tokens * cost_per_token["prompt"])
+            + (completion_tokens * cost_per_token["completion"])
+        ) / 1_000_000
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
                 "latency": latency,
             },
+            "provider": str(self),
         }
```

### Comparing `pyllms-0.2.0/pyllms.egg-info/PKG-INFO` & `pyllms-0.2.1/pyllms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub
@@ -40,15 +40,15 @@
 Feel free to reuse and expand. Pull requests are welcome.
 
 ## Installation
 
 Clone this repository and install the package using pip:
 
 ```
-pip3 install pyllms
+pip install pyllms
 ```
 
 
 ## Usage
 
 
 ```
```

### Comparing `pyllms-0.2.0/setup.py` & `pyllms-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.2.0",
+    version="0.2.1",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

