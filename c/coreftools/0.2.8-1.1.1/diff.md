# Comparing `tmp/coreftools-0.2.8-py3-none-any.whl.zip` & `tmp/coreftools-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6025 bytes, number of entries: 6
+Zip file size: 6003 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
--rw-r--r--  2.0 unx     8928 b- defN 23-May-07 13:35 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3553 b- defN 23-May-07 13:39 coreftools-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 13:39 coreftools-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-07 13:39 coreftools-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-07 13:39 coreftools-0.2.8.dist-info/RECORD
-6 files, 13055 bytes uncompressed, 5167 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx     8862 b- defN 23-May-07 13:49 coreftools/corefresolvers.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-May-07 13:52 coreftools-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 13:52 coreftools-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-07 13:52 coreftools-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      471 b- defN 23-May-07 13:52 coreftools-1.1.1.dist-info/RECORD
+6 files, 12989 bytes uncompressed, 5145 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.2.8.dist-info/METADATA
+Filename: coreftools-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.2.8.dist-info/WHEEL
+Filename: coreftools-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.2.8.dist-info/top_level.txt
+Filename: coreftools-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: coreftools-0.2.8.dist-info/RECORD
+Filename: coreftools-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coreftools/corefresolvers.py

```diff
@@ -87,17 +87,17 @@
             clusters = self.predictor.predict(query)['clusters']
         except AssertionError as e:
             return ""
         doc = self.nlp(query)
         return self.improved_replace_corefs(doc,clusters)
     
 
-query_to_resolve = "When is the next service appointment, vehicle check or oil change? With Teleservices, your BMW knows exactly when the next inspection is due. When maintenance work is required or if there is a malfunction, it sends all relevant data to you and your preferred service partner. Even before your BMW Service Partner calls you to make an appointment, he or she already knows the condition of your vehicle, can order spare parts and is perfectly prepared to meet the individual requirements of your vehicle. This also shortens the wait time during the appointment."
-allennlp =  SpanBERTResolver()
-print("SPANBERT:",allennlp.resolve_coref(query_to_resolve))
+# query_to_resolve = "When is the next service appointment, vehicle check or oil change? With Teleservices, your BMW knows exactly when the next inspection is due. When maintenance work is required or if there is a malfunction, it sends all relevant data to you and your preferred service partner. Even before your BMW Service Partner calls you to make an appointment, he or she already knows the condition of your vehicle, can order spare parts and is perfectly prepared to meet the individual requirements of your vehicle. This also shortens the wait time during the appointment."
+# allennlp =  SpanBERTResolver()
+# print("SPANBERT:",allennlp.resolve_coref(query_to_resolve))
 
 
 
 
 
 ### Check how they pass on the prompts in BMW repo ###
 
@@ -139,21 +139,19 @@
             temperature=0.5,
             max_tokens=256,
             top_p=1.0,
             frequency_penalty=0.0,
             presence_penalty=0.0
         )
         response = response['choices'][0]['text']
-        print("actual-response",response)
         try:
             clean_response = response[response.index("Resolved_query: ") + len("Resolved_query: "):]  ### accepts all the string after "Resolved_query:"" in the output
             clean_response = re.sub(r'(\w)[^\w]*$', r'\1', clean_response) ### cleans all the entailing special character after an english word
         except ValueError:
             raise ValueError("The generated output is in a format that is not supported by the system.")
-        print(clean_response)
         return clean_response
     
 
 # query_to_resolve = "The chef prepared a delicious meal. It included steak, mashed potatoes, and green beans."
 # query_to_resolve = "Wouldn't it be incredible if your BMW was also your personal assistant? Imagine if it could understand you, help you and think with you. That is exactly what the BMW Intelligent Personal Assistant does. Activate it with the voice command 'Hey, BMW' and it will be there for you, ready to help with any needs or questions about your vehicle. You can personalise it and give it a new name ('Hey, BMW. Change the activation word.'). \n\nYour personal assistant is a vehicle expert with whom you can operate numerous vehicle functions using natural voice commands. It also helps you to get to know and use your BMW better. It can explain features ('Hey BMW. How does the High-beam Assistant work?') and understands your vehicle's status ('Hey, BMW. Is my tyre pressure okay?'). \n\n\nSimply say: 'Hey, BMW. I'm hungry,' and your Personal Assistant immediately plans the route and finds the best-rated restaurants on request. Through regular updates, the BMW Intelligent Personal Assistant will be able to handle a growing number of commands and functions."
 
 # GPT = GPTResolver()
```

## Comparing `coreftools-0.2.8.dist-info/METADATA` & `coreftools-1.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.2.8
+Version: 1.1.1
 Summary: Coreference-Resolution library
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
 Requires-Dist: allennlp
```

