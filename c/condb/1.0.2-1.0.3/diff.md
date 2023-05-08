# Comparing `tmp/condb-1.0.2.tar.gz` & `tmp/condb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condb-1.0.2.tar", last modified: Tue Mar 21 13:35:15 2023, max compression
+gzip compressed data, was "condb-1.0.3.tar", last modified: Mon May  8 15:00:29 2023, max compression
```

## Comparing `condb-1.0.2.tar` & `condb-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-03-21 13:35:15.482361 condb-1.0.2/
--rw-r--r--   0 ivm        (501) staff       (20)     1504 2023-03-08 13:41:18.000000 condb-1.0.2/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      262 2023-03-21 13:35:15.482157 condb-1.0.2/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       26 2023-03-08 13:41:18.000000 condb-1.0.2/README.md
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-03-21 13:35:15.478762 condb-1.0.2/condb/
--rw-r--r--   0 ivm        (501) staff       (20)    22388 2023-03-21 12:30:31.000000 condb-1.0.2/condb/ConDB.py
--rw-r--r--   0 ivm        (501) staff       (20)      234 2023-03-19 12:07:51.000000 condb-1.0.2/condb/__init__.py
--rw-r--r--   0 ivm        (501) staff       (20)     6466 2023-03-21 13:25:53.000000 condb-1.0.2/condb/client.py
--rw-r--r--   0 ivm        (501) staff       (20)        0 2023-03-17 15:33:18.000000 condb-1.0.2/condb/csv.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    11948 2023-02-24 00:02:33.000000 condb-1.0.2/condb/dbdig.py
--rw-r--r--   0 ivm        (501) staff       (20)     8929 2023-03-21 13:17:52.000000 condb-1.0.2/condb/http_client.py
--rw-r--r--   0 ivm        (501) staff       (20)      175 2023-03-08 14:50:05.000000 condb-1.0.2/condb/py3.py
--rw-r--r--   0 ivm        (501) staff       (20)      285 2023-03-08 14:50:38.000000 condb-1.0.2/condb/signature.py
--rw-r--r--   0 ivm        (501) staff       (20)     2686 2023-03-09 13:05:40.000000 condb-1.0.2/condb/timelib.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-03-21 13:35:15.480820 condb-1.0.2/condb/ui/
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-03-21 13:35:15.481628 condb-1.0.2/condb/ui/cli/
--rw-r--r--   0 ivm        (501) staff       (20)      100 2022-07-15 16:28:10.000000 condb-1.0.2/condb/ui/cli/__init__.py
--rw-r--r--   0 ivm        (501) staff       (20)    10074 2023-01-03 20:31:34.000000 condb-1.0.2/condb/ui/cli/cli.py
--rw-r--r--   0 ivm        (501) staff       (20)    11437 2023-03-20 11:43:05.000000 condb-1.0.2/condb/ui/condb_ui.py
--rw-r--r--   0 ivm        (501) staff       (20)       64 2023-03-21 13:34:57.000000 condb-1.0.2/condb/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-03-21 13:35:15.480596 condb-1.0.2/condb.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      262 2023-03-21 13:35:14.000000 condb-1.0.2/condb.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      460 2023-03-21 13:35:15.000000 condb-1.0.2/condb.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-03-21 13:35:14.000000 condb-1.0.2/condb.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)       49 2023-03-21 13:35:15.000000 condb-1.0.2/condb.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-03-21 13:35:14.000000 condb-1.0.2/condb.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)        9 2023-03-21 13:35:15.000000 condb-1.0.2/condb.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)        6 2023-03-21 13:35:15.000000 condb-1.0.2/condb.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-03-21 13:35:15.482425 condb-1.0.2/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1006 2023-03-20 13:22:52.000000 condb-1.0.2/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-08 15:00:29.053346 condb-1.0.3/
+-rw-r--r--   0 ivm        (501) staff       (20)     1504 2023-03-08 13:41:18.000000 condb-1.0.3/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      234 2023-05-08 15:00:29.053089 condb-1.0.3/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       26 2023-03-08 13:41:18.000000 condb-1.0.3/README.md
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-08 15:00:29.049029 condb-1.0.3/condb/
+-rw-r--r--   0 ivm        (501) staff       (20)    22545 2023-05-08 14:43:58.000000 condb-1.0.3/condb/ConDB.py
+-rw-r--r--   0 ivm        (501) staff       (20)      234 2023-03-19 12:07:51.000000 condb-1.0.3/condb/__init__.py
+-rw-r--r--   0 ivm        (501) staff       (20)     6466 2023-03-21 13:25:53.000000 condb-1.0.3/condb/client.py
+-rw-r--r--   0 ivm        (501) staff       (20)        0 2023-03-17 15:33:18.000000 condb-1.0.3/condb/csv.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    11760 2023-05-08 14:59:17.000000 condb-1.0.3/condb/dbdig.py
+-rw-r--r--   0 ivm        (501) staff       (20)     8929 2023-03-21 13:17:52.000000 condb-1.0.3/condb/http_client.py
+-rw-r--r--   0 ivm        (501) staff       (20)      175 2023-03-08 14:50:05.000000 condb-1.0.3/condb/py3.py
+-rw-r--r--   0 ivm        (501) staff       (20)      285 2023-03-08 14:50:38.000000 condb-1.0.3/condb/signature.py
+-rw-r--r--   0 ivm        (501) staff       (20)     2686 2023-03-09 13:05:40.000000 condb-1.0.3/condb/timelib.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-08 15:00:29.050935 condb-1.0.3/condb/ui/
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-08 15:00:29.052365 condb-1.0.3/condb/ui/cli/
+-rw-r--r--   0 ivm        (501) staff       (20)      100 2022-07-15 16:28:10.000000 condb-1.0.3/condb/ui/cli/__init__.py
+-rw-r--r--   0 ivm        (501) staff       (20)    10074 2023-01-03 20:31:34.000000 condb-1.0.3/condb/ui/cli/cli.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11437 2023-03-20 11:43:05.000000 condb-1.0.3/condb/ui/condb_ui.py
+-rw-r--r--   0 ivm        (501) staff       (20)       64 2023-05-08 15:00:07.000000 condb-1.0.3/condb/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-05-08 15:00:29.050715 condb-1.0.3/condb.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      234 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      460 2023-05-08 15:00:29.000000 condb-1.0.3/condb.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       49 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)        9 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        6 2023-05-08 15:00:28.000000 condb-1.0.3/condb.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-05-08 15:00:29.053407 condb-1.0.3/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1006 2023-03-20 13:22:52.000000 condb-1.0.3/setup.py
```

### Comparing `condb-1.0.2/LICENSE` & `condb-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/condb/ConDB.py` & `condb-1.0.3/condb/ConDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         ----------
         connection:
             Psycopg2 connection object
         connstr : str
             Postgres connection string, e.g. "host=... port=... dbname=...". 
             Ignored if ``connection`` is provided
         """
+        if isinstance(connection, str):
+            connstr = connection
+            connection = None
         self.Conn = connection
         self.ConnStr = connstr
         
     def connect(self):
         if self.Conn == None:
             import psycopg2
             self.Conn = psycopg2.connect(self.ConnStr)
@@ -184,15 +187,17 @@
         self.DataColumns = [name for name, _ in self.DataColumnsTypes]
         self.AllColumns = self.StructureColumns + self.DataColumns
         if not self.validate():
             raise ValueError("Not a conditions DB table (verification failed)")
 
     @staticmethod
     def open(db, full_name):
-        dig = DbDig(db.connect())
+        dbcon = db.connect()
+        dig = DbDig(dbcon)
+        #print("dbcon:", dbcon)
         name = full_name
         ns = 'public'
         words = full_name.split('.')
         if len(words) > 1:
             ns = words[0]
             name = words[1]
         try:
```

### Comparing `condb-1.0.2/condb/client.py` & `condb-1.0.3/condb/client.py`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/condb/dbdig.py` & `condb-1.0.3/condb/dbdig.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,32 +34,21 @@
     
 class DbDigPostgres(DbDigImpl):
 
     def __init__(self, conn):
         """
         """
         self.Conn = conn
-        self.Dsn = {}
-        dsn = self.Conn.dsn
-        dsn = dsn.split(' ')
-        for v in dsn:
-            v = v.split('=')
-            if v[0] == 'password':
-                continue
-            self.Dsn[v[0]] = v[1]
-
-    def dsn(self):
-        return self.Dsn
 
     def dbases(self):
         """
         Find all databases
         """
         c = self.Conn.cursor()
-        sql = """select datname from %s""" % ('pg_database',)
+        sql = """select datname from pg_database"""
 
         c.execute(sql)
         dd = c.fetchall()
         c.close()
         if dd:
             return [d[0] for d in dd]
         else:
@@ -83,15 +72,21 @@
 
 
     def tables(self, nspace):
         """
         Find all tables
         """
         c = self.Conn.cursor()
-        sql = """select relname from pg_class where relnamespace=(select OID from pg_namespace where nspname=%s) and relkind='r'"""
+        sql = """select c.relname 
+                    from pg_class c, pg_namespace n
+                    where c.relnamespace = n.OID
+                        and n.nspname = %s
+                        and c.relkind='r'
+        """
+        #            (select OID from pg_namespace where nspname=%s) and relkind='r'""" 
 
         c.execute(sql, (nspace,))
         dd = c.fetchall()
         c.close()
         if dd:
             return [d[0] for d in dd]
         else:
