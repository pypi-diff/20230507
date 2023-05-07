# Comparing `tmp/nlpforturkish-0.1.0.tar.gz` & `tmp/nlpforturkish-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpforturkish-0.1.0.tar", last modified: Sun Apr 30 13:53:49 2023, max compression
+gzip compressed data, was "nlpforturkish-0.1.1.tar", last modified: Sun May  7 10:26:10 2023, max compression
```

## Comparing `nlpforturkish-0.1.0.tar` & `nlpforturkish-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 13:53:49.773932 nlpforturkish-0.1.0/
--rw-rw-rw-   0        0        0      748 2023-04-30 13:53:49.773932 nlpforturkish-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 13:53:49.769932 nlpforturkish-0.1.0/nlpforturkish/
--rw-rw-rw-   0        0        0    22506 2023-04-22 12:21:14.000000 nlpforturkish-0.1.0/nlpforturkish/offensive_language_detect.py
--rw-rw-rw-   0        0        0     2637 2023-04-13 15:30:56.000000 nlpforturkish-0.1.0/nlpforturkish/twitterAPILib.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:53:49.772930 nlpforturkish-0.1.0/nlpforturkish.egg-info/
--rw-rw-rw-   0        0        0      748 2023-04-30 13:53:49.000000 nlpforturkish-0.1.0/nlpforturkish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-04-30 13:53:49.000000 nlpforturkish-0.1.0/nlpforturkish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 13:53:49.000000 nlpforturkish-0.1.0/nlpforturkish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-30 13:53:49.000000 nlpforturkish-0.1.0/nlpforturkish.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-30 13:53:49.000000 nlpforturkish-0.1.0/nlpforturkish.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 13:53:49.773932 nlpforturkish-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-04-30 13:51:42.000000 nlpforturkish-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:26:10.545804 nlpforturkish-0.1.1/
+-rw-rw-rw-   0        0        0      748 2023-05-07 10:26:10.543806 nlpforturkish-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 10:26:10.520468 nlpforturkish-0.1.1/nlpforturkish/
+-rw-rw-rw-   0        0        0    27110 2023-05-05 15:52:15.000000 nlpforturkish-0.1.1/nlpforturkish/offensive_language_detect.py
+-rw-rw-rw-   0        0        0     2637 2023-04-13 15:30:56.000000 nlpforturkish-0.1.1/nlpforturkish/twitterAPILib.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:26:10.540866 nlpforturkish-0.1.1/nlpforturkish.egg-info/
+-rw-rw-rw-   0        0        0      748 2023-05-07 10:26:10.000000 nlpforturkish-0.1.1/nlpforturkish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-07 10:26:10.000000 nlpforturkish-0.1.1/nlpforturkish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 10:26:10.000000 nlpforturkish-0.1.1/nlpforturkish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-07 10:26:10.000000 nlpforturkish-0.1.1/nlpforturkish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-07 10:26:10.000000 nlpforturkish-0.1.1/nlpforturkish.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 10:26:10.546305 nlpforturkish-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-05-07 10:09:53.000000 nlpforturkish-0.1.1/setup.py
```

### Comparing `nlpforturkish-0.1.0/PKG-INFO` & `nlpforturkish-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpforturkish
-Version: 0.1.0
+Version: 0.1.1
 Summary: The aim of the NLPforTurkish library is to assist people interested in artificial intelligence by supporting the Turkish NLP area, which will benefit many people, particularly those who want to work on Turkish NLP.
 Author: Furkan Kesgin
 Author-email: furkan_bfk@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nlpforturkish-0.1.0/nlpforturkish/offensive_language_detect.py` & `nlpforturkish-0.1.1/nlpforturkish/offensive_language_detect.py`

 * *Files 13% similar despite different names*

```diff
@@ -412,8 +412,132 @@
         if word2vec:
             X_train, X_test, y_train, y_test = self.get_word2vec(data_path, labels_path, vector_size=vector_size)
         else:
             X_train, X_test, y_train, y_test = self.get_encoded_data(data_path, labels_path, test_size=test_size, data_sep=data_sep)
         models,predictions = clf.fit(X_train, X_test, y_train, y_test)
         print(models)
         with open("NLPResult_new.txt", 'a+', encoding='utf-8') as f:
