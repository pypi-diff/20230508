# Comparing `tmp/pinecone_cli-0.5.2-py3-none-any.whl.zip` & `tmp/pinecone_cli-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17009 bytes, number of entries: 8
--rw-r--r--  2.0 unx    36233 b- defN 23-May-01 18:03 pinecli.py
--rw-r--r--  2.0 unx     1066 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    16757 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-27 19:09 pinecone_cli-0.5.2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      670 b- defN 23-May-01 18:17 pinecone_cli-0.5.2.dist-info/RECORD
-8 files, 54867 bytes uncompressed, 15827 bytes compressed:  71.2%
+Zip file size: 17258 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    37249 b- defN 23-May-08 21:15 pinecli.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16800 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Mar-27 19:09 pinecone_cli-0.5.3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      670 b- defN 23-May-08 21:43 pinecone_cli-0.5.3.dist-info/RECORD
+8 files, 55926 bytes uncompressed, 16076 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pinecli.py
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/LICENSE
+Filename: pinecone_cli-0.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/METADATA
+Filename: pinecone_cli-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/WHEEL
+Filename: pinecone_cli-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/entry_points.txt
+Filename: pinecone_cli-0.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/top_level.txt
+Filename: pinecone_cli-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/zip-safe
+Filename: pinecone_cli-0.5.3.dist-info/zip-safe
 Comment: 
 
-Filename: pinecone_cli-0.5.2.dist-info/RECORD
+Filename: pinecone_cli-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pinecli.py

