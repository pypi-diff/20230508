# Comparing `tmp/colititato-0.1.0.tar.gz` & `tmp/colititato-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colititato-0.1.0.tar", last modified: Sun May  7 21:46:24 2023, max compression
+gzip compressed data, was "colititato-0.1.1.tar", last modified: Sun May  7 22:14:55 2023, max compression
```

## Comparing `colititato-0.1.0.tar` & `colititato-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 21:46:24.468437 colititato-0.1.0/
--rw-r--r--   0 giannis    (501) staff       (20)     1066 2023-04-28 22:10:00.000000 colititato-0.1.0/LICENSE
--rw-r--r--   0 giannis    (501) staff       (20)     2307 2023-05-07 21:46:24.467792 colititato-0.1.0/PKG-INFO
--rw-r--r--   0 giannis    (501) staff       (20)     1720 2023-05-07 21:39:26.000000 colititato-0.1.0/README.md
-drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 21:46:24.462901 colititato-0.1.0/colititato/
--rw-r--r--   0 giannis    (501) staff       (20)        0 2023-04-28 22:12:44.000000 colititato-0.1.0/colititato/__init__.py
--rw-r--r--   0 giannis    (501) staff       (20)     5233 2023-05-05 22:32:20.000000 colititato-0.1.0/colititato/cli.py
-drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 21:46:24.465644 colititato-0.1.0/colititato.egg-info/
--rw-r--r--   0 giannis    (501) staff       (20)     2307 2023-05-07 21:46:24.000000 colititato-0.1.0/colititato.egg-info/PKG-INFO
--rw-r--r--   0 giannis    (501) staff       (20)      277 2023-05-07 21:46:24.000000 colititato-0.1.0/colititato.egg-info/SOURCES.txt
--rw-r--r--   0 giannis    (501) staff       (20)        1 2023-05-07 21:46:24.000000 colititato-0.1.0/colititato.egg-info/dependency_links.txt
--rw-r--r--   0 giannis    (501) staff       (20)       51 2023-05-07 21:46:24.000000 colititato-0.1.0/colititato.egg-info/entry_points.txt
--rw-r--r--   0 giannis    (501) staff       (20)       17 2023-05-07 21:46:24.000000 colititato-0.1.0/colititato.egg-info/top_level.txt
--rw-r--r--   0 giannis    (501) staff       (20)       38 2023-05-07 21:46:24.468664 colititato-0.1.0/setup.cfg
--rw-r--r--   0 giannis    (501) staff       (20)      970 2023-04-28 22:30:38.000000 colititato-0.1.0/setup.py
-drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 21:46:24.466825 colititato-0.1.0/tests/
--rw-r--r--   0 giannis    (501) staff       (20)        0 2023-04-30 20:39:53.000000 colititato-0.1.0/tests/__init__.py
--rw-r--r--   0 giannis    (501) staff       (20)     2803 2023-05-06 22:26:11.000000 colititato-0.1.0/tests/test_game.py
+drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 22:14:55.742339 colititato-0.1.1/
+-rw-r--r--   0 giannis    (501) staff       (20)     1066 2023-04-28 22:10:00.000000 colititato-0.1.1/LICENSE
+-rw-r--r--   0 giannis    (501) staff       (20)     2421 2023-05-07 22:14:55.741715 colititato-0.1.1/PKG-INFO
+-rw-r--r--   0 giannis    (501) staff       (20)     1834 2023-05-07 21:54:16.000000 colititato-0.1.1/README.md
+drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 22:14:55.735678 colititato-0.1.1/colititato/
+-rw-r--r--   0 giannis    (501) staff       (20)        0 2023-04-28 22:12:44.000000 colititato-0.1.1/colititato/__init__.py
+-rw-r--r--   0 giannis    (501) staff       (20)     5277 2023-05-07 22:12:02.000000 colititato-0.1.1/colititato/cli.py
+drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 22:14:55.739075 colititato-0.1.1/colititato.egg-info/
+-rw-r--r--   0 giannis    (501) staff       (20)     2421 2023-05-07 22:14:55.000000 colititato-0.1.1/colititato.egg-info/PKG-INFO
+-rw-r--r--   0 giannis    (501) staff       (20)      277 2023-05-07 22:14:55.000000 colititato-0.1.1/colititato.egg-info/SOURCES.txt
+-rw-r--r--   0 giannis    (501) staff       (20)        1 2023-05-07 22:14:55.000000 colititato-0.1.1/colititato.egg-info/dependency_links.txt
+-rw-r--r--   0 giannis    (501) staff       (20)       51 2023-05-07 22:14:55.000000 colititato-0.1.1/colititato.egg-info/entry_points.txt
+-rw-r--r--   0 giannis    (501) staff       (20)       17 2023-05-07 22:14:55.000000 colititato-0.1.1/colititato.egg-info/top_level.txt
+-rw-r--r--   0 giannis    (501) staff       (20)       38 2023-05-07 22:14:55.742518 colititato-0.1.1/setup.cfg
+-rw-r--r--   0 giannis    (501) staff       (20)      970 2023-05-07 22:13:24.000000 colititato-0.1.1/setup.py
+drwxr-xr-x   0 giannis    (501) staff       (20)        0 2023-05-07 22:14:55.740699 colititato-0.1.1/tests/
+-rw-r--r--   0 giannis    (501) staff       (20)        0 2023-04-30 20:39:53.000000 colititato-0.1.1/tests/__init__.py
+-rw-r--r--   0 giannis    (501) staff       (20)     2803 2023-05-06 22:26:11.000000 colititato-0.1.1/tests/test_game.py
```

### Comparing `colititato-0.1.0/LICENSE` & `colititato-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `colititato-0.1.0/PKG-INFO` & `colititato-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colititato
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI implementation of the classic Tic Tac Toe game
 Home-page: https://github.com/tiakas/colititato
 Author: Giannis Tiakas
 Author-email: giannis@tiakas.com
 Keywords: cli,tic-tat-toe,game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -66,14 +66,22 @@
 To build the package, use:
 ```
 python setup.py sdist bdist_wheel
 ```
 
 This will create a dist directory containing the source distribution (*.tar.gz) and wheel distribution (*.whl) of the package.
 
+Check the package contents:
+ ```
+ twine check dist/*
+ ```
+Upload the package to PyPI:
+```
+twine upload dist/*
+```
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contributing
 Contributions are always welcome! Here are some ways to contribute:
```

### Comparing `colititato-0.1.0/README.md` & `colititato-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,22 @@
 To build the package, use:
 ```
 python setup.py sdist bdist_wheel
 ```
 
 This will create a dist directory containing the source distribution (*.tar.gz) and wheel distribution (*.whl) of the package.
 
+Check the package contents:
+ ```
+ twine check dist/*
+ ```
+Upload the package to PyPI:
+```
+twine upload dist/*
+```
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contributing
 Contributions are always welcome! Here are some ways to contribute:
```

### Comparing `colititato-0.1.0/colititato/cli.py` & `colititato-0.1.1/colititato/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,18 +147,21 @@
         return self.player_wins + self.computer_wins + self.ties
 
     def __str__(self):
         return f'Score: Player {self.player_wins} - Computer {self.computer_wins} - Ties {self.ties}'
 
     def __repr__(self):
         return f'Scoreboard(player_wins={self.player_wins}, computer_wins={self.computer_wins}, ties={self.ties}, games_played={self.games_played})'
-    
-if __name__ == '__main__':
-    game = Game()
 
+def main():
+    game = Game()
+    game.select_marker()
     while True:
-        game.reset_board()
-        game.select_marker()
         game.play()
         if input('Play again? (Y/N): ').upper() != 'Y':
             print(game.scoreboard)
             break
+        game.reset_board()
+        game.select_marker()
+
+if __name__ == '__main__':
+    main()
```

### Comparing `colititato-0.1.0/colititato.egg-info/PKG-INFO` & `colititato-0.1.1/colititato.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colititato
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI implementation of the classic Tic Tac Toe game
 Home-page: https://github.com/tiakas/colititato
 Author: Giannis Tiakas
 Author-email: giannis@tiakas.com
 Keywords: cli,tic-tat-toe,game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -66,14 +66,22 @@
 To build the package, use:
 ```
 python setup.py sdist bdist_wheel
 ```
 
 This will create a dist directory containing the source distribution (*.tar.gz) and wheel distribution (*.whl) of the package.
 
+Check the package contents:
+ ```
+ twine check dist/*
+ ```
+Upload the package to PyPI:
+```
+twine upload dist/*
+```
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contributing
 Contributions are always welcome! Here are some ways to contribute:
```

### Comparing `colititato-0.1.0/setup.py` & `colititato-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='colititato',
-    version='0.1.0',
+    version='0.1.1',
     author='Giannis Tiakas',
     author_email='giannis@tiakas.com',
     description='A CLI implementation of the classic Tic Tac Toe game',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tiakas/colititato',
     packages=find_packages(),
```

### Comparing `colititato-0.1.0/tests/test_game.py` & `colititato-0.1.1/tests/test_game.py`

 * *Files identical despite different names*