-            f.write(str(models)+"\n")
+            f.write(str(models)+"\n")
+
+
+
+    # def svm_accuracy(self,X, y, test_size, kernel='rbf'):
+    #     import numpy as np
+    #     from sklearn import svm
+    #     from sklearn.model_selection import train_test_split
+    #     from sklearn.metrics import accuracy_score
+
+    #     """
+    #     Trains an SVM classifier with the given kernel on the given data and returns
+    #     the accuracy of the classifier on the test set.
+
+    #     Parameters:
+    #         X (ndarray): The feature matrix of shape (n_samples, n_features).
+    #         y (ndarray): The target vector of shape (n_samples,).
+    #         test_size (float): The proportion of the data to be used for testing.
+    #         kernel (str): The type of kernel to be used in the SVM.
+
+    #     Returns:
+    #         float: The accuracy of the SVM classifier on the test set.
+    #     """
+    #     # Split the data into training and testing sets
+    #     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size)
+
+    #     # Train an SVM classifier with the given kernel
+    #     clf = svm.SVC(kernel=kernel)
+    #     clf.fit(X_train, y_train)
+
+    #     # Test the classifier and return the accuracy
+    #     y_pred = clf.predict(X_test)
+    #     accuracy = accuracy_score(y_test, y_pred)
+
+    #     return accuracy
+
+
+
+    def svm_accuracy(self, X, y, test_size, kernel_type):
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from matplotlib.colors import ListedColormap
+        from sklearn import svm
+        from sklearn.datasets import make_blobs
+        from sklearn.model_selection import train_test_split
+        # Split data into training and testing sets
+        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=0)
+
+        # Fit SVM model to the training data
+        clf = svm.SVC(kernel=kernel_type)
+        clf.fit(X_train, y_train)
+
+        # Calculate accuracy of the model on the testing data
+        accuracy = clf.score(X_test, y_test)
+
+        # Create a mesh to plot the decision boundary
+        h = 0.1  # step size in the mesh
+        x_min, x_max = X[:, 0].min() - 1, X[:, 0].max() + 1
+        y_min, y_max = X[:, 1].min() - 1, X[:, 1].max() + 1
+        xx, yy = np.meshgrid(np.arange(x_min, x_max, h),
+                            np.arange(y_min, y_max, h))
+
+        # Predict the decision function for each point on the grid
+        Z = clf.predict(np.c_[xx.ravel(), yy.ravel()])
+        Z = Z.reshape(xx.shape)
+
+        # Plot the decision boundary
+        cmap = ListedColormap(['#FFAAAA', '#AAAAFF'])
+        plt.contourf(xx, yy, Z, cmap=cmap, alpha=.8)
+
+        # Plot the data points
+        colors = ['r' if label == 0 else 'b' for label in y]
+        plt.scatter(X[:, 0], X[:, 1], color=colors, s=30)
+
+        plt.xlim(xx.min(), xx.max())
+        plt.ylim(yy.min(), yy.max())
+        plt.title("SVM Decision Boundary")
+        plt.show()
+
+        return accuracy
+
+
+    def train_lstm_model(self, model, x_path, y_path, epochs=10, batch_size=10):
+        import numpy as np
+        from tensorflow import keras
+        from sklearn.model_selection import train_test_split
+
+        # Load data
+        X = np.genfromtxt(x_path, delimiter=",")
+        y = np.genfromtxt(y_path, delimiter="\n")
+        X = X[:,None]
+        
+        # Train model
+        model.fit(X, y, epochs=epochs, batch_size=batch_size, verbose=1)
+        
+        # Evaluate model
+        loss, acc = model.evaluate(X, y, verbose=0)
+        
+        return model, loss, acc
+
+
+    def random_forest_classifier(self, X, y, test_size=0.2, n_estimators=100, max_depth=None):
+        from sklearn.model_selection import train_test_split
+        from sklearn.ensemble import RandomForestClassifier
+        from sklearn.metrics import accuracy_score
+
+        # Split the data into training and testing sets
+        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size)
+
+        # Create a random forest classifier
+        clf = RandomForestClassifier(n_estimators=n_estimators, max_depth=max_depth)
+
+        # Train the classifier on the training data
+        clf.fit(X_train, y_train)
+
+        # Make predictions on the test data
+        y_pred = clf.predict(X_test)
+
+        # Calculate the accuracy of the classifier on the test data
+        accuracy = accuracy_score(y_test, y_pred)
+
+        # Print the accuracy of the classifier on the test data
+        print("Accuracy:", accuracy)
+
+        return accuracy
```

### Comparing `nlpforturkish-0.1.0/nlpforturkish/twitterAPILib.py` & `nlpforturkish-0.1.1/nlpforturkish/twitterAPILib.py`

 * *Files identical despite different names*

### Comparing `nlpforturkish-0.1.0/nlpforturkish.egg-info/PKG-INFO` & `nlpforturkish-0.1.1/nlpforturkish.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpforturkish
-Version: 0.1.0
+Version: 0.1.1
 Summary: The aim of the NLPforTurkish library is to assist people interested in artificial intelligence by supporting the Turkish NLP area, which will benefit many people, particularly those who want to work on Turkish NLP.
 Author: Furkan Kesgin
 Author-email: furkan_bfk@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nlpforturkish-0.1.0/setup.py` & `nlpforturkish-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='nlpforturkish',
-    version='0.1.0',
+    version='0.1.1',
     description='The aim of the NLPforTurkish library is to assist people interested in artificial intelligence by supporting the Turkish NLP area, which will benefit many people, particularly those who want to work on Turkish NLP.',
     author='Furkan Kesgin',
     author_email='furkan_bfk@hotmail.com',
     packages=['nlpforturkish'],
     install_requires=[
         'pandas',
         'scikit-learn',
```

