# Comparing `tmp/lincs-0.2.1.tar.gz` & `tmp/lincs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.2.1.tar", last modified: Fri May  5 14:06:38 2023, max compression
+gzip compressed data, was "lincs-0.2.2.tar", last modified: Sun May  7 07:36:57 2023, max compression
```

## Comparing `lincs-0.2.1.tar` & `lincs-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/
--rw-r--r--   0 user      (1002) user      (1002)       58 2023-05-04 08:59:02.000000 lincs-0.2.1/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    10602 2023-05-05 14:06:38.845341 lincs-0.2.1/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     9715 2023-05-05 13:53:52.000000 lincs-0.2.1/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      343 2023-05-05 13:09:35.000000 lincs-0.2.1/lincs/__init__.py
--rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.2.1/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    18889 2023-05-05 13:44:47.000000 lincs-0.2.1/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     9114 2023-05-05 13:34:11.000000 lincs-0.2.1/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    12319 2023-05-05 12:56:20.000000 lincs-0.2.1/lincs/liblincs/lincs.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     4460 2023-05-05 13:32:55.000000 lincs-0.2.1/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      718 2023-05-05 13:51:37.000000 lincs-0.2.1/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    10602 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      399 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/top_level.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.2.1/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-05 14:06:38.845341 lincs-0.2.1/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     1720 2023-05-05 14:06:10.000000 lincs-0.2.1/setup.py
+drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.263995 lincs-0.2.2/
+-rw-r--r--   0 user       (501) user      (1000)       58 2023-05-04 08:59:02.000000 lincs-0.2.2/MANIFEST.in
+-rw-r--r--   0 user       (501) user      (1000)    10602 2023-05-07 07:36:57.258234 lincs-0.2.2/PKG-INFO
+-rw-r--r--   0 user       (501) user      (1000)     9715 2023-05-07 07:29:05.000000 lincs-0.2.2/README.md
+drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.102837 lincs-0.2.2/lincs/
+-rw-r--r--   0 user       (501) user      (1000)      343 2023-05-05 13:09:35.000000 lincs-0.2.2/lincs/__init__.py
+-rw-r--r--   0 user       (501) user      (1000)      136 2023-05-04 08:59:02.000000 lincs-0.2.2/lincs/__main__.py
+-rw-r--r--   0 user       (501) user      (1000)    19010 2023-05-07 07:24:16.000000 lincs-0.2.2/lincs/command_line_interface.py
+drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.244083 lincs-0.2.2/lincs/liblincs/
+-rw-r--r--   0 user       (501) user      (1000)    10693 2023-05-07 07:22:28.000000 lincs-0.2.2/lincs/liblincs/liblincs_module.cpp
+-rw-r--r--   0 user       (501) user      (1000)    17260 2023-05-07 07:31:56.000000 lincs-0.2.2/lincs/liblincs/lincs.cpp
+-rw-r--r--   0 user       (501) user      (1000)     5040 2023-05-07 07:22:20.000000 lincs-0.2.2/lincs/liblincs/lincs.hpp
+-rw-r--r--   0 user       (501) user      (1000)      718 2023-05-05 13:51:37.000000 lincs-0.2.2/lincs/visualization.py
+drwxr-xr-x   0 user       (501) user      (1000)        0 2023-05-07 07:36:57.197053 lincs-0.2.2/lincs.egg-info/
+-rw-r--r--   0 user       (501) user      (1000)    10602 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) user      (1000)      399 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) user      (1000)        1 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) user      (1000)       60 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) user      (1000)       27 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/requires.txt
+-rw-r--r--   0 user       (501) user      (1000)       15 2023-05-07 07:36:56.000000 lincs-0.2.2/lincs.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) user      (1000)       27 2023-05-05 13:01:57.000000 lincs-0.2.2/requirements.txt
+-rw-r--r--   0 user       (501) user      (1000)       38 2023-05-07 07:36:57.266651 lincs-0.2.2/setup.cfg
+-rw-r--r--   0 user       (501) user      (1000)     1720 2023-05-07 07:34:57.000000 lincs-0.2.2/setup.py
```

### Comparing `lincs-0.2.1/PKG-INFO` & `lincs-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.2.1
+Version: 0.2.2
 Summary: MCDA algorithms
 Home-page: https://github.com/jacquev6/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -160,23 +160,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-model.yml model.yml
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.1/model.png
+    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.2/model.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp https://github.com/jacquev6/lincs/raw/v0.2.1/model.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.2/model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.2/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 10 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -200,23 +200,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-learning-set.csv learning-set.csv
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png
+    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.2.1/README.md` & `lincs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lincs-0.2.1/lincs/command_line_interface.py` & `lincs-0.2.2/lincs/command_line_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,39 +209,39 @@
         type=click.Choice(["mrsort"]),
         default="mrsort",
         show_default=True,
     ),
     {
         "mrsort": [
             (
-                "fixed-threshold",
+                "fixed-weights-sum",
                 dict(
-                    help="Use this pre-determined threshold instead of a pseudo-random one.",
-                    type=click.FloatRange(min=0.0, max=1.0),
+                    help="Make sure weights add up to this pre-determined value instead of a pseudo-random one.",
+                    type=click.FloatRange(min=1.0),
                     default=None,
                     show_default=True,
                 ),
                 {},
             ),
         ],
     },
 )
 def classification_model(
     domain,
     output_model,
     random_seed,
     model_type,
-    mrsort__fixed_threshold,
+    mrsort__fixed_weights_sum,
 ):
     domain = lincs.load_domain(domain)
     assert model_type == "mrsort"
     model = lincs.generate_mrsort_model(
         domain,
-        # fixed_threshold=mrsort__fixed_threshold,
         random_seed=random_seed,
+        fixed_weights_sum=mrsort__fixed_weights_sum,
     )
     model.dump(output_model)
 
 
 @generate.command(
     help="""
         Generate synthetic classified alternatives.
@@ -266,41 +266,40 @@
     "--output-classified-alternatives",
     type=click.File(mode="w"),
     default="-",
     help="Write generated classified alternatives to this file instead of standard output.",
 )
 @click.option(
     "--max-imbalance",
-    help="@todo Define.",
-    type=click.FloatRange(min=0.0, max=1.0),
+    type=click.FloatRange(min=0.0, max=1.0, max_open=True),
     default=None,
-    show_default=True,
+    help="Ensure that categories are balanced, by forcing their size to differ from the perfectly balanced size by at most this fraction.",
 )
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
     default=random.randrange(2**30),
 )
 def classified_alternatives(
     domain,
     model,
     alternatives_count,
-    max_imbalance,
     output_classified_alternatives,
+    max_imbalance,
     random_seed,
 ):
     domain = lincs.load_domain(domain)
     model = lincs.load_model(domain, model)
     alternatives = lincs.generate_alternatives(
         domain,
         model,
         alternatives_count,
-        # max_imbalance=max_imbalance,
         random_seed=random_seed,
+        max_imbalance=max_imbalance,
     )
     alternatives.dump(output_classified_alternatives)
 
 
 @main.group()
 def visualize():
     pass
```

### Comparing `lincs-0.2.1/lincs/liblincs/liblincs_module.cpp` & `lincs-0.2.2/lincs/liblincs/liblincs_module.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 }
 
 lincs::Alternatives load_alternatives(const lincs::Domain& domain, bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
   return lincs::Alternatives::load(domain, in_stream);
 }
 
+// @todo Thoroughly review all conversions between Python and C++ types.
+// - read Boost.Python doc in details and understand the contract
+// - homogenize converters (some were copy-pasted from SO answers and even ChatGPT)
+// - double-check if/when we need to increment reference counts on Python objects
 // https://stackoverflow.com/a/15940413/905845
 struct iterable_converter {
   template <typename Container>
   iterable_converter& from_python() {
     bp::converter::registry::push_back(
       &iterable_converter::convertible,
       &iterable_converter::construct<Container>,
@@ -101,14 +105,50 @@
     typedef bp::stl_input_iterator<typename Container::value_type> iterator;
 
     new (storage) Container(iterator(bp::object(handle)), iterator());
     data->convertible = storage;
   }
 };
 
+template<typename T>
+struct std_optional_converter {
+  static PyObject* convert(const std::optional<T>& value) {
+    if (value) {
+      return bp::incref(bp::object(*value).ptr());
+    } else {
+      return bp::incref(bp::object().ptr());
+    }
+  }
+
+  static void* convertible(PyObject* obj) {
+    if (obj == Py_None) {
+      return new std::optional<T>();
+    } else if (PyNumber_Check(obj)) {
+      return new std::optional<T>(bp::extract<T>(obj));
+    } else {
+      return nullptr;
+    }
+  }
+
+  static void construct(PyObject* obj, bp::converter::rvalue_from_python_stage1_data* data) {
+    void* storage = reinterpret_cast<bp::converter::rvalue_from_python_storage<std::optional<T>>*>(data)->storage.bytes;
+    new (storage) std::optional<T>(*reinterpret_cast<std::optional<T>*>(convertible(obj)));
+    data->convertible = storage;
+  }
+
+  static void enroll() {
+    bp::to_python_converter<std::optional<T>, std_optional_converter<T>>();
+    bp::converter::registry::push_back(
+      &std_optional_converter<T>::convertible,
+      &std_optional_converter<T>::construct,
+      bp::type_id<std::optional<T>>()
+    );
+  }
+};
+
 }  // namespace
 
 template <typename T>
 void auto_enum(const std::string& name) {
   auto e = bp::enum_<T>(name.c_str());
   for(T value : magic_enum::enum_values<T>()) {
     e.value(std::string(magic_enum::enum_name(value)).c_str(), value);
@@ -121,14 +161,16 @@
     .from_python<std::vector<lincs::Domain::Category>>()
     .from_python<std::vector<lincs::Domain::Criterion>>()
     .from_python<std::vector<lincs::Model::Boundary>>()
     .from_python<std::vector<lincs::Model::SufficientCoalitions>>()
     .from_python<std::vector<lincs::Alternative>>()
   ;
 
+  std_optional_converter<float>::enroll();
+
   // @todo Decide wether we nest types or not, use the same nesting in Python and C++
   auto_enum<lincs::Domain::Criterion::ValueType>("ValueType");
   auto_enum<lincs::Domain::Criterion::CategoryCorrelation>("CategoryCorrelation");
   auto_enum<lincs::Model::SufficientCoalitions::Kind>("SufficientCoalitionsKind");
 
   bp::class_<lincs::Domain::Criterion>("Criterion", bp::init<std::string, lincs::Domain::Criterion::ValueType, lincs::Domain::Criterion::CategoryCorrelation>())
     .def_readwrite("name", &lincs::Domain::Criterion::name)
@@ -199,15 +241,15 @@
     &load_model,
     (bp::arg("domain"), "in"),
     "Load a model for the provided `domain`, from the provided `.read()`-supporting file-like object, in YAML format."
   );
   bp::def(
     "generate_mrsort_model",
     &lincs::Model::generate_mrsort,
-    (bp::arg("domain"), "random_seed"),
+    (bp::arg("domain"), "random_seed", bp::arg("fixed_weights_sum")=std::optional<float>()),
     "Generate an MR-Sort model for the provided `domain`."
   );
 
   bp::class_<lincs::Alternative>("Alternative", bp::init<std::string, std::vector<float>, std::string>())
     .def_readwrite("name", &lincs::Alternative::name)
     .def_readwrite("profile", &lincs::Alternative::profile)
     .def_readwrite("category", &lincs::Alternative::category)
@@ -229,15 +271,15 @@
     &load_alternatives,
     (bp::arg("domain"), "in"),
     "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
   );
   bp::def(
     "generate_alternatives",
     &lincs::Alternatives::generate,
-    (bp::arg("domain"), "model", "alternatives_count", "random_seed"),
+    (bp::arg("domain"), "model", "alternatives_count", "random_seed", bp::arg("max_imbalance")=std::optional<float>()),
     "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `domain`, classified according to the provided `model`."
   );
 
   bp::class_<lincs::ClassificationResult>("ClassificationResult", bp::no_init)
     .def_readonly("changed", &lincs::ClassificationResult::changed)
     .def_readonly("unchanged", &lincs::ClassificationResult::unchanged)
   ;
```

### Comparing `lincs-0.2.1/lincs/liblincs/lincs.cpp` & `lincs-0.2.2/lincs/liblincs/lincs.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
   assert(node["kind"].as<std::string>() == "classification-model");
   assert(node["format_version"].as<int>() == 1);
 
   return Model(domain, node["boundaries"].as<std::vector<Boundary>>());
 }
 
-Model Model::generate_mrsort(const Domain& domain, const unsigned random_seed) {
+Model Model::generate_mrsort(const Domain& domain, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
   const unsigned categories_count = domain.categories.size();
   const unsigned criteria_count = domain.criteria.size();
 
   std::mt19937 gen(random_seed);
 
   // Profile can take any values. We arbitrarily generate them uniformly
   std::uniform_real_distribution<float> values_distribution(0.01f, 0.99f);
@@ -192,22 +192,22 @@
   // ... and use consecutive differences as (normalized) weights
   std::vector<float> normalized_weights(criteria_count);
   std::transform(
     partial_sums.begin(), std::prev(partial_sums.end()),
     std::next(partial_sums.begin()),
     normalized_weights.begin(),
     [](float left, float right) { return right - left; });
-  // We then generate an arbitrary threshold.
-  const float threshold = std::uniform_real_distribution<float>(0.0f, 1.f)(gen);
-  // Finally, we denormalize weights
+  // Finally, we denormalize weights so that they add up to a pseudo-random value not less than 1
+  assert(!fixed_weights_sum || *fixed_weights_sum >= 1);
+  const float weights_sum = fixed_weights_sum ? *fixed_weights_sum : 1.f / std::uniform_real_distribution<float>(0.f, 1.f)(gen);
   std::vector<float> denormalized_weights(criteria_count);
   std::transform(
     normalized_weights.begin(), normalized_weights.end(),
     denormalized_weights.begin(),
-    [threshold](float w) { return w / threshold; });
+    [weights_sum](float w) { return w * weights_sum; });
 
   SufficientCoalitions coalitions{
     SufficientCoalitions::Kind::weights,
     denormalized_weights,
   };
 
   std::vector<Boundary> boundaries;
@@ -270,17 +270,21 @@
     }
     alternatives.push_back(alternative);
   }
 
   return Alternatives{domain, alternatives};
 }
 
-Alternatives Alternatives::generate(const Domain& domain, const Model& model, const unsigned alternatives_count, const unsigned random_seed) {
+Alternatives generate_uniform_alternatives(
+  const Domain& domain,
+  const Model& model,
+  const unsigned alternatives_count,
+  std::mt19937& gen
+) {
   const unsigned criteria_count = domain.criteria.size();
-  std::mt19937 gen(random_seed);
 
   std::vector<Alternative> alternatives;
   alternatives.reserve(alternatives_count);
 
   // We don't do anything to ensure homogeneous repartition amongst categories.
   // We just generate random profiles uniformly in [0, 1]
   std::uniform_real_distribution<float> values_distribution(0.0f, 1.0f);
@@ -300,14 +304,144 @@
 
   Alternatives alts{domain, alternatives};
   classify_alternatives(domain, model, &alts);
 
   return alts;
 }
 
+unsigned min_category_size(const unsigned alternatives_count, const unsigned categories_count, const float max_imbalance) {
+  assert(max_imbalance >= 0);
+  assert(max_imbalance <= 1);
+
+  return std::floor(alternatives_count * (1 - max_imbalance) / categories_count);
+}
+
+unsigned max_category_size(const unsigned alternatives_count, const unsigned categories_count, const float max_imbalance) {
+  assert(max_imbalance >= 0);
+  assert(max_imbalance <= 1);
+
+  return std::ceil(alternatives_count * (1 + max_imbalance) / categories_count);
+}
+
+Alternatives generate_balanced_alternatives(
+  const Domain& domain,
+  const Model& model,
+  const unsigned alternatives_count,
+  const float max_imbalance,
+  std::mt19937& gen
+) {
+  assert(max_imbalance >= 0);
+  assert(max_imbalance <= 1);
+
+  const unsigned categories_count = domain.categories.size();
+
+  // These parameters are somewhat arbitrary and not really critical,
+  // but changing there values *does* change the generated set, because of the two-steps process below:
+  // the same alternatives are generated in the same order, but they treated differently here.
+
+  // How long to insist before accepting failure when we can't find any alternative for a given category
+  const int max_iterations_with_no_effect_with_empty_category = 100;
+
+  // How long to insist before accepting failure when we have found at least one alternative for each category
+  const int max_iterations_with_no_effect_with_all_categories_populated = 1'000;
+
+  // Size ratio to call 'uniform_learning_set'. Small values imply calling it more, and large values
+  // imply discarding more alternatives
+  const int multiplier = 10;
+
+  const unsigned min_size = min_category_size(alternatives_count, categories_count, max_imbalance);
+  const unsigned max_size = max_category_size(alternatives_count, categories_count, max_imbalance);
+
+  std::vector<Alternative> alternatives;
+  alternatives.reserve(alternatives_count);
+  std::map<std::string, unsigned> histogram;
+  for (const auto& category : domain.categories) {
+    histogram[category.name] = 0;
+  }
+
+  int max_iterations_with_no_effect = max_iterations_with_no_effect_with_empty_category;
+
+  // Step 1: fill all categories to exactly the min size
+  // (skip if min size is zero)
+  int iterations_with_no_effect = 0;
+  while (min_size > 0) {
+    ++iterations_with_no_effect;
+
+    Alternatives candidates = generate_uniform_alternatives(domain, model, multiplier * alternatives_count, gen);
+
+    for (const auto& candidate : candidates.alternatives) {
+      assert(candidate.category);
+      const std::string& category = *candidate.category;
+      if (histogram[category] < min_size) {
+        alternatives.push_back(candidate);
+        ++histogram[category];
+        iterations_with_no_effect = 0;
+      }
+    }
+
+    if (std::all_of(histogram.begin(), histogram.end(), [min_size](const auto it) { return it.second >= min_size; })) {
+      // Success
+      break;
+    }
+
+    if (std::all_of(histogram.begin(), histogram.end(), [](const auto it) { return it.second > 0; })) {
+      max_iterations_with_no_effect = max_iterations_with_no_effect_with_all_categories_populated;
+    }
+
+    if (iterations_with_no_effect > max_iterations_with_no_effect) {
+      throw BalancedAlternativesGenerationException(histogram);
+    }
+  }
+
+  // Step 2: reach target size, keeping all categories below or at the max size
+  iterations_with_no_effect = 0;
+  while (true) {
+    ++iterations_with_no_effect;
+
+    Alternatives candidates = generate_uniform_alternatives(domain, model, multiplier * alternatives_count, gen);
+
+    for (const auto& candidate : candidates.alternatives) {
+      assert(candidate.category);
+      const std::string& category = *candidate.category;
+      if (histogram[category] < max_size) {
+        alternatives.push_back(candidate);
+        ++histogram[category];
+        iterations_with_no_effect = 0;
+      }
+
+      if (alternatives.size() == alternatives_count) {
+        assert(std::all_of(
+          histogram.begin(), histogram.end(),
+          [min_size, max_size](const auto it) { return it.second >= min_size && it.second <= max_size; }));
+        return Alternatives(domain, alternatives);
+      }
+    }
+
+    if (iterations_with_no_effect > max_iterations_with_no_effect) {
+      throw BalancedAlternativesGenerationException(histogram);
+    }
+  }
+}
+
+Alternatives Alternatives::generate(
+  const Domain& domain,
+  const Model& model,
+  const unsigned alternatives_count,
+  const unsigned random_seed,
+  const std::optional<float> max_imbalance
+) {
+  std::mt19937 gen(random_seed);
+
+  if (max_imbalance) {
+    return generate_balanced_alternatives(domain, model, alternatives_count, *max_imbalance, gen);
+  } else {
+    return generate_uniform_alternatives(domain, model, alternatives_count, gen);
+  }
+}
+
 ClassificationResult classify_alternatives(const Domain& domain, const Model& model, Alternatives* alternatives) {
   assert(&model.domain == &domain);
   assert(&alternatives.domain == &domain);
 
   const unsigned criteria_count = domain.criteria.size();
   const unsigned categories_count = domain.categories.size();
```

### Comparing `lincs-0.2.1/lincs/liblincs/lincs.hpp` & `lincs-0.2.2/lincs/liblincs/lincs.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#include <map>
 #include <optional>
 #include <ostream>
 #include <string>
 #include <vector>
 
 
 namespace lincs {
@@ -89,38 +90,55 @@
   std::vector<Boundary> boundaries;  // boundary_index 0 is between category_index 0 and category_index 1
 
   Model(const Domain& domain_, const std::vector<Boundary>& boundaries_) : domain(domain_), boundaries(boundaries_) {}
 
   void dump(std::ostream&) const;
   static Model load(const Domain&, std::istream&);
 
-  static Model generate_mrsort(const Domain&, unsigned random_seed);
+  static Model generate_mrsort(const Domain&, unsigned random_seed, std::optional<float> fixed_weights_sum = std::nullopt);
 };
 
 struct Alternative {
   std::string name;
   std::vector<float> profile;
   std::optional<std::string> category;
 
   Alternative() {}
   Alternative(const std::string& name_, const std::vector<float>& profile_, const std::optional<std::string>& category_): name(name_), profile(profile_), category(category_) {}
 
   bool operator==(const Alternative& other) const { return name == other.name && profile == other.profile && category == other.category; }
 };
 
+class BalancedAlternativesGenerationException : public std::exception {
+ public:
+  explicit BalancedAlternativesGenerationException(const std::map<std::string, unsigned>& histogram_) : histogram(histogram_) {}
+
+  const char* what() const noexcept override {
+    return "Unable to generate balanced alternatives. Try increasing the allowed imbalance, or use a more lenient model?";
+  }
+
+  std::map<std::string, unsigned> histogram;
+};
+
 struct Alternatives {
   const Domain& domain;
   std::vector<Alternative> alternatives;
 
   Alternatives(const Domain& domain_, const std::vector<Alternative>& alternatives_): domain(domain_), alternatives(alternatives_) {}
 
   void dump(std::ostream&) const;
   static Alternatives load(const Domain&, std::istream&);
 
-  static Alternatives generate(const Domain&, const Model&, unsigned alternatives_count, unsigned random_seed);
+  static Alternatives generate(
+    const Domain&,
+    const Model&,
+    unsigned alternatives_count,
+    unsigned random_seed,
+    std::optional<float> max_imbalance = std::nullopt
+  );
 };
 
 struct ClassificationResult {
   unsigned unchanged;
   unsigned changed;
 };
```

### Comparing `lincs-0.2.1/lincs/visualization.py` & `lincs-0.2.2/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.2.1/lincs.egg-info/PKG-INFO` & `lincs-0.2.2/lincs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.2.1
+Version: 0.2.2
 Summary: MCDA algorithms
 Home-page: https://github.com/jacquev6/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -160,23 +160,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-model.yml model.yml
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.1/model.png
+    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.2/model.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp https://github.com/jacquev6/lincs/raw/v0.2.1/model.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.2/model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.2/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 10 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -200,23 +200,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-learning-set.csv learning-set.csv
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png
+    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.2/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.2.1/setup.py` & `lincs-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-version = "0.2.1"
+version = "0.2.2"
 
 with open("README.md") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
     long_description = long_description.replace(f"{image}.png", f"https://github.com/jacquev6/lincs/raw/v{version}/{image}.png")
 
 with open("requirements.txt") as f:
```

