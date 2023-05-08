# Comparing `tmp/TCLR-1.5.0.tar.gz` & `tmp/TCLR-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-1.5.0.tar", last modified: Sun Aug 21 10:22:33 2022, max compression
+gzip compressed data, was "TCLR-1.6.0.tar", last modified: Mon May  8 04:09:51 2023, max compression
```

## Comparing `TCLR-1.5.0.tar` & `TCLR-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-08-21 10:22:33.549284 TCLR-1.5.0/
--rw-r--r--   0 jacob      (501) staff       (20)     3226 2022-08-21 10:22:33.549142 TCLR-1.5.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.5.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-08-21 10:22:33.548346 TCLR-1.5.0/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    34119 2022-08-21 10:12:14.000000 TCLR-1.5.0/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      952 2022-08-21 10:18:51.000000 TCLR-1.5.0/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2022-08-21 10:22:33.548950 TCLR-1.5.0/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3226 2022-08-21 10:22:33.000000 TCLR-1.5.0/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2022-08-21 10:22:33.000000 TCLR-1.5.0/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2022-08-21 10:22:33.000000 TCLR-1.5.0/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2022-08-21 10:22:33.000000 TCLR-1.5.0/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2022-08-21 10:22:33.000000 TCLR-1.5.0/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2022-08-21 10:22:33.549330 TCLR-1.5.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1438 2022-08-21 10:22:01.000000 TCLR-1.5.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.186305 TCLR-1.6.0/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:09:51.186183 TCLR-1.6.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.6.0/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.185430 TCLR-1.6.0/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    34848 2023-05-08 04:07:47.000000 TCLR-1.6.0/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.6.0/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:09:51.186014 TCLR-1.6.0/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-08 04:09:51.000000 TCLR-1.6.0/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-08 04:09:51.186347 TCLR-1.6.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-08 04:09:04.000000 TCLR-1.6.0/setup.py
```

### Comparing `TCLR-1.5.0/PKG-INFO` & `TCLR-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.5.0
+Version: 1.6.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
-Maintainer-email: 17734910905@163.com
+Maintainer-email: binjacobcao@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `TCLR-1.5.0/README.md` & `TCLR-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-1.5.0/TCLR/TCLRalgorithm.py` & `TCLR-1.6.0/TCLR/TCLRalgorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-"""
-    Tree Classifier for Linear Regression (TCLR) V1.5.0
-
-    TCLR is a novel tree model proposed by Prof.T-Y Zhang and Mr.Bin Cao et al. to capture the functional relationships
-    between features and target, which partitions the feature space into a set of rectangles, and embody a specific function in each one.
-    It is conceptually simple yet powerful for distinguishing mechanisms. The entire feature space is divided into disjointed
-    unit intervals by hyperplanes parallel to the coordinate axes. In each partition, we model target y as the function
-    of a feature xj (j = 1,⋯,m), linear function used in our studied problem.
-
-    It is worth noting that TCLR has the function of data screening by discarding which cannot be modeled functionally
-    on some resulting leaves. We chose the features and split-point to attain the best fit and recursive binary partitions the space,
-    until some stopping rules are applied.
-
-    Patent No. : 2021SR1951267, China
-    Reference : Domain knowledge guided interpretive machine learning ——  Formula discovery for the oxidation behavior of Ferritic-Martensitic steels in supercritical water. Bin Cao et al., 2022, JMI, journal paper.
-    DOI : 10.20517/jmi.2022.04
-"""
-
 import math
 import re
 from tabnanny import check
 from textwrap import indent
 import time
 import copy
 import os
@@ -43,103 +25,269 @@
         self.size = data.shape[0]
         self.R = 0
         self.bestFeature = 0
         self.bestValue = 0
         self.leaf_no = -1
 
 
-def PearsonR(X, Y):
-    xBar = np.mean(X)
-    yBar = np.mean(Y)
-    SSR = 0
-    varX = 0
-    varY = 0
-    if len(X) > 1:
-        for i in range(0, len(X)):
-            diffXXBar = X[i] - xBar
-            diffYYBar = Y[i] - yBar
-            SSR += (diffXXBar * diffYYBar)
-            varX += diffXXBar ** 2
-            varY += diffYYBar ** 2
-        SST = math.sqrt(varX * varY)
-    else:
-        SST = 1
-        SSR = 0
-    if SST == 0:
-        return 0
-    return SSR / SST
+def start(filePath, correlation='PearsonR(+)', minsize=3, threshold=0.95, mininc=0.01, split_tol = 0.8,tolerance_list = None , weight=True,
+         gplearn = False, gpl_dummyfea = None, population_size = 500, generations = 100, verbose = 1, 
+         metric = 'mean absolute error',
+         function_set = ['add', 'sub', 'mul', 'div', 'log', 'sqrt', 'abs', 'neg','inv','sin','cos','tan',]):
+    
+    """
+    Tree Classifier for Linear Regression (TCLR) 
 
+    TCLR is a new tree model proposed by Professor T-Y Zhang and Mr. Bin Cao et al. for capturing the functional relationships 
+    between features and target variables. The model partitions the feature space into a set of rectangles, with each partition
+    embodying a specific function. This approach is conceptually simple, yet powerful for distinguishing mechanisms. The entire
+    feature space is divided into disjointed unit intervals by hyperplanes parallel to the coordinate axes. Within each partition,
+    the target variable y is modeled as a linear function of a feature xj (j = 1,⋯,m), which is the linear function used in our studied problem.
+    
+    Patent No. : 2021SR1951267, China
+    Reference : Domain knowledge guided interpretive machine learning ——  Formula discovery for the oxidation behavior of Ferritic-Martensitic steels in supercritical water. Bin Cao et al., 2022, JMI, journal paper.
+    DOI : 10.20517/jmi.2022.04
 
-def MIC(X, Y):
-    if len(X) > 0:
-        mine = MINE(alpha=0.6, c=15)
-        mine.compute_score(X, Y)
-        return mine.mic()
-    else:
-        MICs = 0
-        return MICs
+    :param correlation : {'PearsonR(+)','PearsonR(-)',''MIC','R2'}, default PearsonR(+).
+            Methods:
+            * PearsonR: (+)(-). for linear relationship.
+            * MIC for no-linear relationship.
+            * R2 for no-linear relationship.
 
+            The evaluation factor for capture the functional relationship between feature and response
+            1>
+            PearsonR:
+            Pearson correlation coefficient, also known as Pearson's r, the Pearson product-moment correlation coefficient.
+            PearsonR is a measure of linear correlation between two sets of data. 
+            PearsonR = Cov(X,Y) / (sigmaX * sigmaY)
+        
+            2>
+            MIC:
+            The maximal information coefficient (MIC). MIC captures a wide range of associations both functional and not, 
+            and for functional relationships provides a score that roughly equals the coefficient of determination (R2) of 
+            the data relative to the regression function.  MIC belongs to a larger class of maximal information-based 
+            nonparametric exploration (MINE) statistics for identifying and classifying relationship.  
+            Reference : Reshef, D. N., Reshef, Y. A., Finucane, H. K., Grossman, S. R., McVean, G., Turnbaugh, P. J., ... 
+            and Sabeti, P. C. (2011). Detecting novel associations in large data sets. science, 334(6062), 1518-1524.
+            
+            3>
+            R2:
+            In statistics, the coefficient of determination, denoted R2 or r2 and pronounced "R squared", 
+            is the proportion of the variation in the dependent variable that is predictable from the independent variable(s).
+            t is a statistic used in the context of statistical models whose main purpose is either the prediction of future 
+            outcomes or the testing of hypotheses, on the basis of other related information. It provides a measure of how well
+            observed outcomes are replicated by the model, based on the proportion of total variation of outcomes explained by the model.
+            Definition from Wikipedia ：https://en.wikipedia.org/wiki/Coefficient_of_determination
+            R2 = 1 - SSres / SStot. Its value may be a negative one for poor correlation.
+ 
+  
+    :param minsize : 
+            a int number (default=3), minimum unique values for linear features of data on each leaf.
+    
+    :param threshold : 
+            a float (default=0.9), less than or equal to 1, default 0.95 for PearsonR.
+            In the process of dividing the dataset, the smallest relevant index allowed in the you research.
+            To avoid overfitting, threshold = 0.5 is suggested for MIC 0.5.
+    
+    :param mininc : Minimum expected gain of objective function (default=0.01)
 
-def R2(X, Y):
-    X = np.array(X)
-    Y = np.array(Y)
-    if len(X) > 0:
-        a = (X - np.mean(Y)) ** 2
-        SStot = np.sum(a)
-        b = (X - Y) ** 2
-        SSres = np.sum(b)
-        r2 = 1 - SSres / SStot
-        return r2
-    else:
-        r2 = -10
-        return r2
+    :param split_tol : a float (default=0.8), constrained features value shound be narrowed in a minmimu ratio of split_tol on split path
 
+    :param tolerance_list: 
+            constraints imposed on features, default is null
+            list shape in two dimensions, viz., [['feature_name1',tol_1],['feature_name2',tol_2]...]
+            'feature_name1', 'feature_name2' (string) are names of input features;
+            tol_1, tol_2 (float, between 0 to 1) are feature's tolerance ratios;
+            the variations of feature values on each leaf must be in the tolerance;
+            if tol_1 = 0, the value of feature 'feature_name1' must be a constant on each leaf,
+            if tol_1 = 1, there is no constraints on value of feature 'feature_name1';
+            example: tolerance_list = [['feature_name1',0.2],['feature_name2',0.1]].
 
-# Split the DataSet in a specific node
-def splitDataSet(dataSet, axis, value):
-    retDataSetA = []
-    retDataSetB = []
-    for featVec in dataSet:
-        if featVec[axis] <= value:
-            retDataSetA.append(featVec)
-        else:
-            retDataSetB.append(featVec)
-    return np.array(retDataSetA), np.array(retDataSetB)
+    :param weight:
+            The weight of the gain function, default is True.
+            When weight is True: linear_gain = R(father node) - ( W_l * R(left child node) + W_r * R(right child node)) / 2
+            Where W_l is the ratio of the number of samples in the left child node to the total number of samples ;
+                  W_r is the ratio of the number of samples in the right child node to the total number of samples.
+            When weight is False: linear_gain = R(father node) - ( R(left child node) + R(right child node)) / 2
 
-def fea_tol(dataSet,ori_dataSet,feats,tolerance_list):
-    if tolerance_list == None: return True
-    else:
-        record = 0
-        for i in range(len(tolerance_list)):
-            __feaname = tolerance_list[i][0]
-            __tolratio = float(tolerance_list[i][1])
-            index = feats.index(__feaname)
-            if (dataSet[:,index].max() - dataSet[:,index].min()) / (ori_dataSet[:,index].max()- ori_dataSet[:,index].min()) <= __tolratio:
-                record += 1
-        if record == len(tolerance_list):
-            return True
 
-def fea_tol_split(dataSet,ori_dataSet,feats,tolerance_list,split_tol):
-    if tolerance_list == None: return True
-    else:
-        record = 0
-        for i in range(len(tolerance_list)):
-            __feaname = tolerance_list[i][0]
-            __tolratio = float(tolerance_list[i][1])
-            criter = max(split_tol,__tolratio)
-            index = feats.index(__feaname)
-            if (dataSet[:,index].max() - dataSet[:,index].min()) / (ori_dataSet[:,index].max()- ori_dataSet[:,index].min()) <= criter:
-                record += 1
-        if record > int(0.5*len(tolerance_list)):
-            return True
+
+    :param gplearn : Whether to call the embedded gplearn package of TCLR to regress formula (default=False).
+    
+    :param gpl_dummyfea: 
+            dummy features in gpleran regression, default is null
+            list shape in one dimension, viz., ['feature_name1','feature_name2',...]
+            dummy features : 'feature_name1','feature_name2',... are not used anymore in gpleran regression 
+
+    :param population_size : integer, optional (default=500), the number of programs in each generation.
+    
+    :param generations : integer, optional (default=100),the number of generations to evolve.
+
+    :param verbose : int, optional (default=0). Controls the verbosity of the evolution building process.
+    
+    :param metric : 
+            str, optional (default='mean absolute error')
+            The name of the raw fitness metric. Available options include:
+            - 'mean absolute error'.
+            - 'mse' for mean squared error.
+            - 'rmse' for root mean squared error.
+            - 'pearson', for Pearson's product-moment correlation coefficient.
+            - 'spearman' for Spearman's rank-order correlation coefficient.
+    
+    :param function_set : 
+            iterable, optional (default=['add', 'sub', 'mul', 'div', 'log', 'sqrt', 
+                                               'abs', 'neg','inv','sin','cos','tan', 'max', 'min'])
+            The functions to use when building and evolving programs. This iterable can include strings 
+            to indicate either individual functions as outlined below.
+            Available individual functions are:
+            - 'add' : addition, arity=2.
+            - 'sub' : subtraction, arity=2.
+            - 'mul' : multiplication, arity=2.
+            - 'div' : protected division where a denominator near-zero returns 1.,
+                arity=2.
+            - 'sqrt' : protected square root where the absolute value of the
+                argument is used, arity=1.
+            - 'log' : protected log where the absolute value of the argument is
+                used and a near-zero argument returns 0., arity=1.
+            - 'abs' : absolute value, arity=1.
+            - 'neg' : negative, arity=1.
+            - 'inv' : protected inverse where a near-zero argument returns 0.,
+                arity=1.
+            - 'max' : maximum, arity=2.
+            - 'min' : minimum, arity=2.
+            - 'sin' : sine (radians), arity=1.
+            - 'cos' : cosine (radians), arity=1.
+            - 'tan' : tangent (radians), arity=1.
+    
+    Exampel :
+    #coding=utf-8
+    from TCLR import TCLRalgorithm as model
+
+    dataSet = "testdata.csv"
+    correlation = 'PearsonR(+)'
+    minsize = 3
+    threshold = 0.9
+    mininc = 0.01
+    split_tol = 0.8
+
+    model.start(filePath = dataSet, correlation = correlation, minsize = minsize, threshold = threshold,
+                mininc = mininc ,split_tol = split_tol,)
+    """
+
+    os.makedirs('Segmented', exist_ok=True)
+    # global var. for statisticaling  results
+    global record
+    record = 0
+    timename = time.localtime(time.time())
+    namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
+
+    csvData = pd.read_csv(filePath)
+    copy_csvData = copy.deepcopy(csvData)
+    copy_csvData['slope'] = None
+    copy_csvData['intercept'] = None
+    copy_csvData[correlation] = None
+    copy_csvData.to_csv('Segmented/all_dataset.csv', index=False)
+
+    feats = [column for column in csvData]
+    csvData = np.array(csvData)
+    root, _ = createTree(csvData, csvData, feats, 0, correlation,tolerance_list, minsize, threshold, mininc, split_tol,weight)
+    
+    print('All non-image results have been successfully saved!')
+    print('#'*80,'\n')
+   
+    # excute gplearn 
+    if gplearn == True :
+        if correlation == 'MIC' or correlation == 'R2':
+            print('{name} is a non-linear correlation metrics'.format(name = correlation ))
+            print('This is illegal, linear slopes are only allowed to generate when PearsonR is chosen')
+        elif correlation == 'PearsonR(+)' or correlation == 'PearsonR(-)':
+            sr_data = pd.read_csv('Segmented/all_dataset.csv')
+            sr_featurname = sr_data.columns
+            sr_data = np.array(sr_data)
+
+            if gpl_dummyfea == None: 
+
+                gpmodel = genetic.SymbolicRegressor(
+                    population_size = population_size, generations = generations, 
+                    verbose = verbose,feature_names = sr_featurname[:-4],function_set = function_set,
+                    metric = metric
+                    )
+                formula = gpmodel.fit(sr_data[:,:-4], sr_data[:,-3])
+                score = gpmodel.score(sr_data[:,:-4], sr_data[:,-3])
+                print( 'slope = ' + str(formula))
+
+            else:
+                # fea_num --> fea_loc
+                dummyfea = []
+                for i in range(len(gpl_dummyfea)):
+                    index = feats.index(gpl_dummyfea[i])
+                    dummyfea.append(index)
+                # remove fea_loc
+                index_array = [i for i in range(len(sr_featurname)-4)]
+                for i in range(len(gpl_dummyfea)):
+                    index_array.remove(dummyfea[i])
+                
+                gpmodel = genetic.SymbolicRegressor(
+                    population_size = population_size, generations = generations, 
+                    verbose = verbose,feature_names = sr_featurname[index_array],function_set = function_set,
+                    metric = metric
+                    )
+                formula = gpmodel.fit(sr_data[:,index_array], sr_data[:,-3])
+                score = gpmodel.score(sr_data[:,index_array], sr_data[:,-3])
+                print( 'slope = ' + str(formula))
+
+          
+            with open(os.path.join('Segmented', 'A_formula derived by gplearn.txt'), 'w') as wfid:
+                    print('Formula : ', file=wfid)
+                    print(str(formula), file=wfid)
+                    print('Fitness : ', file=wfid)
+                    print(str(metric) + ' = ' + str(score), file=wfid)
+                    print('\n', file=wfid)
+                    print('#'*80, file=wfid)
+                    print('Symbols annotation:', file=wfid)
+                    print('- add : addition, arity=2.', file=wfid)
+                    print('- sub : subtraction, arity=2.', file=wfid) 
+                    print('- mul : multiplication, arity=2.', file=wfid) 
+                    print('- div : protected division where a denominator near-zero returns 1.', file=wfid) 
+                    print('- sqrt : protected square root where the absolute value of the argument is used.', file=wfid) 
+                    print('- log : protected log where the absolute value of the argument is used.', file=wfid) 
+                    print('- abs : absolute value, arity=1.', file=wfid) 
+                    print('- neg : negative, arity=1.', file=wfid) 
+                    print('- inv : protected inverse where a near-zero argument returns 0.', file=wfid)  
+                    print('- max : maximum, arity=2.', file=wfid) 
+                    print('- sin : sine (radians), arity=1.', file=wfid) 
+                    print('- cos : cosine (radians), arity=1.', file=wfid)
+                    print('- tan : tangent (radians), arity=1.', file=wfid)  
+                 
+                        
+            
+    elif gplearn == False:
+        pass
+    
+
+    try:
+        # generate figure in pdf
+        warnings.filterwarnings('ignore')
+        dot = Digraph(comment='Result of TCLR')
+        render('A', root, dot, feats)
+        dot.render(
+            'Result of TCLR {year}.{month}.{day}-{hour}.{minute}'.format(year=namey, month=nameM, day=named, hour=nameh,
+                                                                        minute=namem))
+        return True
+    except :
+        print('Can not generate the Tree plot !')
+        print('Please ensure that the executable files of Graphviz are present on your system.')
+        print('See : https://github.com/Bin-Cao/TCLRmodel/tree/main/User%20Guide')
+        return True 
+  
 
 
 # Capture the functional relationships between features and target
 # Partitions the feature space into a set of rectangles,
-def createTree(dataSet, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol):
+def createTree(dataSet, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight):
     # It is a  positive linear relationship
     if correlation == 'PearsonR(+)':
         node = Node(dataSet)
         # Initial R0
         bestR = PearsonR(dataSet[:, -2], dataSet[:, -1])
         node.R = bestR
         __slope = stats.linregress(dataSet[:, -2], dataSet[:, -1])[0]
@@ -166,18 +314,15 @@
                     continue
                 subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
                 
                 if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                         subDataSetB[:, -2]).size <= minsize - 1:
                     continue
                 
-                newRa = PearsonR(subDataSetA[:, -2], subDataSetA[:, -1])
-                newRb = PearsonR(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                R = (newRa + newRb) / 2
+                R = weight_gain(subDataSetA,subDataSetB,weight,0)
 
                 if R - bestR >= mininc:
                     check_valve = True
                     splitSuccess = True
                     bestR = R
                     lc = subDataSetA
                     rc = subDataSetB
@@ -190,33 +335,32 @@
                 uniqueVals = sorted(list(set(featList)))
                 for value in range(len(uniqueVals) - 1):
                     subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
                     
                     if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                             subDataSetB[:, -2]).size <= minsize - 1:
                         continue
-                    newRa = PearsonR(subDataSetA[:, -2], subDataSetA[:, -1])
-                    newRb = PearsonR(subDataSetB[:, -2], subDataSetB[:, -1])
 
-                    R = (newRa + newRb) / 2
+                    R = weight_gain(subDataSetA,subDataSetB,weight,0)
+
                     if R - bestR >= mininc:
                         splitSuccess = True
                         bestR = R
                         lc = subDataSetA
                         rc = subDataSetB
                         bestFeature = i
                         bestValue = uniqueVals[value]
             else:
                 pass
                         
 
         # The recursive boundary is unable to find a division node that can increase factor(R, MIC, R2) by mininc or more.
         if splitSuccess:
-            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation, tolerance_list,minsize, threshold, mininc,split_tol)
-            node.rc, leaf_no = createTree(rc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol)
+            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation, tolerance_list,minsize, threshold, mininc,split_tol,weight)
+            node.rc, leaf_no = createTree(rc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight)
             node.bestFeature, node.bestValue = bestFeature, bestValue
 
         # This node is leaf
         if node.lc is None:
             node.leaf_no = leaf_no
             leaf_no += 1
             # determine if this node is to save in all_dataset.csv
@@ -257,18 +401,15 @@
                 subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
 
                 if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                         subDataSetB[:, -2]).size <= minsize - 1:
                     continue
 
                 
-                newRa = PearsonR(subDataSetA[:, -2], subDataSetA[:, -1])
-                newRb = PearsonR(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                R = (newRa + newRb) / 2
+                R = weight_gain(subDataSetA,subDataSetB,weight,0)
 
                 if R - bestR <= - mininc:
                     check_valve = True
                     splitSuccess = True
                     bestR = R
                     lc = subDataSetA
                     rc = subDataSetB
@@ -282,31 +423,28 @@
                 for value in range(len(uniqueVals) - 1):
                     subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
 
                     if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                             subDataSetB[:, -2]).size <= minsize - 1:
                         continue
                     
-                    newRa = PearsonR(subDataSetA[:, -2], subDataSetA[:, -1])
-                    newRb = PearsonR(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                    R = (newRa + newRb) / 2
+                    R = weight_gain(subDataSetA,subDataSetB,weight,0)
 
                     if R - bestR <= - mininc:
                         splitSuccess = True
                         bestR = R
                         lc = subDataSetA
                         rc = subDataSetB
                         bestFeature = i
                         bestValue = uniqueVals[value]
         else: pass
 
         if splitSuccess:
-            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol)
-            node.rc, leaf_no = createTree(rc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol)
+            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight)
+            node.rc, leaf_no = createTree(rc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight)
             node.bestFeature, node.bestValue = bestFeature, bestValue
 
         if node.lc is None:
             node.leaf_no = leaf_no
             leaf_no += 1
             # determine if this node is to save in all_dataset.csv
             save_in_all = False
@@ -341,18 +479,15 @@
                 if not fea_tol_split(dataSet,ori_dataset,feats,tolerance_list,split_tol):
                     continue
                 subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
                 if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                         subDataSetB[:, -2]).size <= minsize - 1:
                     continue
                 
-                newRa = MIC(subDataSetA[:, -2], subDataSetA[:, -1])
-                newRb = MIC(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                R = (newRa + newRb) / 2
+                R = weight_gain(subDataSetA,subDataSetB,weight,1)
 
                 if R - bestR >= mininc:
                     check_valve = True
                     splitSuccess = True
                     bestR = R
                     lc = subDataSetA
                     rc = subDataSetB
@@ -365,31 +500,28 @@
                 uniqueVals = sorted(list(set(featList)))
                 for value in range(len(uniqueVals) - 1):
                     subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
                     if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                             subDataSetB[:, -2]).size <= minsize - 1:
                         continue
     
-                    newRa = MIC(subDataSetA[:, -2], subDataSetA[:, -1])
-                    newRb = MIC(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                    R = (newRa + newRb) / 2
+                    R = weight_gain(subDataSetA,subDataSetB,weight,1)
 
                     if R - bestR >= mininc:
                         splitSuccess = True
                         bestR = R
                         lc = subDataSetA
                         rc = subDataSetB
                         bestFeature = i
                         bestValue = uniqueVals[value]
         else: pass
 
         if splitSuccess:
-            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol)
-            node.rc, leaf_no = createTree(rc,ori_dataset, feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol)
+            node.lc, leaf_no = createTree(lc, ori_dataset,feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight)
+            node.rc, leaf_no = createTree(rc,ori_dataset, feats, leaf_no, correlation,tolerance_list, minsize, threshold, mininc,split_tol,weight)
             node.bestFeature, node.bestValue = bestFeature, bestValue
 
         if node.lc is None:
             node.leaf_no = leaf_no
             leaf_no += 1
             # determine if this node is to save in all_dataset.csv
             save_in_all = False
@@ -426,18 +558,15 @@
 
                 subDataSetA, subDataSetB = splitDataSet(dataSet, i, uniqueVals[value])
 
                 if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                         subDataSetB[:, -2]).size <= minsize - 1:
                     continue
 
-                newRa = R2(subDataSetA[:, -2], subDataSetA[:, -1])
-                newRb = R2(subDataSetB[:, -2], subDataSetB[:, -1])
-
-                R = (newRa + newRb) / 2
+                R = weight_gain(subDataSetA,subDataSetB,weight,2)
 
                 if R - bestR >= mininc:
                     check_valve = True
                     splitSuccess = True
                     bestR = R
                     lc = subDataSetA
                     rc = subDataSetB
@@ -449,18 +578,16 @@
                 featList = [example[i] for example in dataSet]
                 uniqueVals = sorted(list(set(featList)))
 
                 for value in range(len(uniqueVals) - 1):
                     if np.unique(subDataSetA[:, -2]).size <= minsize - 1 or np.unique(
                             subDataSetB[:, -2]).size <= minsize - 1:
                         continue
-                    newRa = R2(subDataSetA[:, -2], subDataSetA[:, -1])
-                    newRb = R2(subDataSetB[:, -2], subDataSetB[:, -1])
 
-                    R = (newRa + newRb) / 2
+                    R = weight_gain(subDataSetA,subDataSetB,weight,2)
 
                     if R - bestR >= mininc:
                         splitSuccess = True
                         bestR = R
                         lc = subDataSetA
                         rc = subDataSetB
                         bestFeature = i
@@ -480,14 +607,100 @@
             if node.R >= threshold and fea_tol(node.data,feats,tolerance_list) == True:
                 save_in_all = True 
             write_csv(node, feats, save_in_all, correlation)
 
         return node, leaf_no
 
 
+def PearsonR(X, Y):
+    xBar = np.mean(X)
+    yBar = np.mean(Y)
+    SSR = 0
+    varX = 0
+    varY = 0
+    if len(X) > 1:
+        for i in range(0, len(X)):
+            diffXXBar = X[i] - xBar
+            diffYYBar = Y[i] - yBar
+            SSR += (diffXXBar * diffYYBar)
+            varX += diffXXBar ** 2
+            varY += diffYYBar ** 2
+        SST = math.sqrt(varX * varY)
+    else:
+        SST = 1
+        SSR = 0
+    if SST == 0:
+        return 0
+    return SSR / SST
+
+
+def MIC(X, Y):
+    if len(X) > 0:
+        mine = MINE(alpha=0.6, c=15)
+        mine.compute_score(X, Y)
+        return mine.mic()
+    else:
+        MICs = 0
+        return MICs
+
+
+def R2(X, Y):
+    X = np.array(X)
+    Y = np.array(Y)
+    if len(X) > 0:
+        a = (X - np.mean(Y)) ** 2
+        SStot = np.sum(a)
+        b = (X - Y) ** 2
+        SSres = np.sum(b)
+        r2 = 1 - SSres / SStot
+        return r2
+    else:
+        r2 = -10
+        return r2
+
+
+# Split the DataSet in a specific node
+def splitDataSet(dataSet, axis, value):
+    retDataSetA = []
+    retDataSetB = []
+    for featVec in dataSet:
+        if featVec[axis] <= value:
+            retDataSetA.append(featVec)
+        else:
+            retDataSetB.append(featVec)
+    return np.array(retDataSetA), np.array(retDataSetB)
+
+def fea_tol(dataSet,ori_dataSet,feats,tolerance_list):
+    if tolerance_list == None: return True
+    else:
+        record = 0
+        for i in range(len(tolerance_list)):
+            __feaname = tolerance_list[i][0]
+            __tolratio = float(tolerance_list[i][1])
+            index = feats.index(__feaname)
+            if (dataSet[:,index].max() - dataSet[:,index].min()) / (ori_dataSet[:,index].max()- ori_dataSet[:,index].min()) <= __tolratio:
+                record += 1
+        if record == len(tolerance_list):
+            return True
+
+def fea_tol_split(dataSet,ori_dataSet,feats,tolerance_list,split_tol):
+    if tolerance_list == None: return True
+    else:
+        record = 0
+        for i in range(len(tolerance_list)):
+            __feaname = tolerance_list[i][0]
+            __tolratio = float(tolerance_list[i][1])
+            criter = max(split_tol,__tolratio)
+            index = feats.index(__feaname)
+            if (dataSet[:,index].max() - dataSet[:,index].min()) / (ori_dataSet[:,index].max()- ori_dataSet[:,index].min()) <= criter:
+                record += 1
+        if record > int(0.5*len(tolerance_list)):
+            return True
+
+
 # Use graphviz to visualize the TCLR
 def render(label, node, dot, feats):
     mark = ''
     if node.slope == None:
         mark = "#=" + str(node.size) + " , ρ=" + str(round(node.R, 3))
     else:
         mark = "#=" + str(node.size) + " , ρ=" + str(round(node.R, 3)) + ' , slope=' + str(
@@ -533,217 +746,29 @@
 
     _all_dataset = pd.read_csv('./Segmented/all_dataset.csv')
     for item in range(len(frame.iloc[:, 0])):
         _all_dataset.iloc[item + record, :] = frame.iloc[item, :]
     record += len(frame.iloc[:, 0])
     _all_dataset.to_csv('Segmented/all_dataset.csv', index=False)
 
-
-def start(filePath, correlation='PearsonR(+)',tolerance_list = None , gpl_dummyfea = None, minsize=3, threshold=0.95, mininc=0.01, split_tol = 0.8,
-         gplearn = False, population_size = 500, generations = 100, verbose = 1, 
-         metric = 'mean absolute error',
-         function_set = ['add', 'sub', 'mul', 'div', 'log', 'sqrt', 'abs', 'neg','inv','sin','cos','tan', 'max', 'min']):
-    
-    """
-    :param correlation : {'PearsonR(+)','PearsonR(-)',''MIC','R2'}，default PearsonR(+).
-            Methods:
-            * PearsonR: (+)(-). for linear relationship.
-            * MIC for no-linear relationship.
-            * R2 for no-linear relationship.
-
-            The evaluation factor for capture the functional relationship between feature and response
-            1>
-            PearsonR:
-            Pearson correlation coefficient, also known as Pearson's r, the Pearson product-moment correlation coefficient.
-            PearsonR is a measure of linear correlation between two sets of data. 
-            PearsonR = Cov(X,Y) / (sigmaX * sigmaY)
-        
-            2>
-            MIC:
-            The maximal information coefficient (MIC). MIC captures a wide range of associations both functional and not, 
-            and for functional relationships provides a score that roughly equals the coefficient of determination (R2) of 
-            the data relative to the regression function.  MIC belongs to a larger class of maximal information-based 
-            nonparametric exploration (MINE) statistics for identifying and classifying relationship.  
-            Reference : Reshef, D. N., Reshef, Y. A., Finucane, H. K., Grossman, S. R., McVean, G., Turnbaugh, P. J., ... 
-            and Sabeti, P. C. (2011). Detecting novel associations in large data sets. science, 334(6062), 1518-1524.
-            
-            3>
-            R2:
-            In statistics, the coefficient of determination, denoted R2 or r2 and pronounced "R squared", 
-            is the proportion of the variation in the dependent variable that is predictable from the independent variable(s).
-            t is a statistic used in the context of statistical models whose main purpose is either the prediction of future 
-            outcomes or the testing of hypotheses, on the basis of other related information. It provides a measure of how well
-            observed outcomes are replicated by the model, based on the proportion of total variation of outcomes explained by the model.
-            Definition from Wikipedia ：https://en.wikipedia.org/wiki/Coefficient_of_determination
-            R2 = 1 - SSres / SStot. Its value may be a negative one for poor correlation.
- 
-    :param tolerance_list: constraints imposed on features, default is null
-            list shape in two dimensions, viz., [['feature_name1',tol_1],['feature_name2',tol_2]...]
-            'feature_name1', 'feature_name2' （string） are names of input features;
-            tol_1, tol_2 （float, between 0 to 1）are feature's tolerance ratios;
-            the variations of feature values on each leaf must be in the tolerance;
-            if tol_1 = 0, the value of feature 'feature_name1' must be a constant on each leaf,
-            if tol_1 = 1, there is no constraints on value of feature 'feature_name1';
-            example: tolerance_list = [['feature_name1',0.2],['feature_name2',0.1]].
-
-    :param gpl_dummyfea: dummy features in gpleran regression, default is null
-            list shape in one dimension, viz., ['feature_name1','feature_name2',...]
-            dummy features : 'feature_name1','feature_name2',... are not used anymore in gpleran regression 
-
-    :param minsize : a int number (default=3), minimum unique values for linear features of data on each leaf.
-    
-    :param threshold : a float (default=0.9), less than or equal to 1, default 0.95 for PearsonR.
-            In the process of dividing the dataset, the smallest relevant index allowed in the you research.
-            To avoid overfitting, threshold = 0.5 is suggested for MIC 0.5.
-    
-    :param mininc : Minimum expected gain of objective function (default=0.01)
-
-    :param split_tol : a float (default=0.8), constrained features value shound be narrowed in a minmimu ratio of split_tol on split path
-
-    :param gplearn : Whether to call the embedded gplearn package of TCLR to regress formula (default=False).
-    
-    :param population_size : integer, optional (default=500), the number of programs in each generation.
-    
-    :param generations : integer, optional (default=100),the number of generations to evolve.
-
-    :param verbose : int, optional (default=0). Controls the verbosity of the evolution building process.
-    
-    :param metric : str, optional (default='mean absolute error')
-            The name of the raw fitness metric. Available options include:
-            - 'mean absolute error'.
-            - 'mse' for mean squared error.
-            - 'rmse' for root mean squared error.
-            - 'pearson', for Pearson's product-moment correlation coefficient.
-            - 'spearman' for Spearman's rank-order correlation coefficient.
-    
-    :param function_set : iterable, optional (default=['add', 'sub', 'mul', 'div', 'log', 'sqrt', 
-                                               'abs', 'neg','inv','sin','cos','tan', 'max', 'min'])
-            The functions to use when building and evolving programs. This iterable can include strings 
-            to indicate either individual functions as outlined below.
-            Available individual functions are:
-            - 'add' : addition, arity=2.
-            - 'sub' : subtraction, arity=2.
-            - 'mul' : multiplication, arity=2.
-            - 'div' : protected division where a denominator near-zero returns 1.,
-                arity=2.
-            - 'sqrt' : protected square root where the absolute value of the
-                argument is used, arity=1.
-            - 'log' : protected log where the absolute value of the argument is
-                used and a near-zero argument returns 0., arity=1.
-            - 'abs' : absolute value, arity=1.
-            - 'neg' : negative, arity=1.
-            - 'inv' : protected inverse where a near-zero argument returns 0.,
-                arity=1.
-            - 'max' : maximum, arity=2.
-            - 'min' : minimum, arity=2.
-            - 'sin' : sine (radians), arity=1.
-            - 'cos' : cosine (radians), arity=1.
-            - 'tan' : tangent (radians), arity=1.
-    """
-    
-
-    os.makedirs('Segmented', exist_ok=True)
-    # global var. for statisticaling  results
-    global record
-    record = 0
-    timename = time.localtime(time.time())
-    namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
-
-    csvData = pd.read_csv(filePath)
-    copy_csvData = copy.deepcopy(csvData)
-    copy_csvData['slope'] = None
-    copy_csvData['intercept'] = None
-    copy_csvData[correlation] = None
-    copy_csvData.to_csv('Segmented/all_dataset.csv', index=False)
-
-    feats = [column for column in csvData]
-    csvData = np.array(csvData)
-    root, _ = createTree(csvData, csvData, feats, 0, correlation,tolerance_list, minsize, threshold, mininc, split_tol)
-    
-    print('All non-image results have been successfully saved!')
-    print('________________________________________________________________________________','\n')
-   
-    # excute gplearn 
-    if gplearn == True :
-        if correlation == 'MIC' or correlation == 'R2':
-            print('{name} is a non-linear correlation metrics'.format(name = correlation ))
-            print('This is illegal, linear slopes are only allowed to generate when PearsonR is chosen')
-        elif correlation == 'PearsonR(+)' or correlation == 'PearsonR(-)':
-            sr_data = pd.read_csv('Segmented/all_dataset.csv')
-            sr_featurname = sr_data.columns
-            sr_data = np.array(sr_data)
-
-            if gpl_dummyfea == None: 
-
-                gpmodel = genetic.SymbolicRegressor(
-                    population_size = population_size, generations = generations, 
-                    verbose = verbose,feature_names = sr_featurname[:-4],function_set = function_set,
-                    metric = metric
-                    )
-                formula = gpmodel.fit(sr_data[:,:-4], sr_data[:,-3])
-                score = gpmodel.score(sr_data[:,:-4], sr_data[:,-3])
-                print( 'slope = ' + str(formula))
-
-            else:
-                # fea_num --> fea_loc
-                dummyfea = []
-                for i in range(len(gpl_dummyfea)):
-                    index = feats.index(gpl_dummyfea[i])
-                    dummyfea.append(index)
-                # remove fea_loc
-                index_array = [i for i in range(len(sr_featurname)-4)]
-                for i in range(len(gpl_dummyfea)):
-                    index_array.remove(dummyfea[i])
-                
-                gpmodel = genetic.SymbolicRegressor(
-                    population_size = population_size, generations = generations, 
-                    verbose = verbose,feature_names = sr_featurname[index_array],function_set = function_set,
-                    metric = metric
-                    )
-                formula = gpmodel.fit(sr_data[:,index_array], sr_data[:,-3])
-                score = gpmodel.score(sr_data[:,index_array], sr_data[:,-3])
-                print( 'slope = ' + str(formula))
-
-          
-            with open(os.path.join('Segmented', 'A_formula derived by gplearn.txt'), 'w') as wfid:
-                    print('Formula : ', file=wfid)
-                    print(str(formula), file=wfid)
-                    print('Fitness : ', file=wfid)
-                    print(str(metric) + ' = ' + str(score), file=wfid)
-                    print('\n', file=wfid)
-                    print('_______________________________________________________________________________', file=wfid)
-                    print('Symbols annotation:', file=wfid)
-                    print('- add : addition, arity=2.', file=wfid)
-                    print('- sub : subtraction, arity=2.', file=wfid) 
-                    print('- mul : multiplication, arity=2.', file=wfid) 
-                    print('- div : protected division where a denominator near-zero returns 1.', file=wfid) 
-                    print('- sqrt : protected square root where the absolute value of the argument is used.', file=wfid) 
-                    print('- log : protected log where the absolute value of the argument is used.', file=wfid) 
-                    print('- abs : absolute value, arity=1.', file=wfid) 
-                    print('- neg : negative, arity=1.', file=wfid) 
-                    print('- inv : protected inverse where a near-zero argument returns 0.', file=wfid)  
-                    print('- max : maximum, arity=2.', file=wfid) 
-                    print('- sin : sine (radians), arity=1.', file=wfid) 
-                    print('- cos : cosine (radians), arity=1.', file=wfid)
-                    print('- tan : tangent (radians), arity=1.', file=wfid)  
-                 
-                        
-            
-    elif gplearn == False:
-        pass
-    
-
-    try:
-        # generate figure in pdf
-        warnings.filterwarnings('ignore')
-        dot = Digraph(comment='Result of TCLR')
-        render('A', root, dot, feats)
-        dot.render(
-            'Result of TCLR {year}.{month}.{day}-{hour}.{minute}'.format(year=namey, month=nameM, day=named, hour=nameh,
-                                                                        minute=namem))
-        return True
-    except :
-        print('Can not generate the Tree figure !')
-        print('Please make sure the Graphviz executables are on your systems')
-        return True 
+def weight_gain(subDataSetA,subDataSetB,weight,matrix):
+    if matrix == 0:
+        newRa = PearsonR(subDataSetA[:, -2], subDataSetA[:, -1])
+        newRb = PearsonR(subDataSetB[:, -2], subDataSetB[:, -1])
+    elif matrix == 1:
+        newRa = MIC(subDataSetA[:, -2], subDataSetA[:, -1])
+        newRb = MIC(subDataSetB[:, -2], subDataSetB[:, -1])
+    elif matrix == 2:
+        newRa = R2(subDataSetA[:, -2], subDataSetA[:, -1])
+        newRb = R2(subDataSetB[:, -2], subDataSetB[:, -1])
   
 
+    if weight == False:
+        R = (newRa + newRb) / 2
+        return R
+    elif weight == True:
+        weightRa = len(subDataSetA[:, -1]) / (subDataSetA[:, -1] + subDataSetB[:, -1])
+        weightRb = len(subDataSetB[:, -1]) / (subDataSetA[:, -1] + subDataSetB[:, -1])
+        R = weightRa * newRa + weightRb * newRb
+        return R
+    else:
+        print('Parameter error | weight')
```

### Comparing `TCLR-1.5.0/TCLR.egg-info/PKG-INFO` & `TCLR-1.6.0/TCLR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.5.0
+Version: 1.6.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
-Maintainer-email: 17734910905@163.com
+Maintainer-email: binjacobcao@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `TCLR-1.5.0/setup.py` & `TCLR-1.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='1.5.0',  # 版本
+    version='1.6.0',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
-    maintainer_email='17734910905@163.com',  # 维护者邮件
+    maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
     license='MIT License',  # 协议
     url='https://github.com/Bin-Cao/TCLRmodel',  # github或者自己的网站地址
     packages=find_packages(include=['TCLR', 'TCLR.*']),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

