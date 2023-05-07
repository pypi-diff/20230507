# Comparing `tmp/promptwatch-0.0.6.tar.gz` & `tmp/promptwatch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.6.tar", last modified: Sat May  6 17:47:53 2023, max compression
+gzip compressed data, was "promptwatch-0.0.7.tar", last modified: Sun May  7 09:56:19 2023, max compression
```

## Comparing `promptwatch-0.0.6.tar` & `promptwatch-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 17:47:53.434794 promptwatch-0.0.6/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-06 17:47:53.434645 promptwatch-0.0.6/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.6/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.6/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-06 17:47:53.434835 promptwatch-0.0.6/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.6/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 17:47:53.429925 promptwatch-0.0.6/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 17:47:53.432155 promptwatch-0.0.6/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-06 17:47:49.000000 promptwatch-0.0.6/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.6/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.6/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.6/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 21:26:09.000000 promptwatch-0.0.6/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 17:47:53.433932 promptwatch-0.0.6/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.6/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    34188 2023-05-06 16:57:39.000000 promptwatch-0.0.6/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    14375 2023-05-06 13:44:12.000000 promptwatch-0.0.6/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.6/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 17:47:53.433527 promptwatch-0.0.6/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-06 17:47:53.000000 promptwatch-0.0.6/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-06 17:47:53.000000 promptwatch-0.0.6/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-06 17:47:53.000000 promptwatch-0.0.6/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.6/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-06 17:47:53.000000 promptwatch-0.0.6/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-06 17:47:53.000000 promptwatch-0.0.6/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.950408 promptwatch-0.0.7/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-07 09:56:19.950230 promptwatch-0.0.7/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.7/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.7/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-07 09:56:19.950457 promptwatch-0.0.7/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.7/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.945527 promptwatch-0.0.7/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.948462 promptwatch-0.0.7/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-07 09:54:30.000000 promptwatch-0.0.7/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.7/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1605 2023-05-07 09:39:06.000000 promptwatch-0.0.7/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.949971 promptwatch-0.0.7/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.7/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    34257 2023-05-07 09:37:59.000000 promptwatch-0.0.7/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    14375 2023-05-06 13:44:12.000000 promptwatch-0.0.7/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.7/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-07 09:56:19.949491 promptwatch-0.0.7/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.7/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-07 09:56:19.000000 promptwatch-0.0.7/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.6/PKG-INFO` & `promptwatch-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.6
+Version: 0.0.7
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.6/README.md` & `promptwatch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/setup.py` & `promptwatch-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch/caching.py` & `promptwatch-0.0.7/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch/client.py` & `promptwatch-0.0.7/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch/data_model.py` & `promptwatch-0.0.7/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.0.7/src/promptwatch/langchain/langchain_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from langchain.schema import PromptValue
 from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
 from ..data_model import NamedPromptTemplateDescription,PromptTemplateDescription, LlmPrompt, ParallelPrompt, ChainSequence, ChatMessage, Answer, Action, Question, RetrievedDocuments, DocumentSnippet, ChatMessagePromptTemplate
 from ..utils import find_the_caller_in_the_stack, is_primitive_type, wrap_a_method
 
-from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY
+from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY
 
 from typing import List, Dict
 from .. import PromptWatch
 from langchain.cache import BaseCache
 from langchain.schema import Generation
 from collections import OrderedDict
 
@@ -146,38 +146,39 @@
 
         prompt_template = None
         prompt_input_values=None
         llm_info=None
         info_message=None
         formatted_prompt=None
 
+        current_llm_chain:LLMChain= self.prompt_watch.get_context(LLM_CHAIN_CONTEXT_KEY)
         # this should ensure that all the additional data is available in the context
-        if self.current_llm_chain:
-            if self.current_llm_chain.llm and self.current_llm_chain.llm.dict:
-                llm = self.current_llm_chain.llm
-                if hasattr(self.current_llm_chain.llm,"inner_llm"): # cachedLLM
+        if current_llm_chain:
+            if current_llm_chain.llm and current_llm_chain.llm.dict:
+                llm = current_llm_chain.llm
+                if hasattr(current_llm_chain.llm,"inner_llm"): # cachedLLM
                     llm = llm.inner_llm
                 llm_info = {k:v for k,v in llm.dict().items() if is_primitive_type(v)}
                 llm_info["stop"] = self.prompt_watch.current_activity.inputs.get("stop")
             # lets try to retrieve registered named template first... it's faster
             template_name = self.prompt_watch.get_context(TEMPLATE_NAME_CONTEXT_KEY)
             if template_name:
                 prompt_template = PromptWatch.prompt_template_register_cache.get(template_name)
 
             if not prompt_template:
                 # lets create anonymous prompt template description
-                prompt_template = create_prompt_template_description(self.current_llm_chain.prompt)
+                prompt_template = create_prompt_template_description(current_llm_chain.prompt)
 
             prompt_input_values = self.prompt_watch.current_activity.inputs
 
             formatted_prompt = self.prompt_watch.get_context(FORMATTED_PROMPT_CONTEXT_KEY)
-            if isinstance(self.current_llm_chain.prompt,ChatPromptTemplate):
+            if isinstance(current_llm_chain.prompt,ChatPromptTemplate):
                 if not formatted_prompt:
                     # we need to reformat the prompt so we can get the original values, not the strings
-                    formatted_prompt = self.current_llm_chain.prep_prompts([prompt_input_values])[0][0]
+                    formatted_prompt = current_llm_chain.prep_prompts([prompt_input_values])[0][0]
                 if formatted_prompt:
                     #throwing away the original prompt from langchain tracing and replacing it with the original formatted messages
                     prompts = [convert_chat_messages(formatted_prompt.messages)]
             
             
             
             
@@ -234,16 +235,15 @@
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
         if len(response.generations)>1:
             thoughts =  self.prompt_watch.current_activity.thoughts
         else:
             thoughts=[self.prompt_watch.current_activity]
         
-        if hasattr(self,"current_llm_chain"):
-            self.current_llm_chain = None
+        
         if not self.prompt_watch.current_activity.metadata:
             self.prompt_watch.current_activity.metadata={}
 
         for thought, generated_responses in zip(thoughts, response.generations):
             thought.generated = "\n---\n".join([resp.text for resp in generated_responses])
             thought.metadata["generation_info"] = [resp.generation_info for resp in generated_responses] if len(generated_responses)>1 else generated_responses[0].generation_info
 
@@ -269,15 +269,16 @@
     
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
         
         if serialized.get("name").startswith("LLM") :
-            self.current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
+            current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
+            self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
                   
 
 
         question = inputs.get("question") 
         if not question and "chat_history" in inputs:
@@ -323,16 +324,16 @@
                     metadata=metadata if metadata else None # to not pass empty objects
                     ))
             self.prompt_watch._add_activity(RetrievedDocuments(documents=docs))
     
     def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
         
-        if self.current_llm_chain:
-            self.current_llm_chain =None
+        
+        self.prompt_watch._remove_context(LLM_CHAIN_CONTEXT_KEY)
             
         self.prompt_watch.current_activity.outputs=outputs
         if outputs.get("answer"):
             self.prompt_watch._add_activity(Answer(text=outputs["answer"]),as_root=True)
         if kwargs:
             self.prompt_watch.current_activity.metadata["output_kwargs"]=kwargs
```

### Comparing `promptwatch-0.0.6/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.7/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch/utils.py` & `promptwatch-0.0.7/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.6/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.7/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.6
+Version: 0.0.7
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.6/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.0.7/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

