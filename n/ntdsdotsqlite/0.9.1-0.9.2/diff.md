# Comparing `tmp/ntdsdotsqlite-0.9.1.tar.gz` & `tmp/ntdsdotsqlite-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-0.9.1.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-0.9.2.tar", max compression
```

## Comparing `ntdsdotsqlite-0.9.1.tar` & `ntdsdotsqlite-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.1/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.1/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0     4778 2023-05-08 15:39:42.476407 ntdsdotsqlite-0.9.1/ntdsdotsqlite/accounts.py
--rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.1/ntdsdotsqlite/containers.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.1/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     3092 2023-05-08 09:44:04.537563 ntdsdotsqlite-0.9.1/ntdsdotsqlite/domain.py
--rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.1/ntdsdotsqlite/groups.py
--rw-r--r--   0        0        0      362 2023-05-08 14:14:48.766973 ntdsdotsqlite-0.9.1/ntdsdotsqlite/links.py
--rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.1/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     4630 2023-05-08 16:07:39.897658 ntdsdotsqlite-0.9.1/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.1/ntdsdotsqlite/orga_units.py
--rw-r--r--   0        0        0    27265 2023-05-08 16:14:52.647510 ntdsdotsqlite-0.9.1/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     5505 2023-05-08 09:42:49.642876 ntdsdotsqlite-0.9.1/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      695 2023-05-08 17:27:52.226908 ntdsdotsqlite-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.1/README.md
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.2/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.2/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0     4778 2023-05-08 15:39:42.476407 ntdsdotsqlite-0.9.2/ntdsdotsqlite/accounts.py
+-rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.2/ntdsdotsqlite/containers.py
+-rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.2/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.2/ntdsdotsqlite/domain.py
+-rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.2/ntdsdotsqlite/groups.py
+-rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.2/ntdsdotsqlite/links.py
+-rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.2/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     4630 2023-05-08 16:07:39.897658 ntdsdotsqlite-0.9.2/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.2/ntdsdotsqlite/orga_units.py
+-rw-r--r--   0        0        0    26997 2023-05-08 21:10:10.754799 ntdsdotsqlite-0.9.2/ntdsdotsqlite/secretsdump.py
+-rw-r--r--   0        0        0     5678 2023-05-08 21:13:24.935764 ntdsdotsqlite-0.9.2/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      695 2023-05-08 21:14:52.804604 ntdsdotsqlite-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.2/README.md
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.2/PKG-INFO
```

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/accounts.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/accounts.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/containers.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/containers.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/domain.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             domain_object = row
             # We only need the first object that represents the main domain
             break
     # go up in the tree to get the full domain name
     cur_object = domain_object
     parents = []
     while True:
-        # Si on est remonté au root object (guid '00'*16, name='$ROOT_OBJECT$\u0000'), on break
+        # If we got back to the root object (guid '00'*16, name='$ROOT_OBJECT$\u0000'), break
         parent_dnt = cur_object.get("PDNT_col")
         if parent_dnt == 2:
             break
         for row in datatable.records():
             if row.get("DNT_col") == parent_dnt:
                 parents.append(row)
                 cur_object = row
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/groups.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/groups.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/model.sql`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/orga_units.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/orga_units.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/secretsdump.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/secretsdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,24 +329,14 @@
         Crypt1 = DES.new(Key1, DES.MODE_ECB)
         Crypt2 = DES.new(Key2, DES.MODE_ECB)
 
         decryptedHash = Crypt1.decrypt(cryptedHash[:8]) + Crypt2.decrypt(cryptedHash[8:])
 
         return decryptedHash
 
