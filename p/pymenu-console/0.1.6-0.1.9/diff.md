# Comparing `tmp/pymenu-console-0.1.6.tar.gz` & `tmp/pymenu-console-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymenu-console-0.1.6.tar", last modified: Sun Jan 15 15:49:34 2023, max compression
+gzip compressed data, was "dist\pymenu-console-0.1.9.tar", last modified: Mon May  8 17:06:11 2023, max compression
```

## Comparing `pymenu-console-0.1.6.tar` & `pymenu-console-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/
--rw-rw-rw-   0        0        0      539 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-01-14 17:14:51.000000 pymenu-console-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu/
--rw-rw-rw-   0        0        0       56 2023-01-14 18:16:57.000000 pymenu-console-0.1.6/pymenu/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-01-15 15:48:48.000000 pymenu-console-0.1.6/pymenu/auto_menu.py
--rw-rw-rw-   0        0        0     3026 2023-01-15 15:32:27.000000 pymenu-console-0.1.6/pymenu/menu.py
--rw-rw-rw-   0        0        0      267 2023-01-14 17:14:51.000000 pymenu-console-0.1.6/pymenu/option.py
--rw-rw-rw-   0        0        0      546 2023-01-14 19:35:27.000000 pymenu-console-0.1.6/pymenu/select_menu.py
-drwxrwxrwx   0        0        0        0 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu/utils/
--rw-rw-rw-   0        0        0        0 2023-01-14 18:08:47.000000 pymenu-console-0.1.6/pymenu/utils/__init__.py
--rw-rw-rw-   0        0        0      572 2023-01-15 15:38:24.000000 pymenu-console-0.1.6/pymenu/utils/inputs.py
-drwxrwxrwx   0        0        0        0 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/
--rw-rw-rw-   0        0        0      539 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/pymenu_console.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-15 15:49:34.000000 pymenu-console-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-01-15 15:49:26.000000 pymenu-console-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/
+-rw-rw-rw-   0        0        0     3143 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2092 2023-05-08 16:59:45.000000 pymenu-console-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu/
+-rw-rw-rw-   0        0        0       56 2023-05-08 16:50:02.000000 pymenu-console-0.1.9/pymenu/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-05-08 17:04:44.000000 pymenu-console-0.1.9/pymenu/auto_menu.py
+-rw-rw-rw-   0        0        0     3282 2023-05-08 16:59:56.000000 pymenu-console-0.1.9/pymenu/menu.py
+-rw-rw-rw-   0        0        0      267 2023-05-08 16:50:02.000000 pymenu-console-0.1.9/pymenu/option.py
+-rw-rw-rw-   0        0        0      580 2023-05-08 17:02:22.000000 pymenu-console-0.1.9/pymenu/select_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-08 16:50:02.000000 pymenu-console-0.1.9/pymenu/utils/__init__.py
+-rw-rw-rw-   0        0        0      572 2023-05-08 16:50:02.000000 pymenu-console-0.1.9/pymenu/utils/inputs.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/
+-rw-rw-rw-   0        0        0     3143 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/pymenu_console.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:06:11.000000 pymenu-console-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-05-08 17:06:04.000000 pymenu-console-0.1.9/setup.py
```

### Comparing `pymenu-console-0.1.6/pymenu/auto_menu.py` & `pymenu-console-0.1.9/pymenu/auto_menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     return module_name
 
 
 def run_python_module(module_name: str):
     os.system(f'python -m {module_name}')
 
 
-def create_menu_from_directory(path: str, prefix: str = None) -> Menu:
+def create_menu_from_directory(path: str, prefix: str = None, *args, **kwargs) -> Menu:
     title = get_directory_name(path)
     title = prefix + title if prefix else title
-    menu = Menu(title)
+    menu = Menu(title, *args, **kwargs)
 
     def file_callback(path: str, file: str):
         python_module = python_filename_to_module_name(os.path.join(path, file))
         return lambda: run_python_module(python_module)
 
     for file in get_all_files_from_directory(path):
         menu.add_option(file, file_callback(path, file))
 
     for folder in get_all_folders_from_directory(path):
