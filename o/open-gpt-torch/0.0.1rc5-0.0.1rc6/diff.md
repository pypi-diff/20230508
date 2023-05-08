# Comparing `tmp/open_gpt_torch-0.0.1rc5.tar.gz` & `tmp/open_gpt_torch-0.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc5.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc6.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc5.tar` & `open_gpt_torch-0.0.1rc6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0    10825 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/LICENSE
--rw-r--r--   0        0        0     7518 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/README.md
--rw-r--r--   0        0        0     1144 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/__main__.py
--rw-r--r--   0        0        0      474 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/adapter.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0     1232 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     3088 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/factory.py
--rw-r--r--   0        0        0     1767 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/hub.py
--rw-r--r--   0        0        0      512 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     5274 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     5658 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     8561 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0     1074 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0      638 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/hf_model.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0      846 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0      984 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     1860 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/loading.py
--rw-r--r--   0        0        0     1422 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     1096 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0      790 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/models/stablelm/loading.py
--rw-r--r--   0        0        0     2862 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1504 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0      437 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/flow.py
--rw-r--r--   0        0        0      931 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0     2229 2023-04-27 06:21:46.432002 open_gpt_torch-0.0.1rc5/pyproject.toml
--rw-r--r--   0        0        0    19858 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc5/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/LICENSE
+-rw-r--r--   0        0        0     7531 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/README.md
+-rw-r--r--   0        0        0      853 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/__main__.py
+-rw-r--r--   0        0        0      474 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/adapter.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0     1232 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     1898 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/factory.py
+-rw-r--r--   0        0        0     1767 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/hub.py
+-rw-r--r--   0        0        0      498 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     5274 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     5658 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     8561 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0      846 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/llama/loading.py
+-rw-r--r--   0        0        0     4469 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2623 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     1860 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/loading.py
+-rw-r--r--   0        0        0      947 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0      669 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0      852 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/loading.py
+-rw-r--r--   0        0        0     1619 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0     2862 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0      437 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/flow.py
+-rw-r--r--   0        0        0      931 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0     2263 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/pyproject.toml
+-rw-r--r--   0        0        0    19871 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc6/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc5/LICENSE` & `open_gpt_torch-0.0.1rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/README.md` & `open_gpt_torch-0.0.1rc6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # OpenGPT
 
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
 
-> The content of README.md is just a placeholder to remind me of what I want to do.
+> **Note**
+> The content of `README.md` is just a placeholder to remind me of what I want to do.
 
 ## Features
 
 OpenGPT provides the following features to make it easy to deploy and serve large multi-modal models (LMMs) in production:
 
 - Support for multi-modal models
 - Scalable architecture for handling high traffic loads
