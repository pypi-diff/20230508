# Comparing `tmp/querytograph-0.0.2.tar.gz` & `tmp/querytograph-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querytograph-0.0.2.tar", last modified: Sun May  7 17:04:55 2023, max compression
+gzip compressed data, was "querytograph-0.0.3.tar", last modified: Mon May  8 16:02:58 2023, max compression
```

## Comparing `querytograph-0.0.2.tar` & `querytograph-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.155226 querytograph-0.0.2/
--rw-rw-r--   0 simk      (1000) simk      (1000)     2039 2023-05-07 17:04:55.155226 querytograph-0.0.2/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)     1734 2023-05-07 16:51:32.000000 querytograph-0.0.2/README.md
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.151226 querytograph-0.0.2/querytograph/
--rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.2/querytograph/__init__.py
--rw-rw-r--   0 simk      (1000) simk      (1000)     7212 2023-05-07 15:53:56.000000 querytograph-0.0.2/querytograph/querytograph.py
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.155226 querytograph-0.0.2/querytograph.egg-info/
--rw-rw-r--   0 simk      (1000) simk      (1000)     2039 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)      251 2023-05-07 17:04:55.000000 querytograph-0.0.2/querytograph.egg-info/SOURCES.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/dependency_links.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       71 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/requires.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-07 17:04:55.000000 querytograph-0.0.2/querytograph.egg-info/top_level.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-07 17:04:55.155226 querytograph-0.0.2/setup.cfg
--rw-rw-r--   0 simk      (1000) simk      (1000)     1015 2023-05-07 17:04:13.000000 querytograph-0.0.2/setup.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1065 2023-05-07 16:29:46.000000 querytograph-0.0.3/LICENSE
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2083 2023-05-08 16:02:58.813732 querytograph-0.0.3/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1808 2023-05-08 16:00:20.000000 querytograph-0.0.3/README.md
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/querytograph/
+-rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.3/querytograph/__init__.py
+-rw-rw-r--   0 simk      (1000) simk      (1000)     7686 2023-05-08 15:47:14.000000 querytograph-0.0.3/querytograph/querytograph.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/querytograph.egg-info/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2083 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)      259 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       71 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/requires.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/top_level.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-08 16:02:58.813732 querytograph-0.0.3/setup.cfg
+-rw-rw-r--   0 simk      (1000) simk      (1000)      963 2023-05-08 16:02:21.000000 querytograph-0.0.3/setup.py
```

### Comparing `querytograph-0.0.2/PKG-INFO` & `querytograph-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.2
+Version: 0.0.3
 Summary: Using ChatGPT to convert your plain English queries into graphs
-Home-page: https://github.com/franziss/querytograph
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # QueryToGraph
 QueryToGraph is a Python library that allows user to use simple English to create graph from a dataframe or csv file. It uses ChatGPT as the underlying engine. 
 
 **For security's sake, it does not send the raw data to ChatGPT** but only the data schema (i.e. the data field names) is sent.
 
 
@@ -52,14 +52,15 @@
 
 ![Chart](Screenshot.png)
 
 There are 3 textboxes which you have to key in  
 
 1. Query  
    Question by the user, which will be used to generate the graph
+   Example: "show me the highest and lowest closing price for each month"
 2. Data Folder  
    Folder which contains Pandas dataframes in csv or pkl (pickle)
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
```

### Comparing `querytograph-0.0.2/README.md` & `querytograph-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 ![Chart](Screenshot.png)
 
 There are 3 textboxes which you have to key in  
 
 1. Query  
    Question by the user, which will be used to generate the graph
+   Example: "show me the highest and lowest closing price for each month"
 2. Data Folder  
    Folder which contains Pandas dataframes in csv or pkl (pickle)
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
```

### Comparing `querytograph-0.0.2/querytograph/querytograph.py` & `querytograph-0.0.3/querytograph/querytograph.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,44 +63,49 @@
 
             Your previous generated code has the following error message {err_msg}
             Fix the errors/bugs and you must give me the right code this time!
             """
             prompt = PromptTemplate(
                 input_variables=["query", "columns", "err_msg"], template=_DEFAULT_TEMPLATE)    
 
-        print("--- PROMPT")
-        print(prompt)
+        print("--- Query")
+        print(query)
+        print("--- Err_msg")
+        print(err_msg)
         chain = LLMChain(llm=llm, prompt=prompt)
 
         valid_files = self.find_df(data_path, table_name)
 
         if len(valid_files) > 0:
             # sort and read the first file that has the most similar name
             valid_files.sort(key=lambda x:-x[1])
             print(f'Reading file: {data_path+valid_files[0][0]}')
             df = pd.read_pickle(data_path+valid_files[0][0])            
 
-            ## Call OpenAI api to generate the codes
-            #print(prompt.format_prompt(query=query, columns=list(df.columns)).to_messages())
-            result = chain.run(query=query, columns=list(df.columns), err_msg=err_msg)
-            print('OpenAI results')
-            print(result)
-
-            global global_result
-            global_result = result
-
-            # Use regular expression to extract substrings between ```
-            code_blocks = re.findall(r'```(.*?)```', result, flags=re.DOTALL)
-
-            # Print the extracted code blocks
-            print("code_blocks")
-            code_blocks1 = []
-            for code_block in code_blocks:
-                code_blocks1.append(code_block.replace('python','').strip())
-                print(code_block.replace('python','').strip())
+            if query != '':
+                ## Call OpenAI api to generate the codes
+                #print(prompt.format_prompt(query=query, columns=list(df.columns)).to_messages())
+                result = chain.run(query=query, columns=list(df.columns), err_msg=err_msg)
+                print('OpenAI results')
+                print(result)
+
+                global global_result
+                global_result = result
+
+                # Use regular expression to extract substrings between ```
+                code_blocks = re.findall(r'```(.*?)```', result, flags=re.DOTALL)
+
+                # Print the extracted code blocks
+                print("code_blocks")
+                code_blocks1 = []
+                for code_block in code_blocks:
+                    code_blocks1.append(code_block.replace('python','').strip())
+                    print(code_block.replace('python','').strip())               
+            else:
+                return None, df     
         else:
             raise FileExistsError(f'No matching file for {data_path}{table_name}')
 
         return code_blocks1, df
 
     def generate_chart(self, query_textbox, data_path_textbox, tablename_textbox, openai_api_key=None, err_msg=None):  
         """
