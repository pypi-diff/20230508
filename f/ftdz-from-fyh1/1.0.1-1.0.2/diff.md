# Comparing `tmp/ftdz_from_fyh1-1.0.1.tar.gz` & `tmp/ftdz_from_fyh1-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ftdz_from_fyh1-1.0.1.tar", last modified: Mon May  8 11:46:19 2023, max compression
+gzip compressed data, was "dist\ftdz_from_fyh1-1.0.2.tar", last modified: Mon May  8 12:03:27 2023, max compression
```

## Comparing `ftdz_from_fyh1-1.0.1.tar` & `ftdz_from_fyh1-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/
--rw-rw-rw-   0        0        0      408 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh1-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/
--rw-rw-rw-   0        0        0     9803 2023-05-08 11:44:53.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/__init__.py
--rw-rw-rw-   0        0        0    22195 2023-04-23 11:38:18.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/main.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/
--rw-rw-rw-   0        0        0      408 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/ftdz_from_fyh1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 11:46:19.000000 ftdz_from_fyh1-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      518 2023-05-08 11:45:19.000000 ftdz_from_fyh1-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/
+-rw-rw-rw-   0        0        0      408 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_from_fyh1-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1/
+-rw-rw-rw-   0        0        0     9803 2023-05-08 11:44:53.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1/__init__.py
+-rw-rw-rw-   0        0        0    21339 2023-05-08 11:58:38.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-05-08 12:03:26.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 12:03:26.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 12:03:26.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 12:03:26.000000 ftdz_from_fyh1-1.0.2/ftdz_from_fyh1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 12:03:27.000000 ftdz_from_fyh1-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      518 2023-05-08 12:02:47.000000 ftdz_from_fyh1-1.0.2/setup.py
```

### Comparing `ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/__init__.py` & `ftdz_from_fyh1-1.0.2/ftdz_from_fyh1/__init__.py`

 * *Files identical despite different names*

### Comparing `ftdz_from_fyh1-1.0.1/ftdz_from_fyh1/main.py` & `ftdz_from_fyh1-1.0.2/ftdz_from_fyh1/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,26 +216,14 @@
         self.g = pg.image.load("19.jpg")
         self.g_r = self.g.get_rect()
         self.g_r.top = self.ai.br.top
         self.g_r.x = 420
         self.g_r.y = 600 - 123
     def d_g(self):
         self.ai.sc.blit(self.g,self.g_r)
-class Music:
-    def __init__(self,ai):
-        self.ai = ai
-        self.k = pg.image.load("sn.png")
-        self.k1 = pg.image.load("sn1.png")
-        self.image = self.k
-        self.k_r = self.k.get_rect()
-        self.k_r.y = self.ai.li.s_l_r.bottom + 11
-        pg.mixer.music.load("1.mp3")
-        pg.mixer.music.play(-1)
-    def d_k(self):
-        self.ai.sc.blit(self.image,self.k_r)
 class Help:
     def __init__(self,ai):
         self.ai = ai
         self.l = pg.image.load("help2.png")
         self.l1 = pg.image.load("help1.png")
         self.l3 = pg.image.load("90.jpg")
         self.l2 = pg.image.load("c2.png")
@@ -310,15 +298,14 @@
         self.button = Button(self)
         self.skills = Skills(self)
         self.box = Box(self)
         self.s_b = S_B(self)
         self.li = Life(self)
         self.sw = Switch(self)
         self.sh = Shield(self)
-        self.music = Music(self)
         self.help = Help(self)
         self.bullet = pg.sprite.Group()
         self.ene = pg.sprite.Group()
         self.a_b = pg.sprite.Group()
         self.base = pg.sprite.Group()
         self.br.left = self.width // 2
         self.c_f()
@@ -465,21 +452,14 @@
                 if self.sw.i_r.collidepoint(event.pos):
                     if self.start1:
                         self.start1 = False
                         self.sw.image = self.sw.i1
                     else:
                         self.start1 = True
                         self.sw.image = self.sw.i
-                if self.music.k_r.collidepoint(event.pos):
-                    if self.music.image == self.music.k:
-                        self.music.image = self.music.k1
-                        pg.mixer.music.pause()
-                    elif self.music.image == self.music.k1:
-                        self.music.image = self.music.k
-                        pg.mixer.music.play(-1)
                 if self.help.l_r.collidepoint(event.pos):
                     self.help1 = True
                 if self.help.l2_r.collidepoint(event.pos):
                     self.help1 = False
     def update_screen(self):
         self.sc.blit(self.a,self.a.get_rect())
         self.sc.blit(self.b,self.br)
@@ -508,15 +488,14 @@
         if self.win:
             font = pg.font.Font("C:\\Windows\\Fonts\\STXINGKA.TTF",30)
             win = font.render("胜利！",True,(255,255,250))
             w_r = win.get_rect()
             w_r.y,w_r.x = 300,350
             self.sc.blit(win,w_r)
         self.sw.d_i()
-        self.music.d_k()
         self.s_b.s_h_s()
         self.s_b.s_s_i()
         self.s_b.s_l_i()
         self.s_b.s_li_i()
         self.li.c_d()
         if self.s_s1:
             self.sh.d_g()
```

### Comparing `ftdz_from_fyh1-1.0.1/setup.py` & `ftdz_from_fyh1-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
     name='ftdz_from_fyh1',
-    version='1.0.1',
+    version='1.0.2',
     author='bob',
     author_email='56141537@qq.com',
     description='A game.',
     long_description_content_type="""text/markdown""",
     url='https://www.github.com/',
     packages=['ftdz_from_fyh1'],
     install_requires=['pygame','requests'],
```

