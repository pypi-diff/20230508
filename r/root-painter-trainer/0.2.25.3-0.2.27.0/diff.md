# Comparing `tmp/root_painter_trainer-0.2.25.3.tar.gz` & `tmp/root_painter_trainer-0.2.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "root_painter_trainer-0.2.25.3.tar", last modified: Thu Feb  9 09:03:57 2023, max compression
+gzip compressed data, was "root_painter_trainer-0.2.27.0.tar", last modified: Mon May  8 10:40:42 2023, max compression
```

## Comparing `root_painter_trainer-0.2.25.3.tar` & `root_painter_trainer-0.2.27.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-02-09 09:03:57.437372 root_painter_trainer-0.2.25.3/
--rw-r--r--   0 abe        (501) staff       (20)     2397 2022-10-21 13:43:38.000000 root_painter_trainer-0.2.25.3/LICENSE
--rw-r--r--   0 abe        (501) staff       (20)     4702 2023-02-09 09:03:57.436698 root_painter_trainer-0.2.25.3/PKG-INFO
--rw-r--r--   0 abe        (501) staff       (20)     3711 2022-12-26 15:59:29.000000 root_painter_trainer-0.2.25.3/README.md
-drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-02-09 09:03:57.424782 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/
--rw-r--r--   0 abe        (501) staff       (20)     4702 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/PKG-INFO
--rw-r--r--   0 abe        (501) staff       (20)      521 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 abe        (501) staff       (20)        1 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 abe        (501) staff       (20)       62 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/entry_points.txt
--rw-r--r--   0 abe        (501) staff       (20)      120 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/requires.txt
--rw-r--r--   0 abe        (501) staff       (20)       21 2023-02-09 09:03:57.000000 root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/top_level.txt
--rw-r--r--   0 abe        (501) staff       (20)       38 2023-02-09 09:03:57.437553 root_painter_trainer-0.2.25.3/setup.cfg
--rw-r--r--   0 abe        (501) staff       (20)     1120 2023-02-09 09:03:20.000000 root_painter_trainer-0.2.25.3/setup.py
-drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-02-09 09:03:57.435268 root_painter_trainer-0.2.25.3/trainer/
--rw-r--r--   0 abe        (501) staff       (20)     1263 2022-10-21 13:43:38.000000 root_painter_trainer-0.2.25.3/trainer/__init__.py
--rw-r--r--   0 abe        (501) staff       (20)     6313 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/datasets.py
--rw-r--r--   0 abe        (501) staff       (20)     3248 2020-10-22 21:15:46.000000 root_painter_trainer-0.2.25.3/trainer/elastic.py
--rw-r--r--   0 abe        (501) staff       (20)      948 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/file_utils.py
--rw-r--r--   0 abe        (501) staff       (20)     9620 2023-01-30 16:04:37.000000 root_painter_trainer-0.2.25.3/trainer/im_utils.py
--rw-r--r--   0 abe        (501) staff       (20)     1710 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/loss.py
--rw-r--r--   0 abe        (501) staff       (20)     1509 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/main.py
--rw-r--r--   0 abe        (501) staff       (20)     2292 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/metrics.py
--rw-r--r--   0 abe        (501) staff       (20)     8669 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/model_utils.py
--rw-r--r--   0 abe        (501) staff       (20)     2914 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/startup.py
--rw-r--r--   0 abe        (501) staff       (20)    21578 2023-02-09 08:59:23.000000 root_painter_trainer-0.2.25.3/trainer/trainer.py
--rw-r--r--   0 abe        (501) staff       (20)     4565 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.25.3/trainer/unet.py
+drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-05-08 10:40:42.040247 root_painter_trainer-0.2.27.0/
+-rw-r--r--   0 abe        (501) staff       (20)     2397 2022-10-21 13:43:38.000000 root_painter_trainer-0.2.27.0/LICENSE
+-rw-r--r--   0 abe        (501) staff       (20)     5068 2023-05-08 10:40:42.039709 root_painter_trainer-0.2.27.0/PKG-INFO
+-rw-r--r--   0 abe        (501) staff       (20)     4554 2023-03-17 14:28:23.000000 root_painter_trainer-0.2.27.0/README.md
+drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-05-08 10:40:42.030539 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/
+-rw-r--r--   0 abe        (501) staff       (20)     5068 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 abe        (501) staff       (20)      521 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 abe        (501) staff       (20)        1 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 abe        (501) staff       (20)       62 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/entry_points.txt
+-rw-r--r--   0 abe        (501) staff       (20)      120 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/requires.txt
+-rw-r--r--   0 abe        (501) staff       (20)       21 2023-05-08 10:40:42.000000 root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/top_level.txt
+-rw-r--r--   0 abe        (501) staff       (20)       38 2023-05-08 10:40:42.040361 root_painter_trainer-0.2.27.0/setup.cfg
+-rw-r--r--   0 abe        (501) staff       (20)     1120 2023-05-08 10:35:11.000000 root_painter_trainer-0.2.27.0/setup.py
+drwxr-xr-x   0 abe        (501) staff       (20)        0 2023-05-08 10:40:42.039031 root_painter_trainer-0.2.27.0/trainer/
+-rw-r--r--   0 abe        (501) staff       (20)     1263 2022-10-21 13:43:38.000000 root_painter_trainer-0.2.27.0/trainer/__init__.py
+-rw-r--r--   0 abe        (501) staff       (20)     6313 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/datasets.py
+-rw-r--r--   0 abe        (501) staff       (20)     3248 2020-10-22 21:15:46.000000 root_painter_trainer-0.2.27.0/trainer/elastic.py
+-rw-r--r--   0 abe        (501) staff       (20)      948 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/file_utils.py
+-rw-r--r--   0 abe        (501) staff       (20)    10052 2023-04-19 15:04:54.000000 root_painter_trainer-0.2.27.0/trainer/im_utils.py
+-rw-r--r--   0 abe        (501) staff       (20)     1710 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/loss.py
+-rw-r--r--   0 abe        (501) staff       (20)     1509 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/main.py
+-rw-r--r--   0 abe        (501) staff       (20)     2292 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/metrics.py
+-rw-r--r--   0 abe        (501) staff       (20)     8903 2023-02-22 18:51:27.000000 root_painter_trainer-0.2.27.0/trainer/model_utils.py
+-rw-r--r--   0 abe        (501) staff       (20)     2914 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/startup.py
+-rw-r--r--   0 abe        (501) staff       (20)    21652 2023-05-06 10:37:27.000000 root_painter_trainer-0.2.27.0/trainer/trainer.py
+-rw-r--r--   0 abe        (501) staff       (20)     4565 2022-12-21 13:06:12.000000 root_painter_trainer-0.2.27.0/trainer/unet.py
```

### Comparing `root_painter_trainer-0.2.25.3/LICENSE` & `root_painter_trainer-0.2.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/PKG-INFO` & `root_painter_trainer-0.2.27.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 Metadata-Version: 2.1
 Name: root_painter_trainer