@@ -106,57 +101,55 @@
         sql = """SELECT a.attname as "Column",
           pg_catalog.format_type(a.atttypid, a.atttypmod) as "Type",
           (SELECT substring(pg_catalog.pg_get_expr(d.adbin, d.adrelid) for 128)
            FROM pg_catalog.pg_attrdef d
            WHERE d.adrelid = a.attrelid AND d.adnum = a.attnum AND a.atthasdef) as "Modifiers",
           a.attnotnull as "Not NULL", pg_catalog.col_description(a.attrelid, a.attnum) as "Description"
         FROM pg_catalog.pg_attribute a
-        WHERE a.attrelid = (select OID from pg_catalog.pg_class where relnamespace=(select OID from pg_namespace where nspname='%s') and relname='%s')
+        WHERE a.attrelid = (select OID from pg_catalog.pg_class where relnamespace=(select OID from pg_namespace where nspname=%s) and relname=%s)
           AND a.attnum > 0 AND NOT a.attisdropped
         ORDER BY a.attnum;
-        """ % (nspace, table, )
+        """
 
-        c.execute(sql)
+        c.execute(sql, (nspace, table))
         dd = c.fetchall()
         c.close()
         if dd:
             return dd
-###            return pp(c, dd)
         else:
             return []
 
 
     def indexes(self, nspace, table):
         """
         Find indexes
         """
         nspace, table = self.getTableNameSpace(nspace, table)
         c = self.Conn.cursor()
-        sql = """SELECT indexname,indexdef FROM pg_indexes WHERE schemaname='%s' AND tablename = '%s'
-             """ % (nspace, table, )
+        sql = "SELECT indexname,indexdef FROM pg_indexes WHERE schemaname=%s AND tablename = %s" 
 
-        c.execute(sql)
+        c.execute(sql, (nspace, table))
         dd = c.fetchall()
         c.close()
         if dd:
             return dd
         else:
             return []
 
 
     def pKey(self, nspace, table):
         """
         Find primary keys
         """
         nspace, table = self.getTableNameSpace(nspace, table)
         c = self.Conn.cursor()
-        sql = """SELECT constraint_name FROM information_schema.table_constraints WHERE table_schema='%s' AND table_name='%s' AND constraint_type='PRIMARY KEY'
-             """ % (nspace, table, )
+        sql = """SELECT constraint_name FROM information_schema.table_constraints WHERE table_schema=%s AND table_name=%s AND constraint_type='PRIMARY KEY'
+             """
 
-        c.execute(sql)
+        c.execute(sql, (nspace, table))
         dd = c.fetchall()
         c.close()
         if dd:
             #return dd
              return self.keyDef(nspace, dd[0][0])[-1]    # Return only column list
         else:
             return None
@@ -164,18 +157,18 @@
 
     def fKeys(self, nspace, table):
         """
         Find foreign keys
         """
         nspace, table = self.getTableNameSpace(nspace, table)
         c = self.Conn.cursor()
-        sql = """SELECT constraint_name FROM information_schema.table_constraints WHERE table_schema='%s' AND table_name='%s' AND constraint_type='FOREIGN KEY'
-             """ % (nspace, table, )
+        sql = """SELECT constraint_name FROM information_schema.table_constraints WHERE table_schema=%s AND table_name=%s AND constraint_type='FOREIGN KEY'
+             """
 
-        c.execute(sql)
+        c.execute(sql, (nspace, table))
         dd = c.fetchall()
         c.close()
         if dd:
             #return dd
             reply = []
             for kn in dd:
                 #reply.append(self.keyDef(nspace, kn[0])[2:])   # return only the first pair - (table_name, column_list) for the specified table itself
@@ -189,19 +182,19 @@
     def referringKeys(self, nspace, table):
         """
         Find all keys
         """
         nspace, table = self.getTableNameSpace(nspace, table)
         c = self.Conn.cursor()
         sql = """SELECT constraint_name FROM information_schema.table_constraints WHERE