```diff
@@ -3,110 +3,132 @@
 # pylint: disable=line-too-long,too-many-arguments,invalid-name,no-member,missing-function-docstring,missing-module-docstring
 
 import hashlib
 import itertools
 import os
 import requests
 import sys
+import unittest
 
 from ast import literal_eval
 from time import sleep
 
 import click
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 import openai
 import nltk.data
 import pinecone
 
 from bs4 import BeautifulSoup
-from bs4.element import Comment
+from bs4.element import Comment, Tag
 from dotenv import load_dotenv, find_dotenv
 from numpy import random
 from sklearn.manifold import TSNE
 from sklearn.cluster import KMeans
+from retry import retry
 from rich.console import Console
 from rich.table import Table
 from tqdm.auto import tqdm
+from typing import Dict, List, Tuple, Optional, Union, TypeVar
 
 DEFAULT_REGION = 'us-west1-gcp'
 OPENAI_EMBED_MODEL = "text-embedding-ada-002"
 REGION_HELP = 'Pinecone cluster region'
 
-load_dotenv(find_dotenv(), override=True) # take environment variables from .env
+# take environment variables from .env
+load_dotenv(find_dotenv(), override=True)
 
-def tag_visible(element):
+
+U = TypeVar('U')
+
+
+def nn(inst: Optional[U]) -> U:
+    """Not-none helper to stop mypy errors"""
+    assert inst is not None
+    return inst
+
+
+def tag_visible(element: Tag) -> bool:
     """ Strip out undesirables """
-    if element.parent.name in ['style', 'script', 'head', 'title', 'meta', '[document]']:
+    parent: Tag = nn(element.parent)
+    if parent.name in ['style', 'script', 'head', 'title', 'meta', '[document]']:
         return False
     if isinstance(element, Comment):
         return False
     return True
 
-def _text_from_html(body):
+
+def _text_from_html(body: str) -> str:
     """ Obv pull text from doc with tag_visible filters """
     soup = BeautifulSoup(body, 'html.parser')
     texts = soup.findAll(string=True)
     visible_texts = filter(tag_visible, texts)
     return " ".join(t.strip() for t in visible_texts)
 
-def _get_openai_embedding(apikey, data):
-    """ Fetch an embedding w/ given data """
+
+"""
+def _get_openai_embedding(apikey: str, data: str) -> openai.Embedding:
     openai.api_key = apikey
     try:
         res = openai.Embedding.create(input=data, engine=OPENAI_EMBED_MODEL)
     except:
         done = False
         while not done:
             sleep(5)
             try:
                 res = openai.Embedding.create(
                     input=data, engine=OPENAI_EMBED_MODEL)
                 done = True
             except Exception as e:
                 click.echo(e)
     return res
+"""
+
+
+@retry(tries=3, delay=5)
+def _get_openai_embedding(apikey: str, data: list[str]) -> openai.Embedding:
+    openai.api_key = apikey
+    return openai.Embedding.create(input=data, engine=OPENAI_EMBED_MODEL)
 
 
 @click.group()
-def cli():
+def cli() -> None:
     """
     A command line interface for working with Pinecone.
     """
     pass
 
-def exception_handler(exception_type, exception, traceback):
-    # All your trace are belong to us!
-    click.echo(f"Got exception: {exception_type.__name__}  {exception}")
-    click.echo("Make sure PINECONE_API_KEY is correct.")
-
-# sys.excepthook = exception_handler
-
 
-def _pinecone_init(apikey, environment, indexname=''):
+def _pinecone_init(apikey: str, environment: str, indexname: str = '') -> pinecone.GRPCIndex:
     index = None
-    apikey = os.environ.get('PINECONE_API_KEY', apikey) if apikey is None else apikey
-    environment = os.environ.get('PINECONE_ENVIRONMENT', environment) if environment is None else environment
+    apikey = os.environ.get(
+        'PINECONE_API_KEY', apikey) if apikey is None else apikey
+    environment = os.environ.get(
+        'PINECONE_ENVIRONMENT', environment) if environment is None else environment
     if apikey is None:
         sys.exit(
             "No Pinecone API key set through PINECONE_API_KEY in .env file, environment variable or --apikey\nExample: export PINECONE_API_KEY=1234-abc-9876")
     pinecone.init(api_key=apikey, environment=environment)
     if indexname:
         try:
-            #index = pinecone.Index(indexname)
+            # index = pinecone.Index(indexname)
             index = pinecone.GRPCIndex(indexname)
         except:
             sys.exit("Unable to connect.  Caught exception:")
     return index
 
-def _format_values(vals):
+
+def _format_values(vals) -> str:
     return ",".join(str(x) for x in vals)[:30]
 
-def _print_table(res, pinecone_index_name, namespace, include_meta, include_values, expand_meta):
+
+def _print_table(res, pinecone_index_name, namespace, include_meta, include_values, expand_meta) -> None:
+    """ Print a table of results """
     table = Table(
         title=f"🌲 {pinecone_index_name} ns=({namespace}) Index Results")
     table.add_column("ID", justify="right", style="cyan", no_wrap=True)
     table.add_column("NS", justify="left", style="red", no_wrap=True)
     if include_values:
         table.add_column("Values", style="magenta")
     if include_meta:
@@ -132,22 +154,24 @@
             table.add_row(vecid, ns, metadata, score)
         elif not include_values and not include_meta:
             table.add_row(vecid, ns, score)
 
     console = Console()
     console.print(table)
 
+
 @click.command(short_help='Prints version number.')
-def version():
+def version() -> None:
     if sys.version_info >= (3, 8):
         from importlib import metadata
     else:
         import importlib_metadata as metadata
     click.echo(metadata.version('pinecone_cli'))
 
+
 @click.command(short_help='Queries Pinecone with a given vector.')
 @click.option('--apikey',  help='Pinecone API Key')
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--include_values', help='Should we return the vectors', show_default=True, default=True)
 @click.option('--topk', '--numrows', 'topk', type=click.INT, show_default=True, default=10, help='Top K number to return')
 @click.option('--namespace',  default="", help='Namespace to select results from')
 @click.option('--include-meta', help='Whether to include the metadata values', default=False, show_default=True)
@@ -156,15 +180,16 @@
 @click.option('--print-table', help='Display the output as a pretty table.', is_flag=True, show_default=True, default=False)
 @click.option('--num-clusters', help='Number of clusters in TSNE plot if --show-tsne is used.', type=click.INT, show_default=True, default=4)
 @click.option('--perplexity', '--perp', help='The perplexity of the TSNE plot, if --show-tsne is used.', type=click.INT, default=15, show_default=True)
 @click.option('--tsne-random-state', type=click.INT, default=42, show_default=True)
 @click.option('--show-tsne', default=False)
 @click.argument('pinecone_index_name')
 @click.argument('query_vector')
-def query(pinecone_index_name, apikey, query_vector, region, topk, include_values, include_meta, expand_meta, num_clusters, perplexity, tsne_random_state, namespace, show_tsne, meta_filter, print_table):
+def query(pinecone_index_name, apikey, query_vector, region=DEFAULT_REGION, topk=10, include_values=True, include_meta=True, expand_meta=False, num_clusters=4,
+          perplexity=15, tsne_random_state=True, namespace="", show_tsne=False, meta_filter="{}", print_table=False) -> None:
     """ Queries Pinecone index named <PINECONE_INDEX_NAME> with the given <QUERY_VECTOR> and optional namespace. 
 
         \b
         Example: 
         % ./pinecli.py query lpfactset  "[0,0]"
 
         \b
@@ -183,27 +208,27 @@
         res = index.describe_index_stats()
         num_vector_dims = res['dimension']
         query_vector = [i for i in range(num_vector_dims)]
     else:
         query_vector = literal_eval(query_vector)
 
     res = index.query(vector=query_vector, top_k=topk, include_metadata=True,
-                               include_values=include_values, namespace=namespace, filter=literal_eval(meta_filter))
+                      include_values=include_values, namespace=namespace, filter=literal_eval(meta_filter))
     if print_table:
         _print_table(res, pinecone_index_name, namespace,
                      include_meta, include_values, expand_meta)
     else:
         click.echo(res)
 
     if show_tsne:
         show_tsne_plot(pinecone_index_name, res.matches,
                        num_clusters, perplexity, tsne_random_state)
 
 
-def show_tsne_plot(pinecone_index_name, results, num_clusters, perplexity, random_state):
+def show_tsne_plot(pinecone_index_name, results, num_clusters, perplexity, random_state):  # pragma: no cover
     res2 = np.asarray([np.array(v['values']) for v in results])
     df = pd.DataFrame(data=res2)
 
     kmeans = KMeans(n_clusters=num_clusters, init="k-means++",
                     random_state=random_state, n_init='auto')
     kmeans.fit(res2)
     labels = kmeans.labels_
@@ -238,17 +263,17 @@
 
 
 @click.command(short_help='Fetches vectors from Pinecone specified by the vectors\' ids.')
 @click.option('--apikey', help='Pinecone API Key')
 @click.option('--region', help='Pinecone Index Region', default=DEFAULT_REGION)
 @click.option('--vector_ids', help='Vector ids to fetch')
 @click.option('--pretty', is_flag=True, help='Pretty print output.')
-@click.option('--namespace', help='Namespace within the index to search.')
+@click.option('--namespace', help='Namespace within the index to search.', default="")
 @click.argument('pinecone_index_name')
-def fetch(pinecone_index_name, apikey, region, vector_ids, namespace, pretty):
+def fetch(pinecone_index_name: str, apikey: str, region: str, vector_ids: str, namespace: str = "", pretty: bool = True) -> None:
     """ Fetch queries from Pinecone by vector_ids 
 
         \b    
         Example:
         % ./pinecli.py fetch lpfactset --vector_ids="05b4509ee655aacb10bfbb6ba212c65c"
     """
     index = _pinecone_init(apikey, region, pinecone_index_name)
@@ -263,15 +288,15 @@
 @click.command(short_help='Extracts text from url arg, vectorizes w/ openai embedding api, and upserts to Pinecone.')
 @click.option('--apikey', help='Pinecone API Key')
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--namespace', help='Pinecone index namespace', default='', show_default=True)
 @click.option("--debug", is_flag=True, show_default=True, default=False, help="Output debug to stdout.")
 @click.argument('pinecone_index_name')
 @click.argument('vector_literal')
-def upsert(pinecone_index_name, apikey, region, vector_literal, namespace, debug):
+def upsert(pinecone_index_name: str, apikey: str, region: str, vector_literal: str, namespace: str = "", debug: bool = False) -> None:
     """ 
     Upserts vectors into the index <PINECONE_INDEX_NAME> by using the <VECTOR_LITERAL> which is a string representation of a list of tuples.
     Note the literal is quoted.
 
     \b
     Example:
     % ./pinecli.py upsert upsertfile "[('vec1', [0.1, 0.2, 0.3], {'genre': 'drama'}), ('vec2', [0.2, 0.3, 0.4], {'genre': 'action'}),]" --debug 
@@ -289,15 +314,15 @@
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--namespace', help='Pinecone index namespace', default='', show_default=True)
 @click.option("--debug", is_flag=True, show_default=True, default=False, help="Output debug to stdout.")
 @click.option("--metadata", help="The update to the metadata values.", default='', show_default=True)
 @click.argument("id")
 @click.argument('pinecone_index_name')
 @click.argument('vector_literal')
-def update(pinecone_index_name, apikey, region, id, vector_literal, metadata, namespace, debug):
+def update(pinecone_index_name: str, apikey: str, region: str, id: str, vector_literal: str, metadata: str, namespace: str, debug: bool = False):
     """ Updates the index <PINECONE_INDEX_NAME> with id <ID> and vector values <VECTOR_LITERAL> """
     index = _pinecone_init(apikey, region, pinecone_index_name)
     if metadata:
         resp = index.update(id=id, values=literal_eval(
             vector_literal), set_metadata=literal_eval(metadata), namespace=namespace)
     else:
         resp = index.update(id=id, values=literal_eval(
@@ -314,17 +339,20 @@
 @click.option("--namespace", help='Namespace to store the generated vectors', default='', show_default=True)
 @click.option("--metadata_content_key", help="The key used to store the page content in the metadata with.", show_default=True, default="content")
 @click.option("--window", help='Number of sentences to combine in one embedding (vector).', show_default=True, default=10)
 @click.option("--other_meta", help="Other meta to merge w/ the metadata_content_key", show_default=True, default="{}")
 @click.option("--stride", help='Number of sentences to stride over to create overlap', show_default=True, default=4)
 @click.argument('url')
 @click.argument('pinecone_index_name')
-def upsert_webpage(pinecone_index_name, apikey, namespace, openaiapikey, metadata_content_key, other_meta, region, url, window, stride, debug):
+def upsert_webpage(pinecone_index_name, apikey, namespace, openaiapikey, metadata_content_key, other_meta, region, url, window, stride, debug) -> None:
     """ Upserts vectors into the index <PINECONE_INDEX_NAME> using the openai embeddings api.  You will need your api key for openai and specify it using --openapikey """
     pinecone_index = _pinecone_init(apikey, region, pinecone_index_name)
+    if openaiapikey is None or openaiapikey == "":
+        raise ValueError(
+            "You need to specify an OpenAI API key using --openaiapikey")
 
     html = requests.get(url).text
     html = _text_from_html(html)
     nltk.download('punkt')
     tokenizer = nltk.data.load('tokenizers/punkt/english.pickle')
     sentences = tokenizer.tokenize(html)
     sentences = list(filter(None, sentences))
@@ -352,36 +380,38 @@
     for i in tqdm(range(0, len(new_data), batch_size)):
         i_end = min(len(new_data), i+batch_size)
         meta_batch = new_data[i:i_end]
         ids_batch = [hashlib.md5(x.encode('utf-8')).hexdigest()
                      for x in meta_batch]
         res = _get_openai_embedding(openaiapikey, meta_batch)
         embeds = [record['embedding'] for record in res['data']]
-        new_meta_batch=[]
+        new_meta_batch = []
         for x in meta_batch:
             d = {metadata_content_key: x}
             d.update(literal_eval(other_meta))
             new_meta_batch.append(d)
         to_upsert = list(zip(ids_batch, embeds, new_meta_batch))
         rv = pinecone_index.upsert(vectors=to_upsert, namespace=namespace)
         if debug:
             click.echo(rv)
 
+
 @click.command(short_help='Shows a preview of vectors in the <PINECONE_INDEX_NAME>')
 @click.option('--apikey', help='Pinecone API Key')
 @click.option('--region', help='Pinecone Index Region', default=DEFAULT_REGION)
 @click.option('--topk', '--numrows', 'topk', default=10, help='The number of rows to show')
 @click.option('--random_dims', is_flag=True, help='Flag to have query vector dims be random.  Default will be 0.0')
 @click.option('--include-values', help='Should we return the vectors', show_default=True, default=True)
 @click.option('--namespace',  default="", help='Namespace to select results from')
 @click.option('--include-meta', help='Whether to include the metadata values', default=False, show_default=True)
 @click.option('--expand-meta', help='Whether to fully expand the metadata returned.', is_flag=True, show_default=True, default=False)
 @click.option('--print-table', help='Display the output as a pretty table.', is_flag=True, show_default=True, default=False)
 @click.argument('pinecone_index_name')
-def head(pinecone_index_name, apikey, region, topk, random_dims, namespace, include_meta, expand_meta, include_values, print_table):
+def head(pinecone_index_name: str, apikey: str, region: str, topk: int = 10, random_dims: int = 0, namespace: str = "",
+         include_meta: bool = False, expand_meta: bool = False, include_values: bool = True, print_table: bool = False) -> None:
     """ Shows a preview of vectors in the <PINECONE_INDEX_NAME> with optional numrows (default 10) 
     \b
         Example 1:
 
         % ./pinecli.py head lpfactset --include-meta=true --include-values=true 
         {'matches': [{'id': 'ae23d7574c19cea0b3479c93858a3ee3',
               'metadata': {'content': 'Oded K. R&D Group Lead          Why '
@@ -410,15 +440,15 @@
     res = pinecone_index.describe_index_stats()
     dims = res['dimension']
     if random_dims:
         dims = [random.random() for _ in range(dims)]
     else:
         dims = [0.0 for _ in range(dims)]
     resp = pinecone_index.query(vector=dims, top_k=topk, namespace=namespace,
-                       include_metadata=include_meta, include_values=include_values)
+                                include_metadata=include_meta, include_values=include_values)
     if print_table:
         _print_table(resp, pinecone_index_name, namespace,
                      include_meta, include_values, expand_meta)
     else:
         click.echo(resp)
 
 
@@ -436,35 +466,31 @@
 def create_index(pinecone_index_name, apikey, region, dims, metric, pods, replicas, shards, pod_type, source_collection):
     """ Creates the Pinecone index named <PINECONE_INDEX_NAME> """
     index = _pinecone_init(apikey, region, pinecone_index_name)
     resp = pinecone.create_index(pinecone_index_name, dimension=dims, metric=metric,
                                  pods=pods, replicas=replicas, shards=shards, pod_type=pod_type, source_collection=source_collection)
     click.echo(resp)
 
+
 def chunks(iterable, batch_size=100):
     it = iter(iterable)
     chunk = tuple(itertools.islice(it, batch_size))
     while chunk:
         yield chunk
         chunk = tuple(itertools.islice(it, batch_size))
 
 
-def chunks_df(df):
-    for row in df.itertuples(index=False):
-        yield row
-
-
 @click.command(short_help='Upserts a vector(s) with random dimensions into the specified vector.')
 @click.option('--apikey',  help='Pinecone API Key')
 @click.option('--region', help='Pinecone Index Region', default=DEFAULT_REGION)
 @click.argument('pinecone_index_name')
 @click.option('--num_vectors', '--num_rows', '--numrows', type=click.INT)
 @click.option('--debug', is_flag=True, default=False, show_default=True)
 @click.option('--num_vector_dims', type=click.INT)
-def upsert_random(pinecone_index_name, apikey, region, num_vectors, num_vector_dims, debug):
+def upsert_random(pinecone_index_name, apikey, region, num_vectors, num_vector_dims, debug) -> None:
     """ Upserts random vectors and dimension values using num_vectors (rows) and num_vector_dims (number of dims per vector). IDs for the example vectors will be of the form \'id-{rownum}\' """
     index = _pinecone_init(apikey, region, pinecone_index_name)
 
     # Example generator that generates many (id, vector) pairs
     example_data_generator = map(lambda i: (
         f'id-{i}', [random.random() for _ in range(num_vector_dims)]), range(num_vectors))
 
@@ -510,53 +536,59 @@
 
     for chunk in pd.read_csv(vector_file, chunksize=batch_size, index_col=False, usecols=usecols, converters=converters):
         v = chunk.to_records(index=False).tolist()
         rv = index.upsert(vectors=v, namespace=namespace)
         if debug:
             click.echo(rv)
 
-    
+
 @click.command(short_help='Lists the indexes for your api key.')
 @click.option('--apikey', help='API Key')
 @click.option('--print-table', is_flag=True, default=False)
 @click.argument('region', default=DEFAULT_REGION)
-def list_indexes(apikey, region, print_table):
+def list_indexes(apikey: str, region: str, print_table: bool = False) -> None:
     """ List all Pinecone indexes for the given api key. """
     index = _pinecone_init(apikey, region)
     res = pinecone.list_indexes()
     if not print_table:
         click.echo('\n'.join(res))
     else:
         table = Table(
-        title=f"🌲 Indexes")
-        table.add_column("Index Name", justify="right", style="cyan", no_wrap=True)
-        table.add_column("Dimensions", justify="right", style="cyan", no_wrap=True)
+            title=f"🌲 Indexes")
+        table.add_column("Index Name", justify="right",
+                         style="cyan", no_wrap=True)
+        table.add_column("Dimensions", justify="right",
+                         style="cyan", no_wrap=True)
         table.add_column("Metric", justify="right", style="cyan", no_wrap=True)
-        table.add_column("Replicas", justify="right", style="cyan", no_wrap=True)
+        table.add_column("Replicas", justify="right",
+                         style="cyan", no_wrap=True)
         table.add_column("Pods", justify="right", style="cyan", no_wrap=True)
-        table.add_column("Pod Type", justify="right", style="cyan", no_wrap=True)
+        table.add_column("Pod Type", justify="right",
+                         style="cyan", no_wrap=True)
         table.add_column("Shards", justify="right", style="cyan", no_wrap=True)
         table.add_column("Ready", justify="right", style="cyan", no_wrap=True)
         table.add_column("State", justify="right", style="cyan", no_wrap=True)
 
         for index in res:
             desc = pinecone.describe_index(index)
             state = str(desc.status['state'])
             ready = str(desc.status['ready'])
             ready_formatted = f"[bold green]{ready}[/bold green]" if ready == "True" else f"[bold yellow]{ready}[/bold yellow]"
-            table.add_row(index, f"{int(desc.dimension)}", desc.metric, str(desc.replicas), str(desc.pods), desc.pod_type, str(desc.shards), ready_formatted, desc.status['state'])
+            table.add_row(index, f"{int(desc.dimension)}", desc.metric, str(desc.replicas), str(
+                desc.pods), desc.pod_type, str(desc.shards), ready_formatted, desc.status['state'])
 
         console = Console()
         console.print(table)
 
+
 @click.command(short_help='Describes an index.')
 @click.option('--apikey')
 @click.argument('pinecone_index_name', required=True)
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
-def describe_index(apikey, pinecone_index_name, region):
+def describe_index(apikey: str, pinecone_index_name: str, region: str = DEFAULT_REGION) -> None:
     """ Describe a Pinecone index with given index_name. """
     index = _pinecone_init(apikey, region, pinecone_index_name)
     desc = pinecone.describe_index(pinecone_index_name)
     click.echo("\n".join([f"Name: {desc.name}", f"Dimensions: {int(desc.dimension)}",
                           f"Metric: {desc.metric}", f"Pods: {desc.pods}", f"PodType: {desc.pod_type}", f"Shards: {desc.shards}",
                           f"Replicas: {desc.replicas}", f"Ready: {desc.status['ready']}", f"State: {desc.status['state']}"
                           f"Metaconfig: {desc.metadata_config}", f"Sourcecollection: {desc.source_collection}"]))
@@ -578,25 +610,26 @@
 @click.argument('pinecone_index_name', required=True)
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--num_replicas', required=True, help='Number of replicas to use.')
 def configure_index_replicas(apikey, pinecone_index_name, region, num_replicas):
     """ Configure the number of replicas for an index. """
     _pinecone_init(apikey, region)
     pinecone.configure_index(pinecone_index_name, replicas=num_replicas)
-    
+
+
 @click.command(short_help='Minimizes everything for a cluster to lowest settings.')
 @click.option('--apikey')
 @click.argument('pinecone_index_name', required=True)
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 def minimize_cluster(apikey, pinecone_index_name, region):
     """ Minimizes a cluster to lowest settings index. """
     _pinecone_init(apikey, region)
     pinecone.configure_index(pinecone_index_name, replicas=1, pod_type='s1.x1')
 
-    
+
 @click.command(short_help='Creates a Pinecone collection from the argument \'source_index\'')
 @click.option('--apikey')
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--collection_name', help='The name of the collection to create.', required=True)
 @click.option('--source_index', help='The name index to create collection from.', required=True)
 def create_collection(apikey, region, collection_name, source_index):
     """ Create a Pinecone collection with the given collection_name and source_index. """
@@ -657,24 +690,26 @@
 def delete_all(pinecone_index_name, apikey, region, namespace):
     """ Delete all vectors from the index with optional namespace, but doesnt delete the index itself, will simply have 0 vectors.
         If you want to delete the entire index from existence, use 'delete-index'
     """
     index = _pinecone_init(apikey, region, pinecone_index_name)
     delete_response = index.delete(delete_all=True, namespace=namespace)
     click.echo(delete_response)
-    
+
+
 @click.command(short_help="Deletes a collection.")
 @click.option('--apikey')
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--collection_name', help='The name of the collection to create.', required=True)
 def delete_collection(apikey, region, collection_name):
     """ Delete a collection with the given collection_name """
     _pinecone_init(apikey, region)
     pinecone.delete_collection(collection_name)
 
+
 @click.command(short_help='Deletes an index.  You will be prompted to confirm.')
 @click.option('--apikey')
 @click.option('--region', help='Pinecone Index Region', show_default=True, default=DEFAULT_REGION)
 @click.option('--disable-safety', is_flag=True, default=False, show_default=True, help='Disables the prompt check to see if you really want to delete')
 @click.argument('pinecone_index', required=True)
 def delete_index(apikey, region, pinecone_index, disable_safety):
     """ Delete an index with the given pinecone_index name """
@@ -682,14 +717,15 @@
     if not disable_safety:
         value = click.prompt('Type name of index backwards to confirm: ')
         if value != pinecone_index[::-1]:
             click.echo("Index not deleted: reversed index name does not match.")
 
     pinecone.delete_index(pinecone_index)
 
+
 cli.add_command(query)
 cli.add_command(upsert)
 cli.add_command(upsert_file)
 cli.add_command(upsert_random)
 cli.add_command(update)
 cli.add_command(list_indexes)
 cli.add_command(delete_index)
@@ -707,8 +743,7 @@
 cli.add_command(head)
 cli.add_command(version)
 cli.add_command(minimize_cluster)
 cli.add_command(delete_all)
 
 if __name__ == "__main__":
     cli()
-
```

