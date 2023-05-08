# Comparing `tmp/MLandPattern-0.1.9.tar.gz` & `tmp/MLandPattern-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.1.9.tar", last modified: Wed May  3 19:29:09 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.0.tar", last modified: Mon May  8 07:11:29 2023, max compression
```

## Comparing `MLandPattern-0.1.9.tar` & `MLandPattern-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.635215 MLandPattern-0.1.9/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.629397 MLandPattern-0.1.9/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    16780 2023-04-28 06:57:12.000000 MLandPattern-0.1.9/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.9/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.633597 MLandPattern-0.1.9/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-03 19:29:09.634724 MLandPattern-0.1.9/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.9/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-05-03 19:29:09.635567 MLandPattern-0.1.9/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-05-03 19:27:46.000000 MLandPattern-0.1.9/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.403112 MLandPattern-0.2.0/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.396637 MLandPattern-0.2.0/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    21860 2023-05-08 07:10:03.000000 MLandPattern-0.2.0/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.0/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-08 07:11:29.400802 MLandPattern-0.2.0/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-05-08 07:11:29.000000 MLandPattern-0.2.0/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-08 07:11:29.402303 MLandPattern-0.2.0/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.0/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-05-08 07:11:29.403473 MLandPattern-0.2.0/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-05-08 07:10:11.000000 MLandPattern-0.2.0/setup.py
```

### Comparing `MLandPattern-0.1.9/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.0/MLandPattern/MLandPattern.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,31 @@
     # Re-assign the values of the class names to numeric values
     label_list = []
     for lab in df.loc[:, len(attribute_names)]:
         label_list.append(class_label.index(lab))
     label = np.array(label_list)
     return attribute, label
 
+def load(pathname, vizualization=0):
+    """
+    Loads simple csv, assuming first n-1 columns as attributes, and n col as class labels
+    :param pathname: path to the data file
+    :param vizualization: flag to determine if print on console dataframe head (default false)
+    :return: attributes, labels. attrributes contains a numpy matrix with the attributes of the dataset. labels contains a numpy matrix
+            with the class labels as numbers, ranging from [0, n]
+    """
+    df = pd.read_csv(pathname, header=None)
+    if vizualization:
+        print(df.head())
+    attribute = np.array(df.iloc[:, 0 : len(df.columns) - 1])
+    attribute = attribute.T
+    # print(attribute)
+    label = np.array(df.iloc[:, -1])
+
+    return attribute, label
 
 def vcol(vector):
     """
     Reshape a vector row vector into a column vector
     :param vector: a numpy row vector
     :return: the vector reshaped as a column vector
     """
@@ -105,21 +122,21 @@
 
 
 def PCA(attribute_matrix, m):
     """
     Calculates the PCA dimension reduction of a matrix to a m-dimension sub-space
     :param attribute_matrix: matrix with the datapoints, with each row being a point
     :param m: number of dimensions of the targeted sub-space
-    :return: a projection matrix P
+    :return: The dataset after the dimensionality reduction
     """
     DC = center_data(attribute_matrix)
     C = covariance(DC, 1)
     s, U = eigen(C)
     P = U[:, ::-1][:, 0:m]
