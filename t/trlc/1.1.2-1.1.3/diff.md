# Comparing `tmp/trlc-1.1.2.tar.gz` & `tmp/trlc-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trlc-1.1.2.tar", last modified: Thu May  4 13:51:37 2023, max compression
+gzip compressed data, was "trlc-1.1.3.tar", last modified: Mon May  8 15:02:55 2023, max compression
```

## Comparing `trlc-1.1.2.tar` & `trlc-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.2/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-04 13:51:37.084142 trlc-1.1.2/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.2/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-04 13:51:37.084142 trlc-1.1.2/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.2/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.2/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    96418 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7240 2023-04-12 08:39:07.000000 trlc-1.1.2/trlc/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)    15521 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.2/trlc/lint.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.2/trlc/math.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.2/trlc/nested.py
--rw-r--r--   0 florian   (1000) florian   (1000)    58761 2023-05-04 13:51:21.000000 trlc-1.1.2/trlc/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.2/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-05-04 13:51:32.000000 trlc-1.1.2/trlc/version.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-04 13:51:37.084142 trlc-1.1.2/trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-05-04 13:51:37.000000 trlc-1.1.2/trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:02:55.856355 trlc-1.1.3/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2022-12-05 12:42:52.000000 trlc-1.1.3/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-08 15:02:55.856355 trlc-1.1.3/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.1.3/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-05-08 15:02:55.856355 trlc-1.1.3/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.1.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:02:55.852355 trlc-1.1.3/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.1.3/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    96878 2023-05-08 15:02:21.000000 trlc-1.1.3/trlc/ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7240 2023-04-12 08:39:07.000000 trlc-1.1.3/trlc/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    15521 2023-05-04 13:51:21.000000 trlc-1.1.3/trlc/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2475 2023-04-28 09:15:42.000000 trlc-1.1.3/trlc/lint.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1266 2023-03-23 13:32:34.000000 trlc-1.1.3/trlc/math.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3351 2023-03-23 13:32:34.000000 trlc-1.1.3/trlc/nested.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    58800 2023-05-08 15:02:21.000000 trlc-1.1.3/trlc/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16319 2023-04-28 09:15:42.000000 trlc-1.1.3/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-05-08 15:02:51.000000 trlc-1.1.3/trlc/version.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-08 15:02:55.856355 trlc-1.1.3/trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2965 2023-05-08 15:02:55.000000 trlc-1.1.3/trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      322 2023-05-08 15:02:55.000000 trlc-1.1.3/trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-08 15:02:55.000000 trlc-1.1.3/trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       40 2023-05-08 15:02:55.000000 trlc-1.1.3/trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-05-08 15:02:55.000000 trlc-1.1.3/trlc.egg-info/top_level.txt
```

### Comparing `trlc-1.1.2/LICENSE` & `trlc-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/PKG-INFO` & `trlc-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.2
+Version: 1.1.3
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
```

### Comparing `trlc-1.1.2/README.md` & `trlc-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/setup.py` & `trlc-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/__init__.py` & `trlc-1.1.3/trlc/__init__.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/ast.py` & `trlc-1.1.3/trlc/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,15 +859,15 @@
         elif not self.target.n_typ.is_subclass_of(self.typ):
             mh.ice_loc(self.location,
                        "on resolving references, types do not match; "
                        "expected %s, got %s" % (self.typ.name,
                                                 self.target.n_typ.name))
 
     def to_python_object(self):
-        return self.name
+        return self.target.fully_qualified_name()
 
 
 class Name_Reference(Expression):
     """Reference to a name
 
     Name reference to either a :class:`Composite_Component` or a
     :class:`Quantified_Variable`. The actual value of course depends
@@ -1999,15 +1999,15 @@
         assert isinstance(builtin_stab, Symbol_Table)
         self.symbols = Symbol_Table()
         self.symbols.make_visible(builtin_stab)
         self.declared_late = False
 
     def dump(self, indent=0):  # pragma: no cover
         self.write_indent(indent, "Package %s" % self.name)
-        self.symbols.dump(indent + 1)
+        self.symbols.dump(indent + 1, omit_heading=True)
 
 
 class Composite_Type(Concrete_Type):
     """Abstract base for record and tuple types, as they share some
        functionality.
 
     :attribute components: type components (including inherited if applicable)
