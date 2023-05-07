# Comparing `tmp/vector-quantize-tf-0.0.1.tar.gz` & `tmp/vector-quantize-tf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector-quantize-tf-0.0.1.tar", last modified: Tue May  2 12:07:26 2023, max compression
+gzip compressed data, was "vector-quantize-tf-0.0.2.tar", last modified: Sun May  7 09:08:58 2023, max compression
```

## Comparing `vector-quantize-tf-0.0.1.tar` & `vector-quantize-tf-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:07:26.455843 vector-quantize-tf-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-02 11:44:23.000000 vector-quantize-tf-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      193 2023-05-02 12:07:26.455843 vector-quantize-tf-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-05-02 11:58:34.000000 vector-quantize-tf-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 12:07:26.456344 vector-quantize-tf-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      328 2023-05-02 11:51:40.000000 vector-quantize-tf-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:07:26.444843 vector-quantize-tf-0.0.1/vector_quantize_tf/
--rw-rw-rw-   0        0        0       60 2023-05-02 11:51:25.000000 vector-quantize-tf-0.0.1/vector_quantize_tf/__init__.py
--rw-rw-rw-   0        0        0     6975 2023-05-02 12:06:49.000000 vector-quantize-tf-0.0.1/vector_quantize_tf/vector_quantize_tf.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:07:26.455344 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/
--rw-rw-rw-   0        0        0      193 2023-05-02 12:07:26.000000 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-02 12:07:26.000000 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:07:26.000000 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-02 12:07:26.000000 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-02 12:07:26.000000 vector-quantize-tf-0.0.1/vector_quantize_tf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 09:08:58.630882 vector-quantize-tf-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-02 11:44:23.000000 vector-quantize-tf-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-05-07 09:08:58.630382 vector-quantize-tf-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-05-07 09:07:03.000000 vector-quantize-tf-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 09:08:58.630882 vector-quantize-tf-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      328 2023-05-07 09:05:17.000000 vector-quantize-tf-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:08:58.624883 vector-quantize-tf-0.0.2/vector_quantize_tf/
+-rw-rw-rw-   0        0        0       60 2023-05-02 11:51:25.000000 vector-quantize-tf-0.0.2/vector_quantize_tf/__init__.py
+-rw-rw-rw-   0        0        0     7238 2023-05-07 09:05:09.000000 vector-quantize-tf-0.0.2/vector_quantize_tf/vector_quantize_tf.py
+drwxrwxrwx   0        0        0        0 2023-05-07 09:08:58.628882 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-05-07 09:08:58.000000 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-07 09:08:58.000000 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 09:08:58.000000 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 09:08:58.000000 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-07 09:08:58.000000 vector-quantize-tf-0.0.2/vector_quantize_tf.egg-info/top_level.txt
```

### Comparing `vector-quantize-tf-0.0.1/LICENSE` & `vector-quantize-tf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector-quantize-tf-0.0.1/vector_quantize_tf/vector_quantize_tf.py` & `vector-quantize-tf-0.0.2/vector_quantize_tf/vector_quantize_tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,35 +50,38 @@
             trainable=False)
         
     def expire_codes(self, batch_samples):
         if self.threshold_ema_dead_code <= 0.0:
             return
         
         dead_codes = self.ema_cluster_size < self.threshold_ema_dead_code
+        indices_to_update = tf.where(dead_codes)
 
-        batch_samples = tf.reshape(batch_samples, (self.batch_size, -1, tf.shape(batch_samples)[-1]))
-        seq_len = tf.reduce_sum(tf.ones_like(batch_samples)[:, :, 0], axis=1)[0]
+        reshaped_samples = tf.reshape(batch_samples, (self.batch_size, -1, tf.shape(batch_samples)[-1]))
+        seq_len = tf.reduce_sum(tf.ones_like(reshaped_samples)[:, :, 0], axis=1)[0]
         seq_len = tf.cast(seq_len, tf.int32)
 
+        updated_embeddings = tf.transpose(self.embeddings)
         for i in range(self.batch_size):
-            samples = batch_samples[i]
+            samples = reshaped_samples[i]
             if seq_len >= self.codebook_size:
                 sampled_indices = tf.random.shuffle(tf.range(seq_len))[:self.codebook_size]
             else:
                 sampled_indices = tf.random.uniform((self.codebook_size,), minval=0, maxval=seq_len, dtype=tf.int32)
             sampled_vectors = tf.gather(samples, sampled_indices)
 
-            indices_to_update = tf.where(dead_codes)
             vectors_to_update = tf.gather(sampled_vectors, tf.range(tf.minimum(tf.shape(indices_to_update)[0], tf.shape(sampled_vectors)[0])))
-
-            # 更新
-            updated_embeddings = tf.transpose(self.embeddings)
             updated_embeddings = tf.tensor_scatter_nd_update(updated_embeddings, indices_to_update, vectors_to_update)
-            updated_embeddings = tf.transpose(updated_embeddings)
-            self.embeddings.assign(updated_embeddings)
+
+        updated_embeddings = tf.transpose(updated_embeddings)
+        self.embeddings.assign(updated_embeddings)
+
+        updated_ema_cluster_size = tf.where(dead_codes, tf.ones_like(self.ema_cluster_size) * self.threshold_ema_dead_code, self.ema_cluster_size)
+        self.ema_cluster_size.assign(updated_ema_cluster_size)
+        self.ema_w.assign(updated_embeddings * self.threshold_ema_dead_code)
 
     def call(self, inputs, training=False):
         flat_inputs = tf.reshape(inputs, [-1, self.embedding_dim])
 
         encoding_indices = self.get_code_indices(flat_inputs)
         encodings = tf.one_hot(encoding_indices, self.codebook_size)
         encoding_indices = tf.reshape(encoding_indices, tf.shape(inputs)[:-1])
```