```

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/cli/application.py` & `open_gpt_torch-0.0.1rc6/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/loading.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,66 @@
-from pathlib import Path
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import torch
 from loguru import logger
 
-from .helper import auto_dtype_and_device
+from open_gpt.helper import auto_dtype_and_device
 
 
-def list_models():
-    """List the available models."""
-    ...
+def load_model_and_tokenizer(
+    model_name_or_path: str,
+    tokenizer_name_or_path: Optional[str] = None,
+    device: Optional[torch.device] = None,
+    dtype: Optional[Union[str, torch.dtype]] = None,
+    device_map: Optional[Union[str, List[int]]] = None,
+    no_split_module_classes: Optional[List[str]] = None,
+    **kwargs,
+):
+    """Load a model and tokenizer from HuggingFace."""
+    import os
 
+    from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 
-def load_state_dict(model: torch.nn.Module, checkpoint: Union[str, 'Path']):
-    """Load a model state dict.
+    dtype, device = auto_dtype_and_device(dtype, device)
 
-    :param model: The model to load the state dict into.
-    :param checkpoint: The checkpoint to load the state dict from. It can be a path to a checkpoint file/folder or a URL.
-    """
-    ...
+    tokenizer = AutoTokenizer.from_pretrained(
+        tokenizer_name_or_path or model_name_or_path, trust_remote_code=True
+    )
+
+    if device_map:
+        import huggingface_hub
+        from accelerate import init_empty_weights, load_checkpoint_and_dispatch
+
+        if not os.path.exists(model_name_or_path):
+            model_path = huggingface_hub.snapshot_download(model_name_or_path)
+        else:
+            model_path = model_name_or_path
+
+        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=True)
+        with init_empty_weights():
+            model = AutoModelForCausalLM.from_config(
+                config, torch_dtype=dtype, trust_remote_code=True
+            )
+            # make sure token embedding weights are still tied if needed
+            model.tie_weights()
+
+            model = load_checkpoint_and_dispatch(
+                model,
+                model_path,
+                device_map=device_map,
+                no_split_module_classes=no_split_module_classes,
+                dtype=dtype,
+            )
+    else:
+        model = AutoModelForCausalLM.from_pretrained(
+            model_name_or_path, torch_dtype=dtype, trust_remote_code=True
+        )
+        model.to(device)
+
+    return model, tokenizer
 
 
 def create_model_and_transforms(
     model_name: str,
     device: Optional[Union[str, torch.device]] = None,
     precision: Optional[str] = None,
     **kwargs,
@@ -42,53 +80,53 @@
     model_config = {}
 
     logger.info(
         f'Loading "{model_name}" with precision: `{dtype}` on device: `{device}`'
     )
 
     if model_name.startswith('openflamingo/OpenFlamingo'):
-        from .models.flamingo.loading import load_model_and_transforms
+        from .flamingo.loading import load_model_and_transforms
 
         model_config = {
             'vision_model_name_or_path': 'ViT-L-14::openai',
             'lang_model_name_or_path': 'llama_7B',
             'tokenizer_name_or_path': 'llama_7B',
         }
         return load_model_and_transforms(
             model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('facebook/llama'):
-        from .models.llama.loading import load_model_and_tokenizer
+        from .llama.loading import load_model_and_tokenizer
 
         model_config = {
             'model_name_or_path': 'llama_7B',
             'tokenizer_name_or_path': 'llama_7B',
         }
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('google/flan'):
-        from .models.flan.loading import load_model_and_tokenizer
+        from .flan.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('EleutherAI/pythia'):
-        from .models.pythia.loading import load_model_and_tokenizer
+        from .pythia.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('stabilityai/stablelm'):
-        from .models.stablelm.loading import load_model_and_tokenizer
+        from .stablelm.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config
         )
     elif model_name.startswith('fnlp/moss-moon'):
-        from .models.moss.loading import load_model_and_tokenizer
+        from .moss.loading import load_model_and_tokenizer
 
         return load_model_and_tokenizer(
             model_name, device=device, dtype=dtype, **model_config, **kwargs
         )
     else:
         raise ValueError(f'Unknown model name: {model_name}')
```

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/helper.py` & `open_gpt_torch-0.0.1rc6/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/flan/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/hf_model.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/llama/loading.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-from typing import Optional
+from typing import Optional, Union
 
 import torch
+from loguru import logger
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
-    dtype: 'torch.dtype' = torch.float16,
+    dtype: Optional[Union[str, torch.dtype]] = None,
     **kwargs
 ):
     """Load a model and tokenizer from HuggingFace."""
+
+    from ...helper import auto_dtype_and_device
+
+    dtype, device = auto_dtype_and_device(dtype, device)
+
     tokenizer = AutoTokenizer.from_pretrained(
-        tokenizer_name_or_path or model_name_or_path
+        tokenizer_name_or_path or model_name_or_path, local_files_only=False
     )
 
     model = AutoModelForCausalLM.from_pretrained(
         model_name_or_path,
         torch_dtype=dtype,
+        local_files_only=False,
     )
     model.to(device)
 
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/llama/loading.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/loading.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import torch
 from loguru import logger
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
     dtype: Optional[Union[str, torch.dtype]] = None,
