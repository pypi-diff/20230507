# Comparing `tmp/srtk-0.0.3.tar.gz` & `tmp/srtk-0.0.4.tar.gz`

## Comparing `srtk-0.0.3.tar` & `srtk-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,81 @@
--rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 srtk-0.0.3/graphs-for-paper.ipynb
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 srtk-0.0.3/linked.jsonl
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 srtk-0.0.3/question.jsonl
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.3/requirements.txt
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 srtk-0.0.3/sample_commands.ipynb
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 srtk-0.0.3/test.pdf
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 srtk-0.0.3/train_qald.ipynb
--rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 srtk-0.0.3/train_wd_simple.ipynb
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.3/.github/workflows/pytest.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/resources/wikimapper/index_enwiki.db -> /home/wiss/liao/shen/flamingo-gnn/data/kilt/index_enwiki-latest-uncased.db
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/__init__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/cli.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/link.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocess.py
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/retrieve.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/train.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/utils.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/visualize.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/__init__.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/dbpedia.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/freebase.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/wikidata.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/__init__.py
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/dbpedia.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/freebase.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/graph_base.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/wikidata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/load_dataset.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/merge_ground.py
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/negative_sampling.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/score_path.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/search_path.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/__init__.py
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/encoder.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/scorer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_dbpedia.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_encoder.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_freebase.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_link.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_scorer.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_wikidata.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/1.get_started.ipynb
--rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/2.end_to_end_subgraph_retrieval.ipynb
--rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/3.weak_train_wikidata.ipynb
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/4.weak_train_freebase.ipynb
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/5.supervised_train_wikidata.ipynb
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/6.extend_to_new_kg.ipynb
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 srtk-0.0.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.3/LICENSE
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 srtk-0.0.3/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 srtk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 srtk-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 srtk-0.0.4/bs.py
+-rw-r--r--   0        0        0    64070 2020-02-02 00:00:00.000000 srtk-0.0.4/coverage.svg
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 srtk-0.0.4/elegant_retrieve.py
+-rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 srtk-0.0.4/experiments.ipynb
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 srtk-0.0.4/filter.ipynb
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 srtk-0.0.4/linked.jsonl
+-rw-r--r--   0        0        0    75653 2020-02-02 00:00:00.000000 srtk-0.0.4/paper-graphs.ipynb
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 srtk-0.0.4/question.jsonl
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 srtk-0.0.4/readme.ipynb
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 srtk-0.0.4/subgraph.jsonl
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0     9781 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/cli.rst
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/getting_started.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/index.md
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/install.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/requirements.txt
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.knowledge_graph.rst
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.preprocessing.rst
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.scorer.rst
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/tutorials.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_freebase.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_qendpoint_rootless.md
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_wikidata.md
+-rw-r--r--   0        0        0    64488 2020-02-02 00:00:00.000000 srtk-0.0.4/examples/srtk_retrieve.svg
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-252130520118561472.html
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-4482246352718211871.html
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-5779087988204512933.html
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-7896195082647149010.html
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_164657081694304046.html
+-rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_2009481386569838770.html
+-rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_5967381679542830494.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/__init__.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/cli.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/link.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocess.py
+-rw-r--r--   0        0        0    15809 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/retrieve.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/train.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/utils.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/visualize.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/dbpedia.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/freebase.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/linker_base.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/wikidata.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/dbpedia.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/freebase.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/graph_base.py
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/wikidata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/load_dataset.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/merge_ground.py
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/negative_sampling.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/score_path.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/search_path.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/__init__.py
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/encoder.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/scorer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_dbpedia.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_encoder.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_freebase.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_link.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_scorer.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_wikidata.py
+-rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/2.end_to_end_subgraph_retrieval.ipynb
+-rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/3.weak_train_wikidata.ipynb
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/4.weak_train_freebase.ipynb
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/5.supervised_train_wikidata.ipynb
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/6.extend_to_new_kg.ipynb
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 srtk-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 srtk-0.0.4/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 srtk-0.0.4/PKG-INFO
```

### Comparing `srtk-0.0.3/train_wd_simple.ipynb` & `srtk-0.0.4/tutorials/5.supervised_train_wikidata.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928763440860215%*

 * *Differences: {"'cells'": "{3: {'execution_count': None}, 7: {'execution_count': None}, 9: {'execution_count': "*

 * *            "None}, 11: {'execution_count': None}, 20: {'execution_count': None}, 21: "*

 * *            "{'execution_count': None}, 22: {'source': {insert: [(0, '!CUDA_VISIBLE_DEVICES=1 srtk "*

 * *            "train -t $train_dataset_path \\\\\\n'), (1, '    -v $validation_dataset_path "*

 * *            "\\\\\\n'), (3, '    --output-dir $output_model_dir \\\\\\n'), (7, '    --max-epochs "*

 * *            "5')], delete: [7, 3, […]*

```diff
@@ -32,15 +32,15 @@
                 "```bash\n",
                 "pip install srsly srtk pandas\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "import pandas as pd\n",
                 "import srsly"
@@ -75,15 +75,15 @@
             "metadata": {},
             "source": [
                 "### 1.1 Inspect raw data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "raw_paths = {\n",
                 "    'train': 'data/wikidata-simplequestions/raw/annotated_wd_data_train_answerable.txt',\n",
                 "    'valid': 'data/wikidata-simplequestions/raw/annotated_wd_data_valid_answerable.txt',\n",
                 "    'test': 'data/wikidata-simplequestions/raw/annotated_wd_data_test_answerable.txt',\n",
@@ -101,15 +101,15 @@
             "metadata": {},
             "source": [
                 "`Rxxx` property identifiers encode the inverse property of the Wikidata property `Pxxx`. For example `R19` encodes the properties \"born here\", i.e. the inverse of `P19` (\"birth place\"). "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Q12439\tR19\tQ6106580\twho is a musician born in detroit\n",
@@ -131,15 +131,15 @@
             "metadata": {},
             "source": [
                 "### 1.2 Remove reverse relations"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Full train size: 19481\n",
@@ -231,43 +231,14 @@
                 "        samples.append(sample)\n",
                 "    save_path = os.path.join(intermediate_dir, f'scores_{split}.jsonl')\n",
                 "    srsly.write_jsonl(save_path, samples)\n",
                 "    print(f'Saved {split} scored paths file to {save_path}')"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Number of entities: 26688\n",
-                        "Number of relations: 75\n"
-                    ]
-                }
-            ],
-            "source": [
-                "entity_set = set()\n",
-                "relation_set = set()\n",
-                "for split in splits:\n",
-                "    data = preserved_data[split]\n",
-                "    samples = []\n",
-                "    for idx, line in enumerate(data.values):\n",
-                "        question_entity, relation, answer_entity, question = line\n",
-                "        entity_set.add(question_entity)\n",
-                "        entity_set.add(answer_entity)\n",
-                "        relation_set.add(relation)\n",
-                "print(f'Number of entities: {len(entity_set)}')\n",
-                "print(f'Number of relations: {len(relation_set)}')"
-            ]
-        },
-        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 2. Preprocessing\n",
                 "\n",
                 "Use the `srtk preprocess` command to creating training samples. Do not pass `--search-path` beacuse the paths are already provided in the dataset. This step mainly involves negative sampling and dataset generation."
@@ -349,25 +320,25 @@
                 "Training a retrieval model is as easy as running a single command! Just pass in the pretrained language model name and the training dataset path. We'll handle the rest.\n",
                 "\n",
                 "We recommend you to register an accound at [WanDB](https://docs.wandb.ai/quickstart), and log in in the command line. That's it, then you'll then be able to track your training progress in an online dashboard."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "train_dataset_path = os.path.join(dataset_dir, 'train.jsonl')\n",
                 "validation_dataset_path = os.path.join(dataset_dir, 'valid.jsonl')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "os.environ['TOKENIZERS_PARALLELISM'] = 'true'"
             ]
         },
         {
@@ -436,22 +407,22 @@
                         "\u001b[34m\u001b[1mwandb\u001b[0m: \ud83d\ude80 View run \u001b[33m04282334\u001b[0m at: \u001b[34m\u001b[4mhttps://wandb.ai/yuanchun/retrieval/runs/vtg7f3h7\u001b[0m\n",
                         "\u001b[34m\u001b[1mwandb\u001b[0m: Synced 6 W&B file(s), 0 media file(s), 0 artifact file(s) and 0 other file(s)\n",
                         "\u001b[34m\u001b[1mwandb\u001b[0m: Find logs at: \u001b[35m\u001b[1martifacts/wandb/run-20230428_233419-vtg7f3h7/logs\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
-                "!CUDA_VISIBLE_DEVICES=3 srtk train -t data/wikidata-simplequestions/dataset/train.jsonl \\\n",
-                "    -v data/wikidata-simplequestions/dataset/test.jsonl \\\n",
+                "!CUDA_VISIBLE_DEVICES=1 srtk train -t $train_dataset_path \\\n",
+                "    -v $validation_dataset_path \\\n",
                 "    --model-name-or-path roberta-base \\\n",
-                "    --output-dir artifacts/models/wd_simple_e10 \\\n",
+                "    --output-dir $output_model_dir \\\n",
                 "    --accelerator gpu \\\n",
                 "    --learning-rate 1e-5 \\\n",
                 "    --batch-size 96 \\\n",
-                "    --max-epochs 10"
+                "    --max-epochs 5"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -483,15 +454,15 @@
                 "    \"answer_entities\": [\"Q23513\"]\n",
                 "}\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "test_scored_path = os.path.join(intermediate_dir, 'scores_test.jsonl')"
             ]
         },
         {
```

### Comparing `srtk-0.0.3/.github/workflows/pytest.yml` & `srtk-0.0.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/link.py` & `srtk-0.0.4/src/srtk/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         folder_path.mkdir(parents=True)
         print(f"Folder {folder_path} created")
     Path(args.output).parent.mkdir(parents=True, exist_ok=True)
     srsly.write_jsonl(args.output, all_linked)
     print(f"Entity linking result saved to {args.output}")
 
 
-def add_arguments(parser):
+def _add_arguments(parser):
     """Add entity linking arguments to the parser"""
     parser.description = '''Entity linking on Wikidata.
     The input is a jsonl file. The field of interest is specified by the argument --ground-on.
     The output is a jsonl file, each line is a dict with keys: id, question_entities, spans, entity_names.
     '''
     parser.add_argument('-i', '--input', type=str, help='Input file path, in which the question is stored')
     parser.add_argument('-o', '--output', type=str, help='Output file path, in which the entity linking result is stored')
@@ -64,10 +64,10 @@
                         help='Knowledge graph to link to, only wikidata is supported now')
     parser.add_argument('--wikimapper-db', type=str, default='resources/wikimapper/index_enwiki.db', help='Wikimapper database path')
     parser.add_argument('--ground-on', type=str, default='question', help='The key to ground on, the corresponding text will be sent to the REL endpoint for entity linking')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    add_arguments(parser)