-    return P
+    return np.dot(P.T, attribute_matrix)
 
 
 def covariance_within_class(matrix_values, label):
     """
     Calculates the average covariance within all the classes in a dataset
     :param matrix_values: matrix with the values associated to the parameters of the dataset
     :param label: vector with the label values associated with the dataset
@@ -301,15 +318,15 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}')
+        print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def MVG_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
@@ -340,15 +357,15 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}')
+        print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def Naive_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
@@ -380,15 +397,15 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}')
+        print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def Naive_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
@@ -421,11 +438,115 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}')
+        print(f'Accuracy: {acc}%')
         print(f'Error: {(100 - acc)}%')
 
-    return SPost, predictions
+    return SPost, predictions
+
+
+def TiedGaussian(train_data, train_labels, test_data, prior_probability, test_label=[]):
+    '''
+    Calculates the model of the Tied Gaussian classifier for a set of data, and applyes it to a test dataset
+    :param train_date: matrix of the datapoints of a dataset used to train the model
+    :param train_labels: row vector with the labels associated with each row of the training dataset
+    :param test_data: matrix of the datapoints of a dataset used to test the model
+    :param test_labels: row vector with the labels associated with each row of the test dataset
+    :param prior_probability: col vector associated with the prior probability for each dimension
+    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return predictions: Vector associated with the prediction of the class for each test data point
+    '''
+    class_labels = np.unique(train_labels)
+    with_cov = covariance_within_class(train_data, train_labels)
+    multi_mu = multiclass_mean(train_data, train_labels)
+    densities = []
+    for i in range(class_labels.size):
+        densities.append(
+            np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), with_cov))
+        )
+    S = np.array(densities)
+
+    SJoint = S * prior_probability
+    SMarginal = vrow(SJoint.sum(0))
+    SPost = SJoint / SMarginal
+    predictions = np.argmax(SPost, axis=0)
+
+    if len(test_label) != 0:
+        acc = 0
+        for i in range(len(test_label)):
+            if predictions[i] == test_label[i]:
+                acc += 1
+        acc /= len(test_label)
+        print(f"Accuracy: {acc}")
+        print(f"Error: {1 - acc}")
+
+    return SPost, predictions
+
+def Tied_Naive_classifier(
+    train_data, train_labels, test_data, prior_probability, test_label=[]
+):
+    '''
+    Calculates the model of the Tied Naive classifier for a set of data, and applyes it to a test dataset
+    :param train_date: matrix of the datapoints of a dataset used to train the model
+    :param train_labels: row vector with the labels associated with each row of the training dataset
+    :param test_data: matrix of the datapoints of a dataset used to test the model
+    :param test_labels: row vector with the labels associated with each row of the test dataset
+    :param prior_probability: col vector associated with the prior probability for each dimension
+    :return SPost: matrix associated with the class posterior probabilty associated with each class
+    :return predictions: Vector associated with the prediction of the class for each test data point
+    '''
+    class_labels = np.unique(train_labels)
+    cov = covariance_within_class(train_data, train_labels)
+    identity = np.eye(cov.shape[1])
+    cov = cov * identity
+    multi_mu = multiclass_mean(train_data, train_labels)
+    densities = []
+    for i in range(class_labels.size):
+        densities.append(
+            np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov))
+        )
+    S = np.array(densities)
+    SJoint = S * prior_probability
+    SMarginal = vrow(SJoint.sum(0))
+    SPost = SJoint / SMarginal
+    predictions = np.argmax(SPost, axis=0)
+
+    if len(test_label) != 0:
+        acc = 0
+        for i in range(len(test_label)):
+            if predictions[i] == test_label[i]:
+                acc += 1
+        acc /= len(test_label)
+        print(f"Accuracy: {acc*100}%")
+        print(f"Error: {(1 - acc)*100}%")
+
+    return SPost, predictions
+
+
+
+def split_db(D, L, ratio, seed=0):
+    '''
+    Splits a dataset D into a training set and a validation set, based on the ratio
+    :param D: matrix of attributes of the dataset
+    :param L: vector of labels of the dataset
+    :param ratio: ratio used to divide the dataset (e.g. 2 / 3)
+    :param seed: seed for the random number generator of numpy (default 0)
+    :return (DTR, LTR), (DTE, LTE): (DTR, LTR) attributes and labels releated to the training sub-set. (DTE, LTE) attributes and labels releated to the testing sub-set.
+
+    '''
+    nTrain = int(D.shape[1] * ratio)
+    np.random.seed(seed)
+    idx = np.random.permutation(D.shape[1])
+    idxTrain = idx[0:nTrain]
+    idxTest = idx[nTrain:]
+
+    DTR = D[:, idxTrain]
+    DTE = D[:, idxTest]
+    LTR = L[idxTrain]
+    LTE = L[idxTest]
+
+    return (DTR, LTR), (DTE, LTE)
+
```