-                 table_schema='%s' AND constraint_type='FOREIGN KEY' AND constraint_name IN 
-                (SELECT constraint_name  FROM information_schema.constraint_table_usage WHERE table_schema='%s' AND table_name='%s') ORDER BY table_name
-              """ % (nspace, nspace, table, )
+                 table_schema=%s AND constraint_type='FOREIGN KEY' AND constraint_name IN 
+                (SELECT constraint_name  FROM information_schema.constraint_table_usage WHERE table_schema=%s AND table_name=%s) ORDER BY table_name
+              """
 
-        c.execute(sql)
+        c.execute(sql, (nspace, nspace, table))
         dd = c.fetchall()
         c.close()
         if dd:
             #return dd
             reply = []
             for kn in dd:
                 #reply.append(self.keyDef(nspace, kn[0])[:2])   # Return only the second pair - (table_name, column_list) for the referred table
@@ -214,44 +207,44 @@
     def keyDef(self, nspace, kname):
         """ 
         Find key details
         """
         # Referring table
         c = self.Conn.cursor()
         sql = """SELECT table_name, column_name FROM information_schema.key_column_usage
-                WHERE table_schema='%s' AND constraint_name='%s'
-              """ % (nspace, kname, )
-        c.execute(sql)
+                WHERE table_schema=%s AND constraint_name=%s
+              """
+        c.execute(sql, (nspace, kname))
         rr = c.fetchall()
         if rr:
           rtname = rr[0][0]
           rcname = tuple([v[1] for v in rr])
         else:
             return None
         # Referred table
         #sql = """SELECT table_name, column_name FROM information_schema.constraint_column_usage
         #        WHERE table_schema='%s' AND constraint_name='%s'
         #      """ % (nspace, kname, )