+    _add_arguments(parser)
     args = parser.parse_args()
     link(args)
```

### Comparing `srtk-0.0.3/src/srtk/preprocess.py` & `srtk-0.0.4/src/srtk/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """This script creates the training data from the grounded questions.
 
 Inputs should be a jsonl file, with each line representing a grounded question.
 The format of each line should be like this example:
-```json
-{
-  "id": "sample-id",
-  "question": "Which universities did Barack Obama graduate from?",
-  "question_entities": [
-    "Q76"
-  ],
-  "answer_entities": [
-    "Q49122",
-    "Q1346110",
-    "Q4569677"
-  ]
-}
-```
+
+.. code-block:: json
+
+    {
+        "id": "sample-id",
+        "question": "Which universities did Barack Obama graduate from?",
+        "question_entities": [
+            "Q76"
+        ],
+        "answer_entities": [
+            "Q49122",
+            "Q1346110",
+            "Q4569677"
+        ]
+    }
 """
+
 import os
 import argparse
 from argparse import Namespace
 from pathlib import Path
 
 from .preprocessing.search_path import main as search_path
 from .preprocessing.score_path import main as score_path
@@ -62,27 +64,27 @@
                                            scored_path_file=args.input,
                                            num_negative=args.num_negative,
                                            positive_threshold=args.positive_threshold,
                                            output_path=output_path,)
     negative_sampling(negative_sampling_args)
 
 
-def add_arguments(parser):
+def _add_arguments(parser):
     """Add preprocess arguments to a parser in place."""
     parser.description = 'Create the training data from the grounded questions.'
     parser.add_argument('-i', '--input', type=str, required=True,
                         help='The grounded questions file with question, question & answer entities')
     parser.add_argument('-o', '--output', type=str, required=True,
                         help='The output path where the final training data will be saved.')
     parser.add_argument('--intermediate-dir', type=str, help="The directory to save intermediate files. If not specified, the intermediate \
                         files will be saved in the same directory as the output file, with the name paths.jsonl and scores.jsonl")
     parser.add_argument('-e', '--sparql-endpoint', type=str, required=True,
                         help="SPARQL endpoint URL for either Wikidata or Freebase\
                         (e.g., 'http://localhost:1234/api/endpoint/sparql' for default local qEndpoint)")