-        menu.add_option(folder, create_menu_from_directory(os.path.join(path, folder), f'{title} > '))
+        menu.add_option(folder, create_menu_from_directory(os.path.join(path, folder), f'{title} > ', *args, **kwargs))
 
     return menu
```

### Comparing `pymenu-console-0.1.6/pymenu/menu.py` & `pymenu-console-0.1.9/pymenu/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,24 @@
         self,
         title: str,
         options: List[Option] = None,
         title_color: str = 'blue',
         selected_color: str = 'cyan',
         back_name: str = '<-',
         prefix: str = '%s) ',
+        enable_keyboard_selection: bool = True,
     ) -> None:
         self.title = title
         self.title_color = title_color
         self.selected_color = selected_color
         self.options = options or []
         self.__selected_index: int = 0
         self.back_name = back_name
         self.prefix = prefix
+        self.enable_keyboard_selection = enable_keyboard_selection
 
     def open_submenu(self, submenu: Menu):
         self.clear()
         if submenu.options[-1].name != self.back_name:
             submenu.add_option(self.back_name, lambda: self.return_to_this_menu(submenu))
         submenu.show()
 
@@ -47,32 +49,34 @@
 
     def add_options(self, options: List[Tuple[str, Union[Callable, Menu]]]):
         for option in options:
             self.add_option(*option)
 
     def show(self):
         self.__update()
-        keyboard.add_hotkey('up', self.up)
-        keyboard.add_hotkey('down', self.down)
+        if self.enable_keyboard_selection:
+            keyboard.add_hotkey('up', self.up)
+            keyboard.add_hotkey('down', self.down)
         self.wait_for_command()
         self.run_selected()
 
     def remove_keyboard_listener(self):
-        keyboard.remove_hotkey('up')
-        keyboard.remove_hotkey('down')
+        if self.enable_keyboard_selection:
+            keyboard.remove_hotkey('up')
+            keyboard.remove_hotkey('down')
 
     def clear(self):
         os.system('cls' if os.name == 'nt' else 'clear')
 
     def __update(self):
         self.clear()
         print(colored(self.title, self.title_color), '\n')
         for i, script in enumerate(self.options):
             prefix = self.prefix % (i + 1)
-            if i == self.__selected_index:
+            if self.enable_keyboard_selection and i == self.__selected_index:
                 print(colored(f'{prefix}{script}', self.selected_color))
             else:
                 print(f'{prefix}{script}')
 
     def up(self):
         if self.__selected_index > 0:
             self.__selected_index -= 1
```

### Comparing `pymenu-console-0.1.6/pymenu/select_menu.py` & `pymenu-console-0.1.9/pymenu/select_menu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, TypeVar
 
 from pymenu import Menu
 
 T = TypeVar('T')
 
 
-def create_select_menu(options: List[T], title: str = 'Select an option') -> T:
+def create_select_menu(options: List[T], title: str = 'Select an option', *args, **kwargs) -> T:
     selected_option: T
 
     def select_option(option: T) -> None:
         nonlocal selected_option
         selected_option = option
 
-    menu = Menu(title)
+    menu = Menu(title, *args, **kwargs)
     for option in options:
         def callback(option: T):
             return lambda: select_option(option)
 
         menu.add_option(str(option), callback(option))
     menu.show()
```

### Comparing `pymenu-console-0.1.6/pymenu/utils/inputs.py` & `pymenu-console-0.1.9/pymenu/utils/inputs.py`

 * *Files identical despite different names*

### Comparing `pymenu-console-0.1.6/setup.py` & `pymenu-console-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymenu-console",
-    version="0.1.6",
+    version="0.1.9",
     author="luanws",
     author_email="luan.w.silveira@gmail.com",
     description="Python console menu",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luanws/pymenu",
     packages=setuptools.find_packages(),
```