## Comparing `pinecone_cli-0.5.2.dist-info/LICENSE` & `pinecone_cli-0.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pinecone_cli-0.5.2.dist-info/METADATA` & `pinecone_cli-0.5.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: pinecone-cli is a command-line client for interacting with the pinecone vector embedding database.
 Home-page: https://github.com/tullytim/pinecone-cli
 Author: Tim Tully
 Author-email: tim@menlovc.com
 License: MIT
 Keywords: pinecone vector vectors embeddings database transformers models
 Platform: any
@@ -19,16 +19,18 @@
 Requires-Dist: openai
 Requires-Dist: pinecone-client
 Requires-Dist: pinecone-client[grpc]
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: beautifulsoup4
 Requires-Dist: nltk
+Requires-Dist: retry
 Requires-Dist: rich
 Requires-Dist: python-dotenv
+Requires-Dist: typing
 
 # pinecone-cli
 
 Pinecode-cli is a command-line interface for control and data plane interfacing with [Pinecone](https://pinecone.io).
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/pinecone-cli.svg)](https://badge.fury.io/py/pinecone-cli)
```

## Comparing `pinecone_cli-0.5.2.dist-info/RECORD` & `pinecone_cli-0.5.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pinecli.py,sha256=sovXAG6WtrO1MgLWjCAQGpKaJKAFsTpouueMT7htP0o,36233
-pinecone_cli-0.5.2.dist-info/LICENSE,sha256=VjvZTlbmhfhAS-5Rcv5v5btqvHqNzuXqTShn56FcdzY,1066
-pinecone_cli-0.5.2.dist-info/METADATA,sha256=CDVccUH_Agz5bPaVALs-eM2uLdiflJ3-EPI1-WCPlcc,16757
-pinecone_cli-0.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pinecone_cli-0.5.2.dist-info/entry_points.txt,sha256=lUn2MPNuP8UGCE4D0O76Sck6WBwxbk8n59TqcJgVqU8,40
-pinecone_cli-0.5.2.dist-info/top_level.txt,sha256=JrqfDpPEXItSt4PxDzpUNSzxFSn4p8dCym_tZmSX-oE,8
-pinecone_cli-0.5.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pinecone_cli-0.5.2.dist-info/RECORD,,
+pinecli.py,sha256=JltOMuSljVyw27ydmLwt0MR2uEzKEqXUquZpJ_RpWjM,37249
+pinecone_cli-0.5.3.dist-info/LICENSE,sha256=VjvZTlbmhfhAS-5Rcv5v5btqvHqNzuXqTShn56FcdzY,1066
+pinecone_cli-0.5.3.dist-info/METADATA,sha256=qSF5x1X0k8EHWyffCwX0NAJNR0CFZ_S_qDjpAYPlLWQ,16800
+pinecone_cli-0.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pinecone_cli-0.5.3.dist-info/entry_points.txt,sha256=lUn2MPNuP8UGCE4D0O76Sck6WBwxbk8n59TqcJgVqU8,40
+pinecone_cli-0.5.3.dist-info/top_level.txt,sha256=JrqfDpPEXItSt4PxDzpUNSzxFSn4p8dCym_tZmSX-oE,8
+pinecone_cli-0.5.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pinecone_cli-0.5.3.dist-info/RECORD,,
```