-    parser.add_argument('-kg', '--knowledge-graph', type=str, required=True, choices=('wikidata', 'freebase'),
+    parser.add_argument('-kg', '--knowledge-graph', type=str, required=True, choices=('wikidata', 'freebase', 'dbpedia'),
                         help='knowledge graph name, either wikidata or freebase')
     parser.add_argument('--search-path', action='store_true',
                         help='Whether to search paths between question and answer entities. If not specified, paths and scores fields\
                         must present in the input file. You **have to** specify this for weakly supervised learning. (default: False)')
     parser.add_argument('--metric', choices=('jaccard', 'recall'), default='jaccard',
                         help='The metric used to score the paths. recall will usually result in a lager size of training dataset.\
                         (default: jaccard))')
@@ -91,10 +93,10 @@
     parser.add_argument('--positive-threshold', type=float, default=0.5,
                         help='The threshold to determine whether a path is positive or negative. If you want to use \
                         a larger training dataset, you can set this value to a smaller value. (default: 0.5)')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    add_arguments(parser)
+    _add_arguments(parser)
     args = parser.parse_args()
     preprocess(args)
```

### Comparing `srtk-0.0.3/src/srtk/retrieve.py` & `srtk-0.0.4/src/srtk/retrieve.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from collections import namedtuple
 from typing import List, Any, Dict
 
 import srsly
 import torch
 from tqdm import tqdm
 
-from .knowledge_graph import Freebase, Wikidata, KnowledgeGraphBase
+from .knowledge_graph import KnowledgeGraphBase
 from .scorer import Scorer
+from .utils import get_knowledge_graph
 
 
 END_REL = 'END OF HOP'
 
 
 # Path collects the information at each traversal step
 # - prev_relations stores the relations that have been traversed
@@ -260,48 +261,51 @@
 
 def print_and_save_recall(retrieved_path):
     """Calculate and print the recall of answer entities in retrieved triplets,
     If any answer from the answer entities is in the retrieved entities, the sample
     counts as a hit.
     """
     hit, miss = calculate_hit_and_miss(retrieved_path)
-    print(f"Answer recall: {hit / (hit + miss)} ({hit} / {hit + miss})")
+    print(f"Answer coverage rate: {hit / (hit + miss)} ({hit} / {hit + miss})")
     info = {}
     if hit + miss != 0:
         info = {
             'hit': hit,
             'miss': miss,
             'recall': hit / (hit + miss)
         }
     # path/to/subgraph.jsonl -> path/to/subgraph.metric
     recall_path = os.path.splitext(retrieved_path)[0] + '.metric'
     srsly.write_json(recall_path, info)
 
 
 def retrieve(args):
+    """Retrieve subgraphs from a knowledge graph.
+
+    Args:
+        args (Namespace): arguments for subgraph retrieval
+    """
     pathlib.Path(os.path.dirname(args.output)).mkdir(parents=True, exist_ok=True)
-    if args.knowledge_graph == 'freebase':
-        kg = Freebase(args.sparql_endpoint)
-    else:
-        kg = Wikidata(args.sparql_endpoint, exclude_qualifiers=not args.include_qualifiers)
+    kg = get_knowledge_graph(args.knowledge_graph, args.sparql_endpoint,
+                             exclude_qualifiers=not args.include_qualifiers)
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     scorer = Scorer(args.scorer_model_path, device)
     retriever = Retriever(kg, scorer, args.beam_width, args.max_depth)
     samples = list(srsly.read_jsonl(args.input))
     total = sum(1 for _ in srsly.read_jsonl(args.input))
     for sample in tqdm(samples, desc='Retrieving subgraphs', total=total):
         triplets = retriever.retrieve_subgraph_triplets(sample)
         sample['triplets'] = triplets
     srsly.write_jsonl(args.output, samples)
     print(f'Retrieved subgraphs saved to to {args.output}')
     if args.evaluate:
         print_and_save_recall(args.output)
 
 
-def add_arguments(parser):
+def _add_arguments(parser):
     """Add retrieve arguments to the parser in place."""
     parser.description = '''Retrieve subgraphs with a trained model on a dataset that entities are linked.
     This command can also be used to evaluate a trained retriever when the answer entities are known.
 
     Provide a JSON file as input, where each JSON object must contain at least the 'question' and 'question_entities' fields.
     When ``--evaluate`` is set, the input JSON file must also contain the 'answer_entities' field.
 
@@ -309,17 +313,17 @@
     with each triplet representing a (head, relation, tail) tuple.
     When ``--evaluate`` is set, a metric file will also be saved to the same directory as the output JSONL file.
     '''
     parser.add_argument('-i', '--input', type=str, required=True, help='path to input jsonl file. it should contain at least \
                         ``question`` and ``question_entities`` fields.')
     parser.add_argument('-o', '--output', type=str, required=True, help='output file path for storing retrieved triplets.')
     parser.add_argument('-e', '--sparql-endpoint', type=str, help='SPARQL endpoint for Wikidata or Freebase services.')
-    parser.add_argument('-kg', '--knowledge-graph', type=str, required=True, choices=('freebase', 'wikidata'),
+    parser.add_argument('-kg', '--knowledge-graph', type=str, required=True, choices=('freebase', 'wikidata', 'dbpedia'),
                         help='choose the knowledge graph: currently supports ``freebase`` and ``wikidata``.')
-    parser.add_argument('--scorer-model-path', type=str, required=True, help='Path to the scorer model, containing \
+    parser.add_argument('-m', '--scorer-model-path', type=str, required=True, help='Path to the scorer model, containing \
                         both the saved model and its tokenizer in the Huggingface models format.\
                         Such a model is saved automatically when using the ``srtk train`` command.\
                         Alternatively, provide a pre-trained model name from the Hugging Face model hub.\
                         In practice it supports any Huggingface transformers encoder model, though models that do not use [CLS] \
                         tokens may require modifications on similarity function.')
     parser.add_argument('--beam-width', type=int, default=10, help='beam width for beam search (default: 10).')
     parser.add_argument('--max-depth', type=int, default=2, help='maximum depth for beam search (default: 2).')
@@ -330,16 +334,18 @@
     parser.add_argument('--include-qualifiers', action='store_true', help='Include qualifiers from the retrieved triplets. \
                         Qualifiers are informations represented in non-entity form, like date, count etc.\
                         This is only relevant for Wikidata.')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    add_arguments(parser)
+    _add_arguments(parser)
     args = parser.parse_args()
     if not args.sparql_endpoint:
         if args.knowledge_graph == 'freebase':
             args.sparql_endpoint = 'http://localhost:3001/sparql'
-        else:
+        elif args.knowledge_graph == 'wikidata':
             args.sparql_endpoint = 'http://localhost:1234/api/endpoint/sparql'
+        else:
+            args.sparql_endpoint = 'https://dbpedia.org/sparql'
         print(f'Using default sparql endpoint for {args.knowledge_graph}: {args.sparql_endpoint}')
     retrieve(args)
```

### Comparing `srtk-0.0.3/src/srtk/train.py` & `srtk-0.0.4/src/srtk/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,15 +44,18 @@
                 batched[key].append(value)
         for key, value in batched.items():
             batched[key] = torch.stack(value, dim=0)
         return batched
 
 
 def prepare_dataloaders(train_data, validation_data, tokenizer, batch_size):
-    """Prepare dataloaders for training and validation."""
+    """Prepare dataloaders for training and validation.
+
+    If validation dataset is not provided, 5 percent of the training data will be used as validation data.
+    """
     def tokenize(example):
         tokenized = tokenizer(example['input_text'], padding='max_length', truncation=True, return_tensors='pt', max_length=32)
         return tokenized
 
     train_split = 'train[:95%]' if validation_data is None else 'train'
     validation_split = 'train[95%:]' if validation_data is None else 'train'
     if validation_data is None:
@@ -66,48 +69,58 @@
     validation_dataset = validation_dataset.map(tokenize, remove_columns=validation_dataset.column_names)
     train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True, collate_fn=Collator(tokenizer), num_workers=8)
     validation_loader = DataLoader(validation_dataset, batch_size=batch_size, shuffle=False, collate_fn=Collator(tokenizer), num_workers=8)
     return train_loader, validation_loader
 
 
 def train(args):
+    """Train the scorer model.
+
+    The model compares the similarity between [question; previous relation] and the next relation.
+    """
     torch.set_float32_matmul_precision('medium')
-    model = LitSentenceEncoder(args.model_name_or_path, lr=args.learning_rate)
+    model = LitSentenceEncoder(args.model_name_or_path, lr=args.learning_rate, loss=args.loss)
     tokenizer = AutoTokenizer.from_pretrained(args.model_name_or_path)
     train_loader, validation_loader = prepare_dataloaders(args.train_dataset, args.validation_dataset, tokenizer, args.batch_size)
     day_hour = datetime.datetime.now().strftime('%m%d%H%M')
-    wandb_logger = WandbLogger(project='retrieval', name=day_hour , group='contrastive', save_dir='artifacts')
+    wandb_logger = WandbLogger(project=args.wandb_project, name=day_hour , group=args.wandb_group, save_dir=args.wandb_savedir)
     trainer = pl.Trainer(accelerator=args.accelerator, default_root_dir=args.output_dir,
                          fast_dev_run=args.fast_dev_run, max_epochs=args.max_epochs, logger=wandb_logger)
     trainer.fit(model, train_dataloaders=train_loader, val_dataloaders=validation_loader)
     model.save_huggingface_model(args.output_dir)
     tokenizer.save_pretrained(args.output_dir)
 
 
-def add_arguments(parser):
+def _add_arguments(parser):
     """Add train arguments to a parser in place."""
     parser.add_argument('-t', '--train-dataset', required=True,
                         help='path to the training dataset. It should be a JSONL file with fields: query, positive, negatives')
     parser.add_argument('-v', '--validation-dataset',
                         help='path to the validation dataset. If not provided, 5 percent of the training data will be used as validation data.\
                         (default: None)')
     parser.add_argument('-o', '--output-dir', default='artifacts/scorer',
                         help='output model path. the model will be saved in the format of huggingface models,\
                         which can be uploaded to the huggingface hub and shared with the community.\
                         (default: artifacts/scorer)')
-    parser.add_argument('--model-name-or-path', default='intfloat/e5-small',
+    parser.add_argument('-m', '--model-name-or-path', default='intfloat/e5-small',
                         help='pretrained model name or path. It is fully compatible with HuggingFace models.\
                         You can specify either a local path where a model is saved, or an encoder model identifier\
                         from huggingface hub. (default: intfloat/e5-small)')
     parser.add_argument('-lr', '--learning-rate', default=5e-5, type=float, help='learning rate (default: 5e-5)')
     parser.add_argument('--batch-size', default=16, type=int, help='batch size (default: 16)')
+    parser.add_argument('--loss', default='cross_entropy', choices=['cross_entropy', 'contrastive'],
+                        help='loss function, can be cross_entropy or contrastive (default: cross_entropy)')
     parser.add_argument('--max-epochs', default=10, type=int, help='max epochs (default: 10)')
     parser.add_argument('--accelerator', default='gpu', help='accelerator, can be cpu, gpu, or tpu (default: gpu)')
     parser.add_argument('--fast-dev-run', action='store_true',
                         help='fast dev run for debugging, only use 1 batch for training and validation')
+    parser.add_argument('--wandb-project', default='retrieval', help='wandb project name (default: retrieval)')
+    parser.add_argument('--wandb-group', default='contrastive', help='wandb group name (default: contrastive)')
+    parser.add_argument('--wandb-savedir', default='artifacts', help='wandb save directory (default: artifacts)')
+
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    add_arguments(parser)
+    _add_arguments(parser)
     args = parser.parse_args()
 
     train(args)
```

### Comparing `srtk-0.0.3/src/srtk/visualize.py` & `srtk-0.0.4/src/srtk/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pathlib import Path
 
 import srsly
 from pyvis.network import Network
 from tqdm import tqdm
 from bs4 import BeautifulSoup as Soup
 
-from .knowledge_graph import KnowledgeGraphBase, Wikidata, Freebase
+from .knowledge_graph import KnowledgeGraphBase
+from .utils import get_knowledge_graph
 
 
 def visualize_subgraph(sample, kg: KnowledgeGraphBase):
     """Visualize the subgraph. It returns an html string.
     """
     net = Network(directed=True, font_color='#000000')
     net.barnes_hut()
@@ -66,18 +67,20 @@
     p_tag = soup.new_tag('p', attrs={'class': 'background-text'}, style="white-space:pre-wrap")
     p_tag.string = text
     soup.body.append(p_tag)
     return soup.prettify()
     
 
 def visualize(args):
-    if args.knowledge_graph == 'wikidata':
-        knowledge_graph = Wikidata(args.sparql_endpoint)
-    else:
-        knowledge_graph = Freebase(args.sparql_endpoint)
+    """Main entry for subgraph visualization.
+
+    Args:
+        args (Namespace): arguments for subgraph visualization.
+    """
+    knowledge_graph = get_knowledge_graph(args.knowledge_graph, args.sparql_endpoint)
     samples = srsly.read_jsonl(args.input)
     total = sum(1 for _ in srsly.read_jsonl(args.input))
     total = min(total, args.max_output)
     if not os.path.exists(args.output_dir):
         Path(args.output_dir).mkdir(parents=True, exist_ok=True)
         print(f'Created output directory: {args.output_dir}')
     for i, sample in enumerate(tqdm(samples, desc='Visualizing graphs', total=total)):
@@ -90,25 +93,25 @@
         html = add_text_to_html(html, text_to_append)
         output_path = os.path.join(args.output_dir, sample['id'] + '.html')
         with open(output_path, 'w', encoding='utf-8') as fout:
             fout.write(html)
     print(f'Visualized graphs outputted to {args.output_dir}.')
 
 
-def add_arguments(parser):
+def _add_arguments(parser):
     parser.description = 'Visualize the graph (represented as a set of triplets) using pyvis.'
     parser.add_argument('-i', '--input', required=True, help='The input subgraph file path.')
     parser.add_argument('-o', '--output-dir', required=True, help='The output directory path.')
     parser.add_argument('-e', '--sparql-endpoint', type=str, default='http://localhost:1234/api/endpoint/sparql',
                         help='SPARQL endpoint for Wikidata or Freebase services. In this step, it is used to get the labels of entities.\
                         (Default: http://localhost:1234/api/endpoint/sparql)')
-    parser.add_argument('-kg', '--knowledge-graph', type=str, choices=('wikidata', 'freebase'), default='wikidata',
+    parser.add_argument('-kg', '--knowledge-graph', type=str, choices=('wikidata', 'freebase', 'dbpedia'), default='wikidata',
                         help='The knowledge graph type to use. (Default: wikidata)')
     parser.add_argument('--max-output', type=int, default=1000,
                         help='The maximum number of graphs to output. This is useful for debugging. (Default: 1000)')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    add_arguments(parser)
+    _add_arguments(parser)
     args = parser.parse_args()
     visualize(args)
```

### Comparing `srtk-0.0.3/src/srtk/entity_linking/dbpedia.py` & `srtk-0.0.4/src/srtk/entity_linking/dbpedia.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Link entitiy mentions to DBpedia entities with the DBpedia Spotlight endpoint.
 
 Know more about DBpedia Spotlight at https://www.dbpedia-spotlight.org/.
 """
 import requests
 
+from .linker_base import LinkerBase
 
-class DBpediaLinker:
+class DBpediaLinker(LinkerBase):
     """Link entitiy mentions to DBpedia entities with the DBpedia Spotlight endpoint"""
     def __init__(self, endpoint):
         """Initialize the linker
         
         Args:
             endpoint (str): The endpoint of the DBpedia Spotlight service
                 e.g. https://api.dbpedia-spotlight.org/en/annotate
```

### Comparing `srtk-0.0.3/src/srtk/entity_linking/wikidata.py` & `srtk-0.0.4/src/srtk/entity_linking/wikidata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 
 from wikimapper import WikiMapper
 
+from .linker_base import LinkerBase
 
-class WikidataLinker:
+
+class WikidataLinker(LinkerBase):
     """Link entitiy mentions to Wikidata entities using the REL endpoint"""
     def __init__(self, endpoint, wikimapper_db):
         """Initialize the linker
 
         Args:
             endpoint (str): The endpoint of the REL service
             wikimapper_db (str): The path to the Wikimapper database
```

### Comparing `srtk-0.0.3/src/srtk/knowledge_graph/dbpedia.py` & `srtk-0.0.4/src/srtk/knowledge_graph/dbpedia.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,27 +91,64 @@
         if len(path) == 0:
             return [src]
         
         if len(path) == 1:
             query = f"""
                 SELECT DISTINCT ?dst WHERE {{
                     dbr:{src} dbo:{path[0]} ?dst.
+                    FILTER(STRSTARTS(str(?dst), "http://dbpedia.org/resource/"))
                 }}
-            """
+                LIMIT {limit}
+                """
         else:
             query = f"""
                 SELECT DISTINCT ?dst WHERE {{
                     dbr:{src} dbo:{path[0]} ?mid.
                     ?mid dbo:{path[1]} ?dst.
-                    }}
+                    FILTER(STRSTARTS(str(?dst), "http://dbpedia.org/resource/"))
+                }}
+                LIMIT {limit}
                 """
         leaves = self.queryDBPedia(query)
         leaves = [self.get_id_from_uri(leaf['dst']['value']) for leaf in leaves]
         return leaves
 
+    def deduce_leaves_from_multiple_srcs(self, srcs, path, limit=2000):
+        """Deuce leave entities from multiple source entities following the path.
+
+        Args:
+            srcs (list[str]): list of source entities
+            path (list[str]): path from source entity to destination entity
+            limit (int, optional): limit of the number of leaves. Defaults to 200.
+
+        Returns:
+            list[str]: list of leaves. Each leaf is a QID.
+        """
+        if len(path) >= 2:
+            raise NotImplementedError(f'Currenly only support paths with length less than 2, got {len(path)}')
+        if len(path) == 0:
+            return srcs
+        if len(srcs) == 0:
+            return []
+
+        query = f"""
+            SELECT DISTINCT ?x WHERE {{
+                VALUES ?src {{dbr:{' dbr:'.join(srcs)}}}
+                ?src dbo:{path[0]} ?x.
+                FILTER(STRSTARTS(str(?x), "http://dbpedia.org/resource/"))
+            }}
+            LIMIT {limit}
+            """
+        if self.prepend_prefixes:
+            query = self.PREFIXES + query
+        leaves = self.queryDBPedia(query)
+        # Keep only QIDs in the leaves
+        leaves = [leaf['x']['value'].split('/')[-1] for leaf in leaves]
+        return leaves
+
     @lru_cache
     def get_neighbor_relations(self, src, hop=1, limit=100):
         """Get all relations connected to an entity. The relations are
         limited to direct relations (those with wdt: prefix).
 
         Args:
             src (str): source entity
@@ -175,9 +212,7 @@
                 """
         labels = self.queryDBPedia(query)
         if len(labels) == 0:
             print(f'No label found for {identifier}')
             return None
         label = labels[0]['name']['value']
         return label
-
-
```

### Comparing `srtk-0.0.3/src/srtk/knowledge_graph/freebase.py` & `srtk-0.0.4/src/srtk/knowledge_graph/freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/knowledge_graph/graph_base.py` & `srtk-0.0.4/src/srtk/knowledge_graph/graph_base.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/knowledge_graph/wikidata.py` & `srtk-0.0.4/src/srtk/knowledge_graph/wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/preprocessing/load_dataset.py` & `srtk-0.0.4/src/srtk/preprocessing/load_dataset.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/preprocessing/merge_ground.py` & `srtk-0.0.4/src/srtk/preprocessing/merge_ground.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/src/srtk/preprocessing/negative_sampling.py` & `srtk-0.0.4/src/srtk/preprocessing/negative_sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from collections import defaultdict
 from functools import lru_cache
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import Wikidata, Freebase, KnowledgeGraphBase
+from knowledge_graph import KnowledgeGraphBase
+from utils import get_knowledge_graph
 
 END_REL = "END OF HOP"
 
 
 def sample_negative_relations(soruce_entities, prev_path, positive_connections,
                               num_negative, kg: KnowledgeGraphBase):
     """A helper function to sample negative relations.
@@ -49,15 +50,15 @@
     negative_relations = negative_relations - positive_connections[tuple(prev_path)]
     if len(negative_relations) == 0:
         return []
     negative_relations = random.choices(list(negative_relations), k=num_negative)
     return negative_relations
 
 
-def is_candidate_space_too_large(path, question_entities, kg, candidate_depth_multiplier=5):
+def is_candidate_space_too_large(path, question_entities, kg: KnowledgeGraphBase, candidate_depth_multiplier=5):
     """Check whether the number of the candidate entities along the path is too large.
     
     Args:
         path (list[str]): path from source entity to destination entity
         question_entities (list[str]): list of question entities
         kg (KnowledgeGraphBase): a knowledge graph instance
         candidate_depth_multiplier (int, optional): a multiplier to control the number of candidate entities
@@ -78,15 +79,15 @@
         if len(candidate_entities) > limit:
             flag_too_large = True
             break
     return flag_too_large
 
 
 def sample_records_from_path(path, question, question_entities, positive_connections,
-                             kg, num_negative):
+                             kg: KnowledgeGraphBase, num_negative):
     """Sample training records from a path.
     
     Returns:
         list[dict]: list of training records, each record has the following fields:
             - question (str): the question
             - prev_path (list): previous relations up to a relation (positive_relation) in the path
             - positive_relation (str): the next relation of the prev_path is regarded as the positive relation
@@ -175,18 +176,15 @@
             'negatives': record['negative_relations']
         }
         samples.append(sample)
     return samples
 
 
 def main(args):
-    if args.knowledge_graph == 'freebase':
-        kg = Freebase(args.sparql_endpoint)
-    else:
-        kg = Wikidata(args.sparql_endpoint)
+    kg = get_knowledge_graph(args.knowledge_graph, args.sparql_endpoint)
     positive_threshold = args.positive_threshold
     # Each sample has the following fields:
     # - id: sample id
     # - question: question text
     # - question_entities: list of question entities (ids)
     # - answer_entities: list of answer entities (ids)
     # - question: question text
@@ -219,16 +217,18 @@
     train_records = create_jsonl_dataset(train_records)
     srsly.write_jsonl(args.output_path, train_records)
     print(f"Training samples are saved to {args.output_path}")
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument('--sparql-endpoint', default='http://localhost:1234/api/endpoint/sparql', help='wikidata endpoint')
-    parser.add_argument('-kg', '--knowledge-graph', default='wikidata', help='knowledge graph name')
+    parser.add_argument('-e', '--sparql-endpoint', default='http://localhost:1234/api/endpoint/sparql',
+                        help='knowledge graph endpoint (default: http://localhost:1234/api/endpoint/sparql)')
+    parser.add_argument('-kg', '--knowledge-graph', default='wikidata', choices=['wikidata', 'freebase', 'dbpedia'],
+                        help='knowledge graph name')
     parser.add_argument('--scored-path-file', help='The file containing scored paths')
     parser.add_argument('--output-path', help='The path to the output file')
     parser.add_argument('--positive-threshold', type=float, default=0.5, help='The threshold to determine whether a path is positive or negative')
     parser.add_argument('--num-negative', type=int, default=15, help='The number of negative relations to sample for each positive relation')
     args = parser.parse_args()
 
     main(args)
```

### Comparing `srtk-0.0.3/src/srtk/preprocessing/score_path.py` & `srtk-0.0.4/src/srtk/preprocessing/score_path.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import sys
 import argparse
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import Wikidata, Freebase, KnowledgeGraphBase
+from knowledge_graph import KnowledgeGraphBase
+from utils import get_knowledge_graph
 
 
 def score_path(kg: KnowledgeGraphBase, src, path, answers, metric='jaccard'):
     """Calculate the HIT score of a given path.
     
     Args:
         kg (KnowledgeGraphBase): knowledge graph instance
@@ -49,18 +50,15 @@
         score = len(hit) / len(leaves)
     else: # metric == 'recall':
         score = len(hit) / len(answers)
     return score
 
 
 def main(args):
-    if args.knowledge_graph == 'freebase':
-        kg = Freebase(args.sparql_endpoint)
-    else:
-        kg = Wikidata(args.sparql_endpoint)
+    kg = get_knowledge_graph(args.knowledge_graph_type, args.sparql_endpoint)
     samples = srsly.read_jsonl(args.paths_file)
     total_lines = sum(1 for _ in srsly.read_jsonl(args.paths_file))
     processed_samples = []  # adds path_scores to each sample
     # Each sample is a dict with the following fields:
     # - id: sample id
     # - question: question text
     # - question_entities: list of question entities
@@ -82,15 +80,16 @@
         processed_samples.append(sample)
     srsly.write_jsonl(args.output_path, processed_samples)
     print(f'Scored paths saved to {args.output_path}')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
-    parser.add_argument('--sparql-endpoint', default='http://localhost:1234/api/endpoint/sparql', help='knowledge graph endpoint')
-    parser.add_argument('-kg', '--knowledge-graph', default='wikidata', help='knowledge graph name')
+    parser.add_argument('-e', '--sparql-endpoint', default='http://localhost:1234/api/endpoint/sparql', help='knowledge graph endpoint')
+    parser.add_argument('-kg', '--knowledge-graph', default='wikidata', choices=('wikidata', 'freebase', 'dbpedia'),
+                        help='knowledge graph name')
     parser.add_argument('--paths-file', help='the file where the paths are stored')
     parser.add_argument('--output-path', help='the file where the scores are stored')
     parser.add_argument('--metric', default='jaccard', choices=('jaccard', 'recall'), help='the metric used to score the paths')
     args = parser.parse_args()
 
     main(args)
```

### Comparing `srtk-0.0.3/src/srtk/preprocessing/search_path.py` & `srtk-0.0.4/src/srtk/preprocessing/search_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import os
 import argparse
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import Wikidata, Freebase, KnowledgeGraphBase
+from knowledge_graph import KnowledgeGraphBase
+from utils import get_knowledge_graph
 
 
 def generate_paths(src_entities, dst_entities, kg: KnowledgeGraphBase, max_path=50):
     """Generate paths from question entities to answer entities.
     """
     paths = []
     for src in src_entities:
@@ -47,18 +48,15 @@
     # Each ground sample has the following fields:
     # - id: sample id
     # - question: question text
     # - question_entities: list of question entities
     # - answer_entities: list of answer entities
     ground_samples = srsly.read_jsonl(args.ground_path)
     total_samples = sum(1 for _ in srsly.read_jsonl(args.ground_path))
-    if args.knowledge_graph == 'freebase':
-        kg = Freebase(args.sparql_endpoint)
-    else:
-        kg = Wikidata(args.sparql_endpoint)
+    kg = get_knowledge_graph(args.knowledge_graph, args.sparql_endpoint)
     processed_samples = []
     skipped = 0
     for sample in tqdm(ground_samples, total=total_samples, desc='Searching paths'):
         question_entities = sample['question_entities']
         answer_entities = sample['answer_entities']
         try:
             paths = generate_paths(question_entities, answer_entities, kg)
@@ -67,26 +65,25 @@
             print(e)
             continue
         if args.remove_sample_without_path and not paths:
             skipped += 1
             continue
         # Special filter for Freebase
         if args.knowledge_graph == 'freebase':
-            
             paths = list(filter(has_type_relation, paths))
         sample['paths'] = paths
         processed_samples.append(sample)
     print(f'Processed {len(processed_samples)} samples; skipped {skipped} samples without any paths between question entities and answer entities; total {total_samples} samples')
     srsly.write_jsonl(args.output_path, processed_samples)
     print(f'Retrieved paths saved to {args.output_path}')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('--sparql-endpoint', default='http://localhost:1234/api/endpoint/sparql', help='knowledge graph SPARQL endpoint')
-    parser.add_argument('--knowledge-graph', type=str, default='wikidata', choices=('wikidata', 'freebase'), help='knowledge graph name (default: wikidata)')
+    parser.add_argument('--knowledge-graph', type=str, default='wikidata', choices=('wikidata', 'freebase', 'dbpedia'), help='knowledge graph name (default: wikidata)')
     parser.add_argument('--ground-path', type=str, required=True, help='grounded file where the question and answer entities are stored')
     parser.add_argument('--output-path', type=str, required=True, help='path file where several paths for each sample stored')
     parser.add_argument('--remove-sample-without-path', action='store_true', help='remove samples without paths')
     args = parser.parse_args()
 
     main(args)
```

### Comparing `srtk-0.0.3/src/srtk/scorer/scorer.py` & `srtk-0.0.4/src/srtk/scorer/scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tests/test_dbpedia.py` & `srtk-0.0.4/tests/test_dbpedia.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,7 +44,13 @@
     relations = dbpedia.get_neighbor_relations(src, hop=1, limit=200)
     assert  all(r in relations for r in ["predecessor", "parent", "successor"]),\
         "'predecessor', 'parent', 'successor' should present in the relations"
 
     # Test 2-hop relations
     relations = dbpedia.get_neighbor_relations(src, hop=2)
     assert ("parent", "title") in relations, "Charles III --parent--> Elizabeth II --title--> Queen"
+
+def test_deduce_leaves_from_multiple_srcs(dbpedia):
+    srcs = ["Charles_III", "Elizabeth_II"]
+    path = ("successor",)
+    leaves = dbpedia.deduce_leaves_from_multiple_srcs(srcs, path, limit=10)
+    assert "Charles_III" in leaves and "William,_Prince_of_Wales" in leaves
```

### Comparing `srtk-0.0.3/tests/test_encoder.py` & `srtk-0.0.4/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tests/test_freebase.py` & `srtk-0.0.4/tests/test_freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tests/test_link.py` & `srtk-0.0.4/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tests/test_scorer.py` & `srtk-0.0.4/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tests/test_wikidata.py` & `srtk-0.0.4/tests/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tutorials/2.end_to_end_subgraph_retrieval.ipynb` & `srtk-0.0.4/tutorials/2.end_to_end_subgraph_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tutorials/3.weak_train_wikidata.ipynb` & `srtk-0.0.4/tutorials/3.weak_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/tutorials/4.weak_train_freebase.ipynb` & `srtk-0.0.4/tutorials/4.weak_train_freebase.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/.gitignore` & `srtk-0.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # data
 artifacts/
 data/
 htmls/
 .vscode/
 dist/
 
+# docs
+docs/_*
+
 # Temporarily ignored
 compare-score.ipynb
 el.py
 examine.ipynb
 mintaka.sh
 mkqa.sh
 ugly_retrieve.py
```

### Comparing `srtk-0.0.3/LICENSE` & `srtk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `srtk-0.0.3/pyproject.toml` & `srtk-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "srtk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Yuanchun Shen", email="y.c.shen@tum.de" },
 ]
 description = "A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `srtk-0.0.3/PKG-INFO` & `srtk-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,87 @@
-Metadata-Version: 2.1
-Name: srtk
-Version: 0.0.3
-Summary: A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs.
-Project-URL: Homepage, https://github.com/happen2me/subgraph-retrieval-toolkit
-Project-URL: Bug Tracker, https://github.com/happen2me/subgraph-retrieval-toolkit/issues
-Author-email: Yuanchun Shen <y.c.shen@tum.de>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Requires-Dist: beautifulsoup4
-Requires-Dist: datasets
-Requires-Dist: lightning
-Requires-Dist: pyvis
-Requires-Dist: sparqlwrapper
-Requires-Dist: srsly
-Requires-Dist: tqdm
-Requires-Dist: transformers
-Requires-Dist: wikimapper
-Description-Content-Type: text/markdown
-
-# Subgraph Retrieval Toolkit
+# SRTK: Subgraph Retrieval Toolkit
 
 [![PyPi](https://img.shields.io/pypi/v/srtk)](https://pypi.org/project/srtk/)
 [![Documentation Status](https://readthedocs.org/projects/srtk/badge/?version=latest)](https://srtk.readthedocs.io/en/latest/?badge=latest)
 [![PytestStatus](https://github.com/happen2me/subgraph-retrieval-wikidata/actions/workflows/pytest.yml/badge.svg)](https://github.com/happen2me/subgraph-retrieval-toolkit/actions/workflows/pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![DOI](https://zenodo.org/badge/622648166.svg)](https://zenodo.org/badge/latestdoi/622648166)
+
+
+**SRTK** is a toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs. It currently supports Wikidata, Freebase and DBPedia.
+
+A minimum walkthrough of the retrieve process:
 
-Retrieve subgraphs on Wikidata. The method is based on this [retrieval work](https://github.com/RUCKBReasoning/SubgraphRetrievalKBQA) for Freebase.
+![retrieve example](examples/srtk_retrieve.svg)
+
+<img width="400rem" src="https://i.imgur.com/jG7nZuo.png" alt="Visualized subgraph"/>
 
 ## Prerequisite
 
-### Install SRTK
+### Installations
+
 ```bash
 pip install srtk
 ```
 
-### Wikidata
-
-#### Deploy a Wikidata endpoint locally
-We use [qEndpoint](https://github.com/the-qa-company/qEndpoint) to spin up a Wikidata endpoint that
-contains a [Wikidata Truthy](https://www.wikidata.org/wiki/Wikidata:Database_download#RDF_dumps) dump.
+### Local Deployment of Knowledge Graphs
 
-- Download
+- [Setup Wikidata locally](https://srtk.readthedocs.io/en/latest/setup_wikidata.html)
+- [Setup Freebase locally](https://srtk.readthedocs.io/en/latest/setup_freebase.html)
 
-    ```bash
-    sudo docker run -p 1234:1234 --name qendpoint-wikidata qacompany/qendpoint-wikidata
-    ```
-
-- Run
-
-    ```bash
-    sudo docker start  qendpoint-wikidata
-    ```
-- Add Wikidata prefixes support
+## Usage
 
-    ```bash
-    wget https://raw.githubusercontent.com/the-qa-company/qEndpoint/master/wikibase/prefixes.sparql
-    sudo docker cp prefixes.sparql qendpoint-wikidata:/app/qendpoint && rm prefixes.sparql
-    ```
+There are mainly five subcommands of SRTK, which covers the whole pipeline of subgraph retrieval.
 
-Alternatively, you can also use an [online Wikidata endpoint](https://query.wikidata.org), e.g. `https://query.wikidata.org/sparql`
+For retrieval:
 
+- `srtk link`: Link entity mentions in texts to a knowledge graph. Currently Wikidata and DBPedia are supported out of the box.
+- `srtk retrieve`: Retrieve semantic-relevant subgraphs from a knowledge graph with a trained retriever. It can also be used to evaluate a trained retriever.
+- `srtk visualize`: Visualize retrieved subgraphs using a graph visualization tool.
 
-#### Deploy a REL endpoint for entity linking (only necessary for end-to-end inference)
+For training a retriever:
 
-Please refer to this tutorial for REL endpoint deployment: [End-to-End Entity Linking](https://rel.readthedocs.io/en/latest/tutorials/e2e_entity_linking/)
+- `srtk preprocess`: Preprocess a dataset for training a subgraph retrieval model.
+- `srtk train`: Train a subgraph retrieval model on a preprocessed dataset.
 
-### Freebase
 
-#### Deploy a Freebase endpoint locally
+Use `srtk [subcommand] --help` to see the detailed usage of each subcommand.
 
-Please refer to [dki-lab/Freebase-Setup](https://github.com/dki-lab/Freebase-Setup) for the setup.
+## Walkthrough
 
-```bash
-# Download setup script
-git clone https://github.com/dki-lab/Freebase-Setup.git && cd Freebase-Setup
-# Download virtuoso binary
-wget https://kumisystems.dl.sourceforge.net/project/virtuoso/virtuoso/7.2.5/virtuoso-opensource.x86_64-generic_glibc25-linux-gnu.tar.gz
-tar -zxvf virtuoso-opensource.x86_64-generic_glibc25-linux-gnu.tar.gz && rm virtuoso-opensource.x86_64-generic_glibc25-linux-gnu.tar.gz
-# Replace the virtuoso path in virtuoso.py
-sed -i 's/\/home\/dki_lab\/tools\/virtuoso\/virtuoso-opensource/\.\/virtuoso-opensource/g' virtuoso.py
-# Download Freebase dump
-wget https://www.dropbox.com/s/q38g0fwx1a3lz8q/virtuoso_db.zip
-unzip virtuoso_db.zip && rm virtuoso_db.zip
-# Start virtuoso
-python3 virtuoso.py start 3001 -d virtuoso_db
-```
+### Retrieve Subgraphs
 
+#### Retrieve subgraphs with a trained scorer
 
-## Retrieve subgraphs with a trained scorer
 ```bash
-srtk retrieve --sparql-endpoint WIKIDATA_ENDPOINT \
-    -kg wikidata
-    --scorer-model-path path/to/scorer \
-    --input data/ground.jsonl \
-    --output-path data/subgraph.jsonl \
-    --beam-width 10
+srtk retrieve [-h] -i INPUT -o OUTPUT [-e SPARQL_ENDPOINT] -kg {freebase,wikidata}
+              -m SCORER_MODEL_PATH [--beam-width BEAM_WIDTH] [--max-depth MAX_DEPTH]
+              [--evaluate] [--include-qualifiers]
 ```
 
 The `scorer-model-path` argument can be any huggingface pretrained encoder model. If it is a local
 path, please ensure the tokenizer is also saved along with the model.
 
-## Visualize retrieved subgraph
+#### Visualize retrieved subgraph
+
 ```bash
-srtk visualize --sparql-endpoint WIKIDATA_ENDPOINT \
-    --knowledge-graph wikidata \
-    --input data/subgraph.jsonl \
-    --output-dir ./htmls/
+srtk visualize [-h] -i INPUT -o OUTPUT_DIR [-e SPARQL_ENDPOINT]
+               [-kg {wikidata,freebase}] [--max-output MAX_OUTPUT]
 ```
 
-## Train a scorer
+### Train a Retriever
+
 A scorer is the model used to navigate the expanding path. At each expanding step, relations scored higher with scorer are picked as relations for the next hop.
 
 The score is based on the embedding similarity of the to-be-expanded relation with the query (question + previous expanding path).
 
 The model is trained in a distant supervised learning fashion. Given the question entities and the answer entities, the model uses the shortest paths along them as the supervision signal.
 
-### Preprocess a dataset
+#### Preprocess a dataset
+
 1. prepare training samples where question entities and answer entities are know.
 
     The training data should be saved in a jsonl file (e.g. `data/grounded.jsonl`). Each training sample should come with the following format:
     
     ```json
     {
       "id": "sample-id",
@@ -136,31 +95,41 @@
         "Q4569677"
       ]
     }
     ```
 2. Preprocess the samples with `srtk preprocess` command.
 
     ```bash
-    srtk preprocess --sparql-endpoint WIKIDATA_ENDPOINT \
-        -kg wikidata \
-        --input-file data/grounded.jsonl \
-        --output-dir data/retrieved --metric jaccard
+    srtk preprocess [-h] -i INPUT -o OUTPUT [--intermediate-dir INTERMEDIATE_DIR]
+                    -e SPARQL_ENDPOINT -kg {wikidata,freebase} [--search-path]
+                    [--metric {jaccard,recall}] [--num-negative NUM_NEGATIVE]
+                    [--positive-threshold POSITIVE_THRESHOLD]
     ```
 
     Under the hood, it does four things:
 
     1. Find the shortest paths between the question entities and the answer entities.
     2. Score the searched paths with Jaccard scores with the answers.
     3. Negative sampling. At each expanding step, the negative samples are those false relations connected to the tracked entities.
     4. Generate training dataset as a jsonl file.
 
-
-
-### Train a sentence encoder
+#### Train a sentence encoder
 
 The scorer should be initialized from a pretrained encoder model from huggingface hub. Here I used `intfloat/e5-small`, which is a checkpoint of the BERT model.
 
 ```bash
 srtk train --data-file data/train.jsonl \
     --model-name-or-path intfloat/e5-small \
     --save-model-path artifacts/scorer
 ```
+
+## Tutorials
+
+- [End-to-end Subgraph Retrieval](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/2.end_to_end_subgraph_retrieval.ipynb)
+- [Train a Retriever on Wikidata with Weak Supervision](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/3.weak_train_wikidata.ipynb)
+- [Train a Retriever on Freebase with Weak Supervision](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/4.weak_train_freebase.ipynb)
+- [Supervised Training with Wikidata Simple Questions](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/5.supervised_train_wikidata.ipynb)
+- [Extend SRTK to other Knowledge Graphs](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/6.extend_to_new_kg.ipynb)
+
+## License
+
+This project is licensed under the terms of the MIT license.
```