+    device_map: Optional[Union[str, List[int]]] = None,
     **kwargs
 ):
     """Load a model and tokenizer from HuggingFace."""
 
     from ...helper import auto_dtype_and_device
 
     dtype, device = auto_dtype_and_device(dtype, device)
 
     tokenizer = AutoTokenizer.from_pretrained(
-        tokenizer_name_or_path or model_name_or_path, local_files_only=False
+        tokenizer_name_or_path or model_name_or_path
     )
 
     model = AutoModelForCausalLM.from_pretrained(
         model_name_or_path,
         torch_dtype=dtype,
-        local_files_only=False,
     )
     model.to(device)
 
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/models/moss/loading.py` & `open_gpt_torch-0.0.1rc6/open_gpt/models/moss/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc6/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from multiprocessing.pool import ThreadPool
 from typing import Dict, List, Optional, Union
 
 import torch
 from docarray import DocumentArray
 from jina import Executor, requests
 
-from open_gpt.factory import create_model_and_transforms
+from open_gpt.factory import create_model
 from open_gpt.logging import logger
 
 
 class CausualLMExecutor(Executor):
     def __init__(
         self,
         model_name_or_path: str = '',
@@ -27,18 +27,27 @@
             model_name_or_path
         ), '`model_name_or_path` must be provided to initialize the model and tokenizer.'
 
         self._model_name_or_path = model_name_or_path
         self._minibatch_size = minibatch_size
         self._thread_pool = ThreadPool(processes=num_workers)
 
-        logger.info(f'==> loading model of `{model_name_or_path}` ...')
-        self.model, self.tokenizer, *_ = create_model_and_transforms(
+        self.model = create_model(
             model_name_or_path, precision=precision, device_map=device_map, **kwargs
         )
 
+        # warmup the model to avoid the first-time slowness
+        self.model.generate(['Hello world!'])
+
     @requests
     def generate(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
-        num_captions = int(parameters.get('num_captions', 1))
         prompted_da = DocumentArray(
             [d for d in docs if d.tags.get('prompt') is not None]
         )
+        prompts = [d.tags['prompt'] for d in prompted_da]
+
+        if prompts:
+            result = self.model.generate(prompts, **parameters)
+            for d, r in zip(prompted_da, result):
+                d.tags['generated_text'] = r
+        else:
+            logger.warning('No prompts found in the request.')
```

### Comparing `open_gpt_torch-0.0.1rc5/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.1rc6/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc5/pyproject.toml` & `open_gpt_torch-0.0.1rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc5"
+version = "0.0.1rc6"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
@@ -53,14 +53,16 @@
 open-flamingo = { version = "^0.0", optional = true }
 
 [tool.poetry.extras]
 flamingo = ["open-flamingo"]
 
 # Dependency groups are supported for organizing your dependencies
 [tool.poetry.group.dev.dependencies]
+ruff = "^0.0.262"
+mypy = "^1.2.0"
 pre-commit = ">=2.15.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0"
 pytest-mock = ">=3.5"
 
 [tool.pytest.ini_options]
 # Ignore deprecation warnings
```

### Comparing `open_gpt_torch-0.0.1rc5/PKG-INFO` & `open_gpt_torch-0.0.1rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc5
+Version: 0.0.1rc6
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -36,15 +36,16 @@
 Description-Content-Type: text/markdown
 
 # OpenGPT
 
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution. 
 It is designed to simplify the deployment and management of large language models, on a distributed cluster of GPUs.
 
-> The content of README.md is just a placeholder to remind me of what I want to do.
+> **Note**
+> The content of `README.md` is just a placeholder to remind me of what I want to do.
 
 ## Features
 
 OpenGPT provides the following features to make it easy to deploy and serve large multi-modal models (LMMs) in production:
 
 - Support for multi-modal models
 - Scalable architecture for handling high traffic loads
```

