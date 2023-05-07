# Comparing `tmp/coreftools-0.2.5-py3-none-any.whl.zip` & `tmp/coreftools-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5369 bytes, number of entries: 6
+Zip file size: 5927 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
--rw-r--r--  2.0 unx     6996 b- defN 23-May-05 19:20 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3676 b- defN 23-May-05 20:13 coreftools-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 20:13 coreftools-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-05 20:13 coreftools-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 20:13 coreftools-0.2.5.dist-info/RECORD
-6 files, 11246 bytes uncompressed, 4511 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     8669 b- defN 23-May-07 12:48 coreftools/corefresolvers.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-May-07 12:53 coreftools-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 12:53 coreftools-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-07 12:53 coreftools-0.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      471 b- defN 23-May-07 12:53 coreftools-0.2.7.dist-info/RECORD
+6 files, 12796 bytes uncompressed, 5069 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.2.5.dist-info/METADATA
+Filename: coreftools-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.2.5.dist-info/WHEEL
+Filename: coreftools-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.2.5.dist-info/top_level.txt
+Filename: coreftools-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: coreftools-0.2.5.dist-info/RECORD
+Filename: coreftools-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coreftools/corefresolvers.py

```diff
@@ -3,19 +3,26 @@
 import neuralcoref
 from typing import List
 from spacy.tokens import Doc, Span
 import pandas as pd
 import os
 import openai
 import re
-#print(openai.api_key )
 
 class SpanBERTResolver:
+    """
+    Add desc here
+    """
     def __init__(self, model_url: str = 'default_model_url'):
-        self.nlp = spacy.load('en_core_web_sm')
+        try:
+            self.nlp = spacy.load('en_core_web_sm')
+        except OSError:
+            print("Model not found. Downloading 'en-small' model...")
+            spacy.cli.download("en_core_web_sm")
+            self.nlp = spacy.load('en_core_web_sm')
         neuralcoref.add_to_pipe(self.nlp)
         if model_url == 'default_model_url':
             model_url = 'https://storage.googleapis.com/allennlp-public-models/coref-spanbert-large-2020.02.27.tar.gz'
         self.predictor = Predictor.from_path(model_url)
 
     def core_logic_part(self, document: Doc, coref: List[int], resolved: List[str], mention_span: Span):
         final_token = document[coref[1]]
@@ -103,39 +110,47 @@
     Resolved answer: Tell me more about BMW iX technology toolkit
     ###\n
     """
 
 
 class GPTResolver:
     """
-    Currently raises: openai.error.AuthenticationError: Incorrect API key provided: <module
+    Add desc here
     """
     def __init__(self):
         openai.api_key = os.getenv("OPENAI_API_KEY")
 
     def resolve_coref(self, query_to_resolve:str, few_shot_prompt:str = None, engine:str="text-davinci-003") -> str :
         if not few_shot_prompt:
             few_shot_prompt = """
             
-{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {John and Jane went to the park. They had a picnic and played frisbee. When they were done, they walked home together.}", "output": "Resolved query: {John and Jane went to the park. John and Jane had a picnic and played frisbee. When John and Jane were done, John and Jane walked home together.}" }
-{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {My car needs an oil change. When can I have the next appointment for it? }", "output": "Resolved query: {My car needs an oil change. When can I have the next appointment for an oil change?}" }
+{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {John and Jane went to the park. They had a picnic and played frisbee. When they were done, they walked home together.}", "output": "Resolved_query: {John and Jane went to the park. John and Jane had a picnic and played frisbee. When John and Jane were done, John and Jane walked home together.}" }
+{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {My car needs an oil change. When can I have the next appointment for it? }", "output": "Resolved_query: {My car needs an oil change. When can I have the next appointment for an oil change?}" }
 
 """
         formatted_input_query = f'{{"input": "Resolve the coreferences in the following sentence and do not paraphrase: {query_to_resolve}"}}'
         gpt_prompt = few_shot_prompt + formatted_input_query
         response = openai.Completion.create(
             engine=engine,
             prompt=gpt_prompt,
             temperature=0.5,
             max_tokens=256,
             top_p=1.0,
             frequency_penalty=0.0,
             presence_penalty=0.0
         )
         response = response['choices'][0]['text']
-        clean_response = re.sub(r'[^a-zA-Z0-9\s]', '', response.split(": ")[2])
+        print("actual-response",response)
+        try:
+            clean_response = response[response.index("Resolved_query: ") + len("Resolved_query: "):]  ### accepts all the string after "Resolved_query:"" in the output
+            clean_response = re.sub(r'(\w)[^\w]*$', r'\1', clean_response) ### cleans all the entailing special character after an english word
+        except ValueError:
+            raise ValueError("The generated output is in a format that is not supported by the system.")
+        print(clean_response)
         return clean_response
     
 
 # query_to_resolve = "The chef prepared a delicious meal. It included steak, mashed potatoes, and green beans."
+# query_to_resolve = "Wouldn't it be incredible if your BMW was also your personal assistant? Imagine if it could understand you, help you and think with you. That is exactly what the BMW Intelligent Personal Assistant does. Activate it with the voice command 'Hey, BMW' and it will be there for you, ready to help with any needs or questions about your vehicle. You can personalise it and give it a new name ('Hey, BMW. Change the activation word.'). \n\nYour personal assistant is a vehicle expert with whom you can operate numerous vehicle functions using natural voice commands. It also helps you to get to know and use your BMW better. It can explain features ('Hey BMW. How does the High-beam Assistant work?') and understands your vehicle's status ('Hey, BMW. Is my tyre pressure okay?'). \n\n\nSimply say: 'Hey, BMW. I'm hungry,' and your Personal Assistant immediately plans the route and finds the best-rated restaurants on request. Through regular updates, the BMW Intelligent Personal Assistant will be able to handle a growing number of commands and functions."
+
 # GPT = GPTResolver()
 # print("GPT3:",GPT.resolve_coref(query_to_resolve))
```

## Comparing `coreftools-0.2.5.dist-info/METADATA` & `coreftools-0.2.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.2.5
+Version: 0.2.7
 Summary: Coreference-Resolution library
-Download-URL: https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.1.0/en_core_web_sm-2.1.0.tar.gz
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
 Requires-Dist: allennlp
 Requires-Dist: allennlp-models
```