-        sql =   """select table_name, column_name from
+        sql = """select table_name, column_name from
                         (SELECT nr.nspname, r.relname, a.attname, c.conname
                           FROM pg_namespace nr, pg_class r, pg_attribute a,
                                 pg_namespace nc, pg_constraint c
                                          WHERE nr.oid = r.relnamespace AND r.oid = a.attrelid AND
                                 nc.oid = c.connamespace AND
                                                CASE
                                                    WHEN c.contype = 'f'::"char" THEN r.oid =
                                 c.confrelid AND (a.attnum = ANY (c.confkey))
                                                    ELSE r.oid = c.conrelid AND (a.attnum = ANY (c.conkey))
                                                END AND NOT a.attisdropped AND (c.contype = ANY
                                 (ARRAY['p'::"char", 'u'::"char", 'f'::"char"])) AND r.relkind =
                                 'r'::"char") 
                         as x(namespace, table_name, column_name, constraint_name)
-                where namespace='%s' and constraint_name='%s'""" % (nspace, kname,)
+                where namespace=%s and constraint_name=%s""" 
 
-        c.execute(sql)
+        c.execute(sql, (nspace, kname))
         pp = c.fetchall()
         if pp:
           ptname = pp[0][0]
           pcname = tuple([v[1] for v in pp])
         else:
             return None
```

### Comparing `condb-1.0.2/condb/http_client.py` & `condb-1.0.3/condb/http_client.py`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/condb/timelib.py` & `condb-1.0.3/condb/timelib.py`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/condb/ui/cli/cli.py` & `condb-1.0.3/condb/ui/cli/cli.py`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/condb/ui/condb_ui.py` & `condb-1.0.3/condb/ui/condb_ui.py`

 * *Files identical despite different names*

### Comparing `condb-1.0.2/setup.py` & `condb-1.0.3/setup.py`

 * *Files identical despite different names*

