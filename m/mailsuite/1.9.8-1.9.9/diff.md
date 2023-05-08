# Comparing `tmp/mailsuite-1.9.8.tar.gz` & `tmp/mailsuite-1.9.9.tar.gz`

## Comparing `mailsuite-1.9.8.tar` & `mailsuite-1.9.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mailsuite-1.9.8/mailsuite/__init__.py
--rw-r--r--   0        0        0    16106 2020-02-02 00:00:00.000000 mailsuite-1.9.8/mailsuite/imap.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 mailsuite-1.9.8/mailsuite/smtp.py
--rw-r--r--   0        0        0    26390 2020-02-02 00:00:00.000000 mailsuite-1.9.8/mailsuite/utils.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mailsuite-1.9.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mailsuite-1.9.8/LICENSE
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 mailsuite-1.9.8/README.md
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 mailsuite-1.9.8/pyproject.toml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 mailsuite-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mailsuite-1.9.9/mailsuite/__init__.py
+-rw-r--r--   0        0        0    16106 2020-02-02 00:00:00.000000 mailsuite-1.9.9/mailsuite/imap.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 mailsuite-1.9.9/mailsuite/smtp.py
+-rw-r--r--   0        0        0    26441 2020-02-02 00:00:00.000000 mailsuite-1.9.9/mailsuite/utils.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mailsuite-1.9.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mailsuite-1.9.9/LICENSE
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 mailsuite-1.9.9/README.md
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 mailsuite-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 mailsuite-1.9.9/PKG-INFO
```

### Comparing `mailsuite-1.9.8/mailsuite/imap.py` & `mailsuite-1.9.9/mailsuite/imap.py`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/mailsuite/smtp.py` & `mailsuite-1.9.9/mailsuite/smtp.py`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/mailsuite/utils.py` & `mailsuite-1.9.9/mailsuite/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,17 +318,17 @@
         if is_outlook_msg(data):
             data = convert_outlook_msg(data)
         data = data.decode("utf-8", errors="replace")
     _parsed_email = mailparser.parse_from_string(data)
     parsed_email = _parsed_email.mail
     if isinstance(parsed_email, str):
         raise ValueError("Not an email")
-    headers_str = data.split("\n\n")[0]
+    headers_str = re.split(r"(\n|\r\n){2,}", data)[0]
     parsed_email["raw_headers"] = headers_str
-    headers_str = re.sub(r"\n\s+", " ", headers_str)
+    headers_str = re.sub(r"(\n|\r\n)\s+", " ", headers_str)
     if "subject" in parsed_email:
         headers_str = re.sub(r"Subject: .+",
                              f"Subject: {parsed_email['subject']}",
                              headers_str)
 
     if "thread-topic" in parsed_email:
         headers_str = re.sub(r"Thread-Topic: .+",
@@ -525,15 +525,15 @@
                 message = email_file.read()
     if isinstance(message, dict):
         parsed_email = message
     else:
         parsed_email = parse_email(message)
 
     if isinstance(trusted_domains, str):
-        trusted_domains.split("\n")
+        trusted_domains = re.split(r"(\n|\r\n)", trusted_domains)
 
     for i in range(len(trusted_domains)):
         trusted_domains[i] = trusted_domains[i].lower().strip()
     trusted_domains = set(trusted_domains)
     if "" in trusted_domains:
         trusted_domains.remove("")
     trusted_domains = list(trusted_domains)
```

### Comparing `mailsuite-1.9.8/.gitignore` & `mailsuite-1.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/LICENSE` & `mailsuite-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/README.md` & `mailsuite-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/pyproject.toml` & `mailsuite-1.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mailsuite-1.9.8/PKG-INFO` & `mailsuite-1.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailsuite
-Version: 1.9.8
+Version: 1.9.9
 Summary: A Python package for retrieving, parsing, and sending emails
 Project-URL: Homepage, https://github.com/seanthegeek/mailsuite/
 Project-URL: Documentation, https://seanthegeek.github.io/mailsuite/
 Project-URL: Issues, https://github.com/seanthegeek/mailsuite/issues
 Project-URL: Changelog, https://github.com/seanthegeek/mailsuite/blob/master/CHANGELOG.md
 Author-email: Sean Whalen <whalenster@gmail.com>
 License-File: LICENSE
```