@@ -122,25 +127,30 @@
         fig : Plotly figure object
             The actual figure based on query_textbox
         """  
         try:
             print('HELLO')
             code_blocks1, df = self.generate_codes(query_textbox, data_path_textbox, tablename_textbox, openai_api_key, err_msg)
             #print(df)
+            table = df.tail()#.to_dict(orient='records')
+
+            if code_blocks1 is None:
+                return None, table
+                        
             globals()['df']=df
             loc = {}    
             # execute the code        
             for code_block in code_blocks1:
                 print(code_block.strip())
                 exec(code_block.strip(), globals(), loc)
             print("loc:{loc}")
             try:
-                return loc['fig'], str(list(df.columns))
+                return loc['fig'], table # str(list(df.columns))
             except:
-                return loc['figure'], str(list(df.columns))
+                return loc['figure'], table #str(list(df.columns))
         except Exception:
             print('Start recursive exception!!!')
             etype, evalue, tb = sys.exc_info()
             err_msg = traceback.format_exception_only(etype, evalue)[-1]
             print(err_msg)
             return self.generate_chart(query_textbox, data_path_textbox, tablename_textbox, openai_api_key, err_msg)
 
@@ -159,18 +169,18 @@
             return ''
     """
 
 def run_gr():
     """
     Launch a Gradio where user can input their queries
     """
-    query_textbox = gr.inputs.Textbox(label="Query")
+    query_textbox = gr.inputs.Textbox(label="Query. Click submit with empty query to show the preview of the data")
     data_path_textbox = gr.inputs.Textbox(label="Data Folder", default="./")
     tablename_textbox = gr.inputs.Textbox(label="Table Name", default="vgt")
-    output_textbox = gr.outputs.Textbox(label="Columns")
+    output_textbox = gr.Dataframe(row_count = (5, "dynamic"), col_count = (1, "dynamic"))
     #button = gr.Button(label="Display Columns")
 
     qtg = QueryToGraph()
 
     interface = gr.Interface(fn=qtg.generate_chart, 
                                 inputs=[query_textbox, data_path_textbox, tablename_textbox],
                                 outputs=["plot", output_textbox])
```

### Comparing `querytograph-0.0.2/querytograph.egg-info/PKG-INFO` & `querytograph-0.0.3/querytograph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.2
+Version: 0.0.3
 Summary: Using ChatGPT to convert your plain English queries into graphs
-Home-page: https://github.com/franziss/querytograph
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # QueryToGraph
 QueryToGraph is a Python library that allows user to use simple English to create graph from a dataframe or csv file. It uses ChatGPT as the underlying engine. 
 
 **For security's sake, it does not send the raw data to ChatGPT** but only the data schema (i.e. the data field names) is sent.
 
 
@@ -52,14 +52,15 @@
 
 ![Chart](Screenshot.png)
 
 There are 3 textboxes which you have to key in  
 
 1. Query  
    Question by the user, which will be used to generate the graph
+   Example: "show me the highest and lowest closing price for each month"
 2. Data Folder  
    Folder which contains Pandas dataframes in csv or pkl (pickle)
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
```

### Comparing `querytograph-0.0.2/setup.py` & `querytograph-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='querytograph',
     packages=find_packages(include=['querytograph']),
-    version='0.0.2',
+    version='0.0.3',
     description='Using ChatGPT to convert your plain English queries into graphs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='franziss',
     author_email='franziss@gmail.com',
     license='MIT',
-    url="https://github.com/franziss/querytograph",
     install_requires=[
         'pandas',
         'openai',
         'langchain==0.0.160',
         'rapidfuzz==3.0.0',
         'gradio==3.26.0',
         'numpy'
```

