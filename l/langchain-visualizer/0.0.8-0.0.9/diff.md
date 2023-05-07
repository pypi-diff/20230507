# Comparing `tmp/langchain_visualizer-0.0.8.tar.gz` & `tmp/langchain_visualizer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_visualizer-0.0.8.tar", max compression
+gzip compressed data, was "langchain_visualizer-0.0.9.tar", max compression
```

## Comparing `langchain_visualizer-0.0.8.tar` & `langchain_visualizer-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-01-22 04:59:36.043304 langchain_visualizer-0.0.8/LICENSE
--rw-r--r--   0        0        0     3622 2023-02-06 09:25:39.438781 langchain_visualizer-0.0.8/README.md
--rw-r--r--   0        0        0      472 2023-02-03 09:01:32.038627 langchain_visualizer-0.0.8/langchain_visualizer/__init__.py
--rw-r--r--   0        0        0        0 2023-01-23 09:59:05.085353 langchain_visualizer-0.0.8/langchain_visualizer/agents/__init__.py
--rw-r--r--   0        0        0      285 2023-02-02 13:32:51.675223 langchain_visualizer-0.0.8/langchain_visualizer/agents/tools.py
--rw-r--r--   0        0        0      158 2023-02-02 13:23:07.588203 langchain_visualizer-0.0.8/langchain_visualizer/chains/__init__.py
--rw-r--r--   0        0        0      126 2023-02-02 13:23:04.548203 langchain_visualizer-0.0.8/langchain_visualizer/chains/base.py
--rw-r--r--   0        0        0      246 2023-02-03 09:07:41.776169 langchain_visualizer-0.0.8/langchain_visualizer/embeddings/__init__.py
--rw-r--r--   0        0        0     2102 2023-02-03 09:20:58.245606 langchain_visualizer-0.0.8/langchain_visualizer/hijacking.py
--rw-r--r--   0        0        0      864 2023-01-23 07:41:08.127604 langchain_visualizer-0.0.8/langchain_visualizer/ice.py
--rw-r--r--   0        0        0        0 2023-01-22 10:31:54.857541 langchain_visualizer-0.0.8/langchain_visualizer/llms/__init__.py
--rw-r--r--   0        0        0      723 2023-02-01 08:40:04.630088 langchain_visualizer-0.0.8/langchain_visualizer/llms/base.py
--rw-r--r--   0        0        0        0 2023-01-22 07:16:01.560480 langchain_visualizer-0.0.8/langchain_visualizer/prompts/__init__.py
--rw-r--r--   0        0        0     2378 2023-01-23 11:07:19.854620 langchain_visualizer-0.0.8/langchain_visualizer/prompts/few_shot.py
--rw-r--r--   0        0        0     1239 2023-01-23 11:07:19.854620 langchain_visualizer-0.0.8/langchain_visualizer/prompts/prompt.py
--rw-r--r--   0        0        0        0 2023-01-22 05:03:07.212712 langchain_visualizer-0.0.8/langchain_visualizer/py.typed
--rw-r--r--   0        0        0     1020 2023-02-06 09:44:24.932846 langchain_visualizer-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 langchain_visualizer-0.0.8/setup.py
--rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 langchain_visualizer-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-22 04:59:36.043304 langchain_visualizer-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3622 2023-02-06 09:25:39.438781 langchain_visualizer-0.0.9/README.md
+-rw-r--r--   0        0        0      472 2023-02-03 09:01:32.038627 langchain_visualizer-0.0.9/langchain_visualizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 09:59:05.085353 langchain_visualizer-0.0.9/langchain_visualizer/agents/__init__.py
+-rw-r--r--   0        0        0      285 2023-02-02 13:32:51.675223 langchain_visualizer-0.0.9/langchain_visualizer/agents/tools.py
+-rw-r--r--   0        0        0      158 2023-02-02 13:23:07.588203 langchain_visualizer-0.0.9/langchain_visualizer/chains/__init__.py
+-rw-r--r--   0        0        0      126 2023-02-02 13:23:04.548203 langchain_visualizer-0.0.9/langchain_visualizer/chains/base.py
+-rw-r--r--   0        0        0      246 2023-02-03 09:07:41.776169 langchain_visualizer-0.0.9/langchain_visualizer/embeddings/__init__.py
+-rw-r--r--   0        0        0     2102 2023-02-03 09:20:58.245606 langchain_visualizer-0.0.9/langchain_visualizer/hijacking.py
+-rw-r--r--   0        0        0      864 2023-01-23 07:41:08.127604 langchain_visualizer-0.0.9/langchain_visualizer/ice.py
+-rw-r--r--   0        0        0        0 2023-01-22 10:31:54.857541 langchain_visualizer-0.0.9/langchain_visualizer/llms/__init__.py
+-rw-r--r--   0        0        0      723 2023-02-01 08:40:04.630088 langchain_visualizer-0.0.9/langchain_visualizer/llms/base.py
+-rw-r--r--   0        0        0        0 2023-01-22 07:16:01.560480 langchain_visualizer-0.0.9/langchain_visualizer/prompts/__init__.py
+-rw-r--r--   0        0        0     2378 2023-01-23 11:07:19.854620 langchain_visualizer-0.0.9/langchain_visualizer/prompts/few_shot.py
+-rw-r--r--   0        0        0     1239 2023-01-23 11:07:19.854620 langchain_visualizer-0.0.9/langchain_visualizer/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2023-01-22 05:03:07.212712 langchain_visualizer-0.0.9/langchain_visualizer/py.typed
+-rw-r--r--   0        0        0     1020 2023-02-10 16:45:42.665174 langchain_visualizer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4612 1970-01-01 00:00:00.000000 langchain_visualizer-0.0.9/setup.py
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 langchain_visualizer-0.0.9/PKG-INFO
```

### Comparing `langchain_visualizer-0.0.8/LICENSE` & `langchain_visualizer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/README.md` & `langchain_visualizer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/langchain_visualizer/hijacking.py` & `langchain_visualizer-0.0.9/langchain_visualizer/hijacking.py`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/langchain_visualizer/ice.py` & `langchain_visualizer-0.0.9/langchain_visualizer/ice.py`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/langchain_visualizer/llms/base.py` & `langchain_visualizer-0.0.9/langchain_visualizer/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/langchain_visualizer/prompts/few_shot.py` & `langchain_visualizer-0.0.9/langchain_visualizer/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/langchain_visualizer/prompts/prompt.py` & `langchain_visualizer-0.0.9/langchain_visualizer/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_visualizer-0.0.8/pyproject.toml` & `langchain_visualizer-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "langchain-visualizer"
-version = "0.0.8"
+version = "0.0.9"
 description = "Visualization and debugging tool for LangChain workflows"
 authors = ["Amos Jun-yeung Ng <me@amos.ng>"]
 readme = "README.md"
 packages = [{include = "langchain_visualizer"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
-langchain = "^0.0.77"
+langchain = "^0.0.81"
 ought-ice = "^0.4.0"
 gorilla = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 black = "^22.12.0"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
 openai = "^0.26.1"
-vcr-langchain = "^0.0.11"
+vcr-langchain = "^0.0.12"
 google-search-results = "^2.4.1"
 faiss-cpu = "^1.7.3"
 tiktoken = "^0.1.2"
 
 [tool.pytest.ini_options]
 markers = [
     "network: marks tests as requiring network services",
```

### Comparing `langchain_visualizer-0.0.8/setup.py` & `langchain_visualizer-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
  'langchain_visualizer.prompts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['gorilla>=0.4.0,<0.5.0',
- 'langchain>=0.0.77,<0.0.78',
+ 'langchain>=0.0.81,<0.0.82',
  'ought-ice>=0.4.0,<0.5.0']
 
 setup_kwargs = {
     'name': 'langchain-visualizer',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Visualization and debugging tool for LangChain workflows',
     'long_description': '# LangChain Visualizer\n\nAdapts [ICE](https://github.com/oughtinc/ice) for use with [LangChain](https://github.com/hwchase17/langchain) so that you can view LangChain interactions with a beautiful UI.\n\n![Screenshot of an execution run](screenshots/serp_screenshot.png "SERP agent demonstration")\n\nYou can now\n\n- See the full prompt text being sent with every interaction with the LLM\n- Tell from the coloring which parts of the prompt are hardcoded and which parts are templated substitutions\n- Inspect the execution flow and observe when each function goes up the stack\n\n## Quickstart\n\nInstall this library:\n\n```bash\npip install langchain-visualizer\n```\n\nThen:\n\n1. Add `import langchain_visualizer` as **the first import** in your Python entrypoint file\n2. Write an async function to visualize whichever workflow you\'re running\n3. Call `langchain_visualizer.visualize` on that function\n\nFor an example, see below instructions on reproducing the screenshot.\n\n\n### Running the example screenshot\n\nTo run the example you see in the screenshot, first install this library and optional dependencies:\n\n```bash\npip install langchain-visualizer google-search-results openai\n```\n\nIf you haven\'t yet set up your [OpenAI API keys](https://openai.com/api/) or SERP API keys, you can [replay the recorded interactions](https://github.com/amosjyng/vcr-langchain) by cloning this repository and running\n\n```bash\npython tests/agents/test_langchain_getting_started.py\n```\n\nIf you have set them up, you can run the following script (adapted from [LangChain docs](https://langchain.readthedocs.io/en/latest/modules/agents/getting_started.html)):\n\n```python\nimport langchain_visualizer\nimport asyncio\nfrom langchain.agents import initialize_agent, load_tools\nfrom langchain.llms import OpenAI\n\nllm = OpenAI(temperature=0.7)\ntools = load_tools(["serpapi", "llm-math"], llm=llm)\nagent = initialize_agent(tools, llm, agent="zero-shot-react-description", verbose=True)\nasync def search_agent_demo():\n    return agent.run(\n        "Who is Olivia Wilde\'s boyfriend? What is his current age raised to the 0.23 "\n        "power?"\n    )\n\nlangchain_visualizer.visualize(search_agent_demo)\n```\n\nA browser window will open up, and you can actually see the agent execute happen in real-time!\n\n### Visualizing embeddings\n\nIf you want to also visualize documents being chunked up for embeddings, you can now do so by calling the `visualize_embeddings` function before you visualize the main chain:\n\n```python\nfrom langchain_visualizer import visualize, visualize_embeddings\n\nasync def run_chain():\n    ...\n\nvisualize_embeddings()\nvisualize(run_chain)\n```\n\n## Why not just use LangChain\'s built-in tracer?\n\nFor me personally:\n\n- I prefer the ICE UI. In particular:\n    - I like the colored highlighting of parts of the prompt that are filled-in template variables\n    - I like the ability to quickly inspect different LLM calls without leaving the trace page\n- I prefer the visualization of my agent logic to remain static when LLM calls are cached\n- I prefer seeing when the tool (e.g. `PythonREPL`) actually gets called, rather than just the high-level execution of the chain (e.g. `LLMMathChain`)\n\nThat being said, LangChain\'s tracer is definitely better supported. **Please note that there is a lot of langchain functionality that I haven\'t gotten around to hijacking for visualization.** If there\'s anything you need to show up in the execution trace, please open a PR or issue.\n\n## My other projects\n\nPlease check out [VCR LangChain](https://github.com/amosjyng/vcr-langchain), a library that lets you record LLM interactions for your tests and demos!\n',
     'author': 'Amos Jun-yeung Ng',
     'author_email': 'me@amos.ng',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `langchain_visualizer-0.0.8/PKG-INFO` & `langchain_visualizer-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: langchain-visualizer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Visualization and debugging tool for LangChain workflows
 Author: Amos Jun-yeung Ng
 Author-email: me@amos.ng
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: gorilla (>=0.4.0,<0.5.0)
-Requires-Dist: langchain (>=0.0.77,<0.0.78)
+Requires-Dist: langchain (>=0.0.81,<0.0.82)
 Requires-Dist: ought-ice (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # LangChain Visualizer
 
 Adapts [ICE](https://github.com/oughtinc/ice) for use with [LangChain](https://github.com/hwchase17/langchain) so that you can view LangChain interactions with a beautiful UI.
```