@@ -2391,32 +2391,45 @@
 
     :attribute field: the specific values for all components (see 3 and 4)
     :type: dict[str, Expression]
 
     :attribute section: None or the section this record is contained in (see 5)
     :type: Section
 
+    :attribute n_package: The package in which this record is declared in
+    :type: Section
+
     The actual type of expressions in the field attribute are limited
     to:
 
     * :class:`Literal`
     * :class:`Unary_Expression`
     * :class:`Array_Aggregate`
     * :class:`Tuple_Aggregate`
     * :class:`Record_Reference`
     * :class:`Implicit_Null`
 
     """
-    def __init__(self, name, location, n_typ, section):
+    def __init__(self, name, location, n_typ, section, n_package):
         assert isinstance(n_typ, Record_Type)
         assert isinstance(section, Section) or section is None
+        assert isinstance(n_package, Package)
         super().__init__(name, location, n_typ)
-        self.field   = {name: None
-                        for name in self.n_typ.components.all_names()}
-        self.section = section
+        self.field     = {name: None
+                          for name in self.n_typ.components.all_names()}
+        self.section   = section
+        self.n_package = n_package
+
+    def fully_qualified_name(self):
+        """Return the FQN for this type (i.e. PACKAGE.NAME)
+
+        :returns: the object's full name
+        :rtype: str
+        """
+        return self.n_package.name + "." + self.name
 
     def to_python_dict(self):
         """Return an evaluated and simplified object for Python.
 
         For example it might provide::
 
           {"foo" : [1, 2, 3],
```

### Comparing `trlc-1.1.2/trlc/errors.py` & `trlc-1.1.3/trlc/errors.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/lexer.py` & `trlc-1.1.3/trlc/lexer.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/lint.py` & `trlc-1.1.3/trlc/lint.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/math.py` & `trlc-1.1.3/trlc/math.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/nested.py` & `trlc-1.1.3/trlc/nested.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/parser.py` & `trlc-1.1.3/trlc/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1408,19 +1408,21 @@
         if r_typ.is_abstract:
             self.mh.error(self.ct.location,
                           "cannot declare object of abstract record type %s" %
                           r_typ.name)
 
         self.match("IDENTIFIER")
         obj = ast.Record_Object(
-            name     = self.ct.value,
-            location = self.ct.location,
-            n_typ    = r_typ,
-            section  = self.section[-1] if self.section else None)
+            name      = self.ct.value,
+            location  = self.ct.location,
+            n_typ     = r_typ,
+            section   = self.section[-1] if self.section else None,
+            n_package = self.pkg)
         self.pkg.symbols.register(self.mh, obj)
+
         self.match("C_BRA")
         while not self.peek("C_KET"):
             self.match("IDENTIFIER")
             comp = r_typ.components.lookup(self.mh,
                                            self.ct,
                                            ast.Composite_Component)
             if r_typ.is_frozen(comp):
```

### Comparing `trlc-1.1.2/trlc/trlc.py` & `trlc-1.1.3/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `trlc-1.1.2/trlc/version.py` & `trlc-1.1.3/trlc/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (1, 1, 2)
+VERSION_TUPLE = (1, 1, 3)
 VERSION_SUFFIX = ""
 
 TRLC_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "TRLC %s" % TRLC_VERSION
```

### Comparing `trlc-1.1.2/trlc.egg-info/PKG-INFO` & `trlc-1.1.3/trlc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.1.2
+Version: 1.1.3
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
```