-    @staticmethod
-    def __fileTimeToDateTime(t):
-        t -= 116444736000000000
-        t //= 10000000
-        if t < 0:
-            return 'never'
-        else:
-            dt = datetime.fromtimestamp(t)
-            return dt.strftime("%Y-%m-%d %H:%M")
-
     def __decryptSupplementalInfo(self, record):
         # This is based on [MS-SAMR] 2.2.10 Supplemental Credentials Structures
         haveInfo = False
         LOG.debug('Entering NTDSHashes.__decryptSupplementalInfo')
         if record[self.NAME_TO_INTERNAL['supplementalCredentials']] is not None:
             if len(unhexlify(record[self.NAME_TO_INTERNAL['supplementalCredentials']])) > 24:
                 cipherText = self.CRYPTED_BLOB(
```

### Comparing `ntdsdotsqlite-0.9.1/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-0.9.2/ntdsdotsqlite/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     p2 = raw[4:6][::-1].hex()
     p3 = raw[6:8][::-1].hex()
     p4 = raw[8:10].hex()
     p5 = raw[10:].hex()
     return f"{p1}-{p2}-{p3}-{p4}-{p5}"
 
 
+# Transforms raw bytes returned by dessect to a correct SID string
 def raw_to_sid(raw):
     rev = str(int(raw[0]))
     nb_dashes = int(raw[1])
     id_auth_value = int.from_bytes(raw[2:8], "big")
     subparts = []
     for i in range(nb_dashes):
         endianess = "big" if i == nb_dashes - 1 else "little"
         subparts.append(str(int.from_bytes(raw[8+(i*4):8+(i*4)+4], endianess)))
     return f"S-{rev}-{id_auth_value}-{'-'.join(subparts)}"
 
 
+# Translates microsoft duration/datetime format (intervals of 100ns) to python datetime object
 def hundredns_to_datetime(ns):
     return timedelta(seconds=ns / 10000000) + datetime(1601, 1, 1)
 
 
 # Function to get attribute names from the ESE database. Gets real column names
 # like "sAMAccountName" from attribute IDs like "ATTc131102". Way easier to work
 # with !
@@ -79,23 +81,16 @@
     script = open(Path(__file__).parent / "model.sql", "r").read()
     cursor = db.cursor()
     cursor.executescript(script)
     if db:
         db.close()
 
 
-def ESE_cursor_next(db, table):
-    cursor = db.openTable(table)
-    while (row := db.getNextRow(cursor)):
-        yield {
-            db.column_names[k].decode("utf-8") if k in db.column_names.keys() else k: v
-            for k, v in row.items() if v
-        }
-
-
+# Returns the object in the database representing a schema object of the chosen schema GUID.
+# Its main use is to get its DNT that will be used by all subsequent objects as an objectCategory.
 def get_schema_object(ese_db, schemaGuid):
     slices = [
         slice(0, 8), slice(9, 13), slice(14, 18), slice(19, 23),
         slice(24, 36)
     ]
     sguid = binascii.unhexlify(schemaGuid[slices[0]])[::-1].hex()
     sguid += binascii.unhexlify(schemaGuid[slices[1]])[::-1].hex()
@@ -133,17 +128,18 @@
     USE_DES_KEY_ONLY = 0x200000
     DONT_REQ_PREAUTH = 0x400000
     PASSWORD_EXPIRED = 0x800000
     TRUSTED_TO_AUTH_FOR_DELEGATION = 0x1000000
     PARTIAL_SECRETS_ACCOUNT = 0x04000000
 
 
+# Extracted from python-ldap/Lib/ldap/dn.py, in order to remove one dependency
+# that would need to be compiled otherwise.
 def escape_dn_chars(s):
     """
-    From python-ldap/Lib/ldap/dn.py
     Escape all DN special characters found in s
     with a back-slash (see RFC 4514, section 2.4)
     """
     if s:
         s = s.replace('\\', '\\\\')
         s = s.replace(',', '\\,')
         s = s.replace('+', '\\+')
```

### Comparing `ntdsdotsqlite-0.9.1/pyproject.toml` & `ntdsdotsqlite-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "0.9.1"
+version = "0.9.2"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-0.9.1/README.md` & `ntdsdotsqlite-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.1/PKG-INFO` & `ntdsdotsqlite-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 0.9.1
+Version: 0.9.2
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