-Version: 0.2.25.3
+Version: 0.2.27.0
 Summary: Trainer (server component) for RootPainter
 Home-page: https://github.com/Abe404/root_painter
 Author: Abraham George Smith
 License: GPL-2.0
-Description: ## RootPainter
-        
-        Described in the paper "RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation"
-        
-        Published peer-reviewed paper available in the New Phytologist at:
-        [https://doi.org/10.1111/nph.18387](https://doi.org/10.1111/nph.18387)
-        
-        To see a list of work using (or citing) the RootPainter paper, please see the [google scholar page](https://scholar.google.com/scholar?cites=12740268016453642124)
-        
-        BioRxiv Pre-print available at:
-        [https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2](https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2)
-        
-        RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
-        RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.   
-        
-        ### Getting started quickly
-        
-         I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-         
-         A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements.
-         
-        ### Videos
-        A video demonstrating how to train and use a model is available to [download](https://nph.onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1111%2Fnph.18387&file=nph18387-sup-0002-VideoS1.mp4)
-        
-        There is a [youtube video](https://www.youtube.com/watch?v=73u73tBvRO4) of a workshop explaining the background behind the software and covering using the colab notebook to train and use a root segmentation model.
-        
-        
-        ### Client Downloads
-        
-        See [releases](https://github.com/Abe404/root_painter/releases) 
-        
-        If you are not confident installing and running python applications on the command line then to get started quickly I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-        
-        #### Server setup 
-        
-        The following instructions are for a local server. If you do not have a suitable NVIDIA GPU with at least 8GB of GPU memory then my current recommendation is to run via Google colab. A publicly available notebook is available at [Google Drive with Google Colab](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-        
-        Other options to run the server component of RootPainter on a remote machine include the [the sshfs server setup tutorial](https://github.com/Abe404/root_painter/blob/master/docs/server_setup_sshfs.md). You can also use Dropbox instead of sshfs.
-        
-        
-        For the next steps I assume you have a suitable GPU and CUDA installed.
-        
-        1. To install the RootPainter trainer:
-        
-        ```
-        pip install root-painter-trainer
-        ```
-        
-        2. To run the trainer.  This will first create the sync directory.
-        
-        ```
-        start-trainer
-        ```
-        
-        You will be prompted to input a location for the sync directory. This is the folder where files are shared between the client and server. I will use ~/root_painter_sync.
-        RootPainter will then create some folders inside ~/root_painter_sync.
-        The server should print the automatically selected batch size, which should be greater than 0. It will then start watching for instructions from the client.
-        
-        You should now be able to see the folders created by RootPainter (datasets, instructions and projects) inside ~/Desktop/root_painter_sync on your local machine 
-        See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model.
-        
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## RootPainter
+
+RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
+RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.  
+
+A detailed description is available in the paper published in the New Phytologist  [RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation](https://doi.org/10.1111/nph.18387)
+
+![RootPainter Interface](https://user-images.githubusercontent.com/376295/224013411-cb44c7c2-5c72-4819-98a3-6c0ab8b9ea4d.png)
+
+To see a list of work using (or citing) the RootPainter paper, please see the [google scholar page](https://scholar.google.com/scholar?cites=12740268016453642124)
+
+A BioRxiv Pre-print (earlier version of the paper) is available at:
+[https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2](https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2)
+
+
+### Getting started quickly
+
+ I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+ 
+ A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements. 
+ 
+ 
+ 
+
+ 
+### Videos
+A video demonstrating how to train and use a model is available to [download](https://nph.onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1111%2Fnph.18387&file=nph18387-sup-0002-VideoS1.mp4)
+
+There is a [youtube video](https://www.youtube.com/watch?v=73u73tBvRO4) of a workshop explaining the background behind the software and covering using the colab notebook to train and use a root segmentation model.
+
+
+### Client Downloads
+
+See [releases](https://github.com/Abe404/root_painter/releases) 
+
+If you are not confident installing and running python applications on the command line then to get started quickly I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+
+#### Server setup 
+
+The following instructions are for a local server. If you do not have a suitable NVIDIA GPU with at least 8GB of GPU memory then my current recommendation is to run via Google colab. A publicly available notebook is available at [Google Drive with Google Colab](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+
+Other options to run the server component of RootPainter on a remote machine include the [the sshfs server setup tutorial](https://github.com/Abe404/root_painter/blob/master/docs/server_setup_sshfs.md). You can also use Dropbox instead of sshfs.
+
+
+For the next steps I assume you have a suitable GPU and CUDA installed.
+
+1. To install the RootPainter trainer:
+
+```
+pip install root-painter-trainer
+```
+
+2. To run the trainer.  This will first create the sync directory.
+
+```
+start-trainer
+```
+
+You will be prompted to input a location for the sync directory. This is the folder where files are shared between the client and server. I will use ~/root_painter_sync.
+RootPainter will then create some folders inside ~/root_painter_sync.
+The server should print the automatically selected batch size, which should be greater than 0. It will then start watching for instructions from the client.
+
+You should now be able to see the folders created by RootPainter (datasets, instructions and projects) inside ~/Desktop/root_painter_sync on your local machine 
+See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model. I now actually suggest following the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing) instructions but using your local setup instead of the colab server, as these are easier to follow than the lung tutorial.
+
+
+ ### Questions and Problems
+ 
+The [FAQ](https://github.com/Abe404/root_painter/blob/master/docs/FAQ.md) may  be worth checking before reaching out with any questions you have. If you do have a question you can either email me or post in the [discussions](https://github.com/Abe404/root_painter/discussions). If you have an issue/ have identified a problem with the software then you can [post an issue](https://github.com/Abe404/root_painter/issues).
+
+
```

### Comparing `root_painter_trainer-0.2.25.3/README.md` & `root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,46 @@
+Metadata-Version: 2.1
+Name: root-painter-trainer
+Version: 0.2.27.0
+Summary: Trainer (server component) for RootPainter
+Home-page: https://github.com/Abe404/root_painter
+Author: Abraham George Smith
+License: GPL-2.0
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## RootPainter
 
-Described in the paper "RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation"
+RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
+RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.  
+
+A detailed description is available in the paper published in the New Phytologist  [RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation](https://doi.org/10.1111/nph.18387)
 
-Published peer-reviewed paper available in the New Phytologist at:
-[https://doi.org/10.1111/nph.18387](https://doi.org/10.1111/nph.18387)
+![RootPainter Interface](https://user-images.githubusercontent.com/376295/224013411-cb44c7c2-5c72-4819-98a3-6c0ab8b9ea4d.png)
 
 To see a list of work using (or citing) the RootPainter paper, please see the [google scholar page](https://scholar.google.com/scholar?cites=12740268016453642124)
 
-BioRxiv Pre-print available at:
+A BioRxiv Pre-print (earlier version of the paper) is available at:
 [https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2](https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2)
 
-RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
-RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.   
 
 ### Getting started quickly
 
  I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
  
- A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements.
+ A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements. 
+ 
+ 
+ 
+
  
 ### Videos
 A video demonstrating how to train and use a model is available to [download](https://nph.onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1111%2Fnph.18387&file=nph18387-sup-0002-VideoS1.mp4)
 
 There is a [youtube video](https://www.youtube.com/watch?v=73u73tBvRO4) of a workshop explaining the background behind the software and covering using the colab notebook to train and use a root segmentation model.
 
 
@@ -53,9 +72,15 @@
 ```
 
 You will be prompted to input a location for the sync directory. This is the folder where files are shared between the client and server. I will use ~/root_painter_sync.
 RootPainter will then create some folders inside ~/root_painter_sync.
 The server should print the automatically selected batch size, which should be greater than 0. It will then start watching for instructions from the client.
 
 You should now be able to see the folders created by RootPainter (datasets, instructions and projects) inside ~/Desktop/root_painter_sync on your local machine 
-See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model.
+See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model. I now actually suggest following the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing) instructions but using your local setup instead of the colab server, as these are easier to follow than the lung tutorial.
+
+
+ ### Questions and Problems
+ 
+The [FAQ](https://github.com/Abe404/root_painter/blob/master/docs/FAQ.md) may  be worth checking before reaching out with any questions you have. If you do have a question you can either email me or post in the [discussions](https://github.com/Abe404/root_painter/discussions). If you have an issue/ have identified a problem with the software then you can [post an issue](https://github.com/Abe404/root_painter/issues).
+
```

### Comparing `root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/PKG-INFO` & `root_painter_trainer-0.2.27.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,69 @@
-Metadata-Version: 2.1
-Name: root-painter-trainer
-Version: 0.2.25.3
-Summary: Trainer (server component) for RootPainter
-Home-page: https://github.com/Abe404/root_painter
-Author: Abraham George Smith
-License: GPL-2.0
-Description: ## RootPainter
-        
-        Described in the paper "RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation"
-        
-        Published peer-reviewed paper available in the New Phytologist at:
-        [https://doi.org/10.1111/nph.18387](https://doi.org/10.1111/nph.18387)
-        
-        To see a list of work using (or citing) the RootPainter paper, please see the [google scholar page](https://scholar.google.com/scholar?cites=12740268016453642124)
-        
-        BioRxiv Pre-print available at:
-        [https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2](https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2)
-        
-        RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
-        RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.   
-        
-        ### Getting started quickly
-        
-         I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-         
-         A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements.
-         
-        ### Videos
-        A video demonstrating how to train and use a model is available to [download](https://nph.onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1111%2Fnph.18387&file=nph18387-sup-0002-VideoS1.mp4)
-        
-        There is a [youtube video](https://www.youtube.com/watch?v=73u73tBvRO4) of a workshop explaining the background behind the software and covering using the colab notebook to train and use a root segmentation model.
-        
-        
-        ### Client Downloads
-        
-        See [releases](https://github.com/Abe404/root_painter/releases) 
-        
-        If you are not confident installing and running python applications on the command line then to get started quickly I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-        
-        #### Server setup 
-        
-        The following instructions are for a local server. If you do not have a suitable NVIDIA GPU with at least 8GB of GPU memory then my current recommendation is to run via Google colab. A publicly available notebook is available at [Google Drive with Google Colab](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
-        
-        Other options to run the server component of RootPainter on a remote machine include the [the sshfs server setup tutorial](https://github.com/Abe404/root_painter/blob/master/docs/server_setup_sshfs.md). You can also use Dropbox instead of sshfs.
-        
-        
-        For the next steps I assume you have a suitable GPU and CUDA installed.
-        
-        1. To install the RootPainter trainer:
-        
-        ```
-        pip install root-painter-trainer
-        ```
-        
-        2. To run the trainer.  This will first create the sync directory.
-        
-        ```
-        start-trainer
-        ```
-        
-        You will be prompted to input a location for the sync directory. This is the folder where files are shared between the client and server. I will use ~/root_painter_sync.
-        RootPainter will then create some folders inside ~/root_painter_sync.
-        The server should print the automatically selected batch size, which should be greater than 0. It will then start watching for instructions from the client.
-        
-        You should now be able to see the folders created by RootPainter (datasets, instructions and projects) inside ~/Desktop/root_painter_sync on your local machine 
-        See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model.
-        
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+## RootPainter
+
+RootPainter is a GUI-based software tool for the rapid training of deep neural networks for use in biological image analysis. 
+RootPainter uses a client-server architecture, allowing users with a typical laptop to utilise a GPU on a more computationally powerful server.  
+
+A detailed description is available in the paper published in the New Phytologist  [RootPainter: Deep Learning Segmentation of Biological Images with Corrective Annotation](https://doi.org/10.1111/nph.18387)
+
+![RootPainter Interface](https://user-images.githubusercontent.com/376295/224013411-cb44c7c2-5c72-4819-98a3-6c0ab8b9ea4d.png)
+
+To see a list of work using (or citing) the RootPainter paper, please see the [google scholar page](https://scholar.google.com/scholar?cites=12740268016453642124)
+
+A BioRxiv Pre-print (earlier version of the paper) is available at:
+[https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2](https://www.biorxiv.org/content/10.1101/2020.04.16.044461v2)
+
+
+### Getting started quickly
+
+ I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+ 
+ A  shorter [mini guide](https://github.com/Abe404/root_painter/blob/master/docs/mini_guide.md) is available including more concise instruction, that could be used as reference. I suggest the paper, videos and then colab tutorial to get an idea of how the software interface could be used and then this mini guide for reference to help remember each of the key steps to get from raw data to final measurements. 
+ 
+ 
+ 
+
+ 
+### Videos
+A video demonstrating how to train and use a model is available to [download](https://nph.onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1111%2Fnph.18387&file=nph18387-sup-0002-VideoS1.mp4)
+
+There is a [youtube video](https://www.youtube.com/watch?v=73u73tBvRO4) of a workshop explaining the background behind the software and covering using the colab notebook to train and use a root segmentation model.
+
+
+### Client Downloads
+
+See [releases](https://github.com/Abe404/root_painter/releases) 
+
+If you are not confident installing and running python applications on the command line then to get started quickly I suggest the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+
+#### Server setup 
+
+The following instructions are for a local server. If you do not have a suitable NVIDIA GPU with at least 8GB of GPU memory then my current recommendation is to run via Google colab. A publicly available notebook is available at [Google Drive with Google Colab](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing).
+
+Other options to run the server component of RootPainter on a remote machine include the [the sshfs server setup tutorial](https://github.com/Abe404/root_painter/blob/master/docs/server_setup_sshfs.md). You can also use Dropbox instead of sshfs.
+
+
+For the next steps I assume you have a suitable GPU and CUDA installed.
+
+1. To install the RootPainter trainer:
+
+```
+pip install root-painter-trainer
+```
+
+2. To run the trainer.  This will first create the sync directory.
+
+```
+start-trainer
+```
+
+You will be prompted to input a location for the sync directory. This is the folder where files are shared between the client and server. I will use ~/root_painter_sync.
+RootPainter will then create some folders inside ~/root_painter_sync.
+The server should print the automatically selected batch size, which should be greater than 0. It will then start watching for instructions from the client.
+
+You should now be able to see the folders created by RootPainter (datasets, instructions and projects) inside ~/Desktop/root_painter_sync on your local machine 
+See [lung tutorial](docs/cxr_lung_tutorial.md) for an example of how to use RootPainter to train a model. I now actually suggest following the [colab tutorial](https://colab.research.google.com/drive/104narYAvTBt-X4QEDrBSOZm_DRaAKHtA?usp=sharing) instructions but using your local setup instead of the colab server, as these are easier to follow than the lung tutorial.
+
+
+ ### Questions and Problems
+ 
+The [FAQ](https://github.com/Abe404/root_painter/blob/master/docs/FAQ.md) may  be worth checking before reaching out with any questions you have. If you do have a question you can either email me or post in the [discussions](https://github.com/Abe404/root_painter/discussions). If you have an issue/ have identified a problem with the software then you can [post an issue](https://github.com/Abe404/root_painter/issues).
```

### Comparing `root_painter_trainer-0.2.25.3/root_painter_trainer.egg-info/SOURCES.txt` & `root_painter_trainer-0.2.27.0/root_painter_trainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/setup.py` & `root_painter_trainer-0.2.27.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 current_dir = Path(__file__).parent
 long_description = io.open(current_dir / "README.md", mode="r", encoding="utf-8").read()
 
 setup(
   name = 'root_painter_trainer',
   package_dir = {'root_painter_trainer': 'trainer'},
   packages = ['root_painter_trainer'],
-  version = '0.2.25.3',
+  version = '0.2.27.0',
   license = 'GPL-2.0', 
   description = 'Trainer (server component) for RootPainter',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Abraham George Smith',
   url = 'https://github.com/Abe404/root_painter',
   entry_points={
```

### Comparing `root_painter_trainer-0.2.25.3/trainer/__init__.py` & `root_painter_trainer-0.2.27.0/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/datasets.py` & `root_painter_trainer-0.2.27.0/trainer/datasets.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/elastic.py` & `root_painter_trainer-0.2.27.0/trainer/elastic.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/file_utils.py` & `root_painter_trainer-0.2.27.0/trainer/file_utils.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/im_utils.py` & `root_painter_trainer-0.2.27.0/trainer/im_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,21 @@
             fnames = [a for a in fnames if is_photo(a)]
             fname = random.sample(fnames, 1)[0]
             annot_path = os.path.join(train_annot_dir, fname)
             image_path_part = os.path.join(dataset_dir,
                                            os.path.splitext(fname)[0])
             # it's possible the image has a different extenstion
             # so use glob to get it
+            
+            # Use glob.escape to allow arbitrary strings in file paths,
+            # including [ and ]  
+            # For related bug See https://github.com/Abe404/root_painter/issues/87
+            image_path_part = glob.escape(image_path_part)
             image_path = glob.glob(image_path_part + '.*')[0]
+            
             latest_im_path = image_path
             image = load_image(image_path)
             latest_annot_path = annot_path
             annot = imread(annot_path).astype(bool)
             assert np.sum(annot) > 0
             assert image.shape[2] == 3 # should be RGB
             # also return fname for debugging purposes.
@@ -237,14 +243,17 @@
             return
         time.sleep(0.1)
     raise Exception(f'Could not find image at {temp_path} '
                     f'after trying {max_attempts} times')
 
 def load_image(photo_path):
     photo = Image.open(photo_path)
+    # Convert to RGB before converting to NumPy due to bug in Pillow
+    # https://github.com/Abe404/root_painter/issues/94
+    photo = photo.convert("RGB")
     photo = ImageOps.exif_transpose(photo)
     photo = np.array(photo)
 
     # sometimes photo is a list where first element is the photo
     if len(photo.shape) == 1:
         photo = photo[0]
     # if 4 channels then convert to rgb
@@ -252,8 +261,9 @@
     if len(photo.shape) > 2 and photo.shape[2] == 4:
         photo = color.rgba2rgb(photo)
 
     # if image is black and white then change it to rgb
     # TODO: train directly on B/W instead of doing this conversion.
     if len(photo.shape) == 2:
         photo = color.gray2rgb(photo)
+
     return photo
```

### Comparing `root_painter_trainer-0.2.25.3/trainer/loss.py` & `root_painter_trainer-0.2.27.0/trainer/loss.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/main.py` & `root_painter_trainer-0.2.27.0/trainer/main.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/metrics.py` & `root_painter_trainer-0.2.27.0/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/model_utils.py` & `root_painter_trainer-0.2.27.0/trainer/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,20 @@
             time.sleep(0.1)
             annot = imread(annot_path)
 
         annot = np.array(annot)
         foreground = annot[:, :, 0].astype(bool).astype(int)
         background = annot[:, :, 1].astype(bool).astype(int)
         image_path_part = os.path.join(dataset_dir, os.path.splitext(fname)[0])
+
+        # Use glob.escape to allow arbitrary strings in file paths,
+        # including [ and ]  
+        # For related bug See https://github.com/Abe404/root_painter/issues/87
+        image_path_part = glob.escape(image_path_part)
+
         image_path = glob.glob(image_path_part + '.*')[0]
         image = im_utils.load_image(image_path)
         image, pad_settings = im_utils.pad_to_min(image, min_w=572, min_h=572)
         predicted = unet_segment(cnn, image, bs, in_w,
                                  out_w, threshold=0.5)
         predicted = im_utils.crop_from_pad_settings(predicted, pad_settings)
```

### Comparing `root_painter_trainer-0.2.25.3/trainer/startup.py` & `root_painter_trainer-0.2.27.0/trainer/startup.py`

 * *Files identical despite different names*

### Comparing `root_painter_trainer-0.2.25.3/trainer/trainer.py` & `root_painter_trainer-0.2.27.0/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,17 +277,21 @@
             # # calculate all the false positives, false negatives etc
             tps += torch.sum((foregrounds_list == 1) * (preds_list == 1)).cpu().numpy()
             tns += torch.sum((foregrounds_list == 0) * (preds_list == 0)).cpu().numpy()
             fps += torch.sum((foregrounds_list == 0) * (preds_list == 1)).cpu().numpy()
             fns += torch.sum((foregrounds_list == 1) * (preds_list == 0)).cpu().numpy()
             defined_total += torch.sum(defined_list > 0).cpu().numpy()
             loss_sum += loss.item() # float
-            sys.stdout.write(f"Training {(step+1) * self.bs}/"
-                             f"{len(train_loader.dataset)} "
-                             f" loss={round(loss.item(), 3)} \r")
+
+            # https://github.com/googlecolab/colabtools/issues/166
+            print(f"\rTraining: {(step+1) * self.bs}/"
+                  f"{len(train_loader.dataset)} "
+                  f" loss={round(loss.item(), 3)}",
+                  end='', flush=True)
+
             self.check_for_instructions() # could update training parameter
             if not self.training:
                 return
 
         duration = round(time.time() - epoch_start, 3)
         print('epoch train duration', duration)
         self.log_metrics('train', get_metrics(tps, fps, tns, fns,
```

### Comparing `root_painter_trainer-0.2.25.3/trainer/unet.py` & `root_painter_trainer-0.2.27.0/trainer/unet.py`

 * *Files identical despite different names*

