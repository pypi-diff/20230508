# Comparing `tmp/QuNet-0.0.8-py3-none-any.whl.zip` & `tmp/QuNet-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 30601 bytes, number of entries: 12
+Zip file size: 31279 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
 -rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
--rw-rw-rw-  2.0 fat    22012 b- defN 23-Apr-22 16:36 qunet/models.py
+-rw-rw-rw-  2.0 fat    21899 b- defN 23-Apr-22 20:00 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
 -rw-rw-rw-  2.0 fat    10435 b- defN 23-Apr-22 11:36 qunet/optim.py
 -rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-22 14:25 qunet/plots.py
--rw-rw-rw-  2.0 fat    25071 b- defN 23-Apr-22 17:10 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13314 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/RECORD
-12 files, 103592 bytes uncompressed, 29167 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    26998 b- defN 23-Apr-23 11:26 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13877 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-23 11:32 QuNet-0.0.9.dist-info/RECORD
+12 files, 105969 bytes uncompressed, 29845 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.8.dist-info/LICENSE
+Filename: QuNet-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.8.dist-info/METADATA
+Filename: QuNet-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.8.dist-info/WHEEL
+Filename: QuNet-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.8.dist-info/top_level.txt
+Filename: QuNet-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.8.dist-info/RECORD
+Filename: QuNet-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/models.py

```diff
@@ -94,22 +94,22 @@
 class CNN(nn.Module):
     """
     Свёрточная сеть: (B, C, H, W) ->  (B, C', H', W')
     """
     def __init__(self, cfg) -> None:
         super().__init__()
         self.cfg = {
-            'input'    : (1, 64, 64),   # входной тензор: (channels, height, width)
-            'output'   : None,          # выходной тензор устанавливает create()
-            'channel'  : [16,32,64],    # число каналов в каждом слое
-            'kernel'   : [3,3,3],       # int or list: размеры конволюционного ядра
-            'stride'   : 1,             # int or list: шаг конволюционного ядра
-            'padding'  : 1,             # int or list: забивка вокруг картинки
-            'pool_ker' : 2,             # int or list: ядро max-пулинга
-            'pool_str' : 2,             # int or list: шаг max-пулинга
+            'input'    : (1, 64, 64),   # input tensor shape:: (channels, height, width)
+            'output'   : None,          # output tensor shape;  sets in create()
+            'channel'  : [16,32,64],    # number of channels in each layer
+            'kernel'   : [3,3,3],       # int or list: size of the convolutional kernel
+            'stride'   : 1,             # int or list: stride of the convolutional kernel
+            'padding'  : 1,             # int or list: padding around the image
+            'pool_ker' : 2,             # int or list: max-pooling kernel
+            'pool_str' : 2,             # int or list: stride of max-pooling kernel
             'drop'     : 0,             # int or list: dropout после каждого слоя            
         }
         if type(cfg) is dict:           # добавляем, меняем свойства
             self.cfg.update(copy.deepcopy(cfg))
         cfg = self.cfg
 
         n = len(cfg['channel'])
```

## qunet/trainer.py

```diff
@@ -149,25 +149,66 @@
             if sch.enable:
                 sch.step(samples_trn)
                 self.scheduler = sch
                 break
 
     #---------------------------------------------------------------------------
 
-    def to_device(self, X):
-        if type(X) is list or type(X) is tuple:
-            for i in range(len(X)):
-                X[i] = X[i].to(self.device)
+    def to_device(self, batch):
+        """ send mini-batch to device """        
+        if torch.is_tensor(batch):
+            return batch.to(self.device)
+        batch = list(batch)        
+        for i in range(len(batch)):
+            batch[i] = self.to_device(batch[i])
+        return batch
+
+    #---------------------------------------------------------------------------
+
+    def get_fun_step(self, model, train):
+        """ Получить функцию шага тренировки или dfkblfwbb """
+        fun_step = None
+        if train: 
+            if hasattr(model, "training_step"):            
+                fun_step = model.training_step
         else:
-            X = X.to(self.device)
-        return X
+            if hasattr(model, "validation_step"):            
+                fun_step = model.validation_step
+            elif hasattr(model, "training_step"):            
+                fun_step = model.training_step
+
+        assert fun_step is not None, "model must has training_step function"
+        return fun_step
+
+    #---------------------------------------------------------------------------
+
+    def get_metrics(self, step):
+        """ из результатов шага обучения вделить ишибку и метрику"""
+        if torch.is_tensor(step):
+            loss   = step
+            scores = None
+        elif type(step) is dict:
+            loss  = step.get('loss')
+            scores = step.get('score')
+        if torch.is_tensor(scores) and scores.ndim == 1:
+            scores = scores.view(-1,1)
+        return loss, scores
 
     #---------------------------------------------------------------------------
 
-    def fit(self, epoch, model, data,  train=True, accumulate=1, verbose=1):
+    def samples_in_batch(self, batch):
+        """ сколько примров в батче """
+        if torch.is_tensor(batch):
+            return len(batch)
+        if type(batch) is list or type(batch) is tuple:
+            return self.samples_in_batch(batch[0]) 
+        assert False, "wrong type of the fist element in batch"
+    #---------------------------------------------------------------------------
+
+    def fit_epoch(self, epoch, model, data,  train=True, accumulate=1, verbose=1):
         """
         Args:
             * train      - True: режим тренировки, иначе валидации
             * accumulate - аккумулировать градиент для стольки батчей перед сдвигом оптимизатора;
                            используем, когда большой батч или граф не помещаются в GPU
         https://pytorch.org/blog/what-every-user-should-know-about-mixed-precision-training-in-pytorch/
         """
@@ -176,55 +217,58 @@
 
         scaler = None
         if torch.cuda.is_available() and self.dtype != torch.float32:
             scaler = torch.cuda.amp.GradScaler()
 
         if train:
             self.optim.zero_grad()                  # обнуляем градиенты
+        
+        fun_step = self.get_fun_step(model, train)  # функция шага тренировки или валидации           
 
         samples, steps, beg, lst = 0, 0, time.time(), time.time()
         counts_all, losses_all,  scores_all = torch.empty(0,1), None,  None
-        for b, (x, y_true) in enumerate(data):
-            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
-            x, y_true = self.to_device(x), self.to_device(y_true)
+        for batch_id, batch in enumerate(data):    
+            num   = self.samples_in_batch(batch)
+            batch = self.to_device(batch)            
 
             if scaler is None:
-                y_pred = model(x)
-                loss, scores = model.metrics(x, y_pred, y_true)
+                step = fun_step(batch, batch_id)                
             else:
                 with torch.autocast(device_type=self.device, dtype=self.dtype):
-                    y_pred = model(x)
-                    loss, scores = model.metrics(x, y_pred, y_true)
-
+                    step = fun_step(batch, batch_id)
+            loss, scores = self.get_metrics(step)
+                
             if train:
                 if scaler is None:
                     loss.backward()   # вычисляем градиенты
                 else:
                     scaler.scale(loss).backward()   # вычисляем градиенты
-                if (b+1) % accumulate == 0:
+                if (batch_id+1) % accumulate == 0:
                     if scaler is None:
                         self.optim.step()
                     else:
                         scaler.step(self.optim)     # подправляем параметры
                         scaler.update()             # Updates the scale for next iteration
                     self.optim.zero_grad()          # обнуляем градиенты
                     steps      += 1                 # шагов за эпоху
                     self.hist['steps'] += 1         # шагов за всё время
                 self.hist['samples'] += num         #  примеров за всё время
 
             samples += num                          # просмотренных примеров за эпоху
             losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
             if scores is not None:
-                scores = scores.detach().mean(dim=0)
+                scores = scores.detach()
+                assert scores.ndim == 2, f"model must has tensor score in function metrics with dim==2, but got {scores.ndim}"
+                scores = scores.mean(dim=0)
                 scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
             counts_all = torch.vstack([counts_all, torch.Tensor([num])])
 
-            if verbose and (time.time()-lst > 1 or b+1 == len(data) ):
+            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
                 lst = time.time()
-                self.fit_progress(epoch, train, (b+1)/len(data),
+                self.fit_progress(epoch, train, (batch_id+1)/len(data),
                                   losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
 
         if train: self.hist['time_trn'] += (time.time()-beg)
         else:     self.hist['time_val'] += (time.time()-beg)
 
         if scores_all is not None:
             scores_all = scores_all.cpu()
@@ -276,49 +320,44 @@
         """
         Вычислить предсказание, ошибку и метрику для каждого примера в data        
         """
         self.model.train(False)          # режим тестирование
         torch.set_grad_enabled(False)    # вычислительный граф не строим
         data.whole = whole               # обычно по всем примерам (и по дробному батчу)
 
-        samples, beg, lst = 0, time.time(), time.time()
-        scores_all, output_all = None, None
+        assert hasattr(model, "predict_step"), "for method predict model must has method predict_step, witch return output tensor"
 
         scaler = None
         if torch.cuda.is_available() and self.dtype != torch.float32:
             scaler = torch.cuda.amp.GradScaler()
-        for b, (x, y_true) in enumerate(data):
-            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
-            x, y_true = self.to_device(x), self.to_device(y_true)
+
+        samples, beg, lst = 0, time.time(), time.time()
+        output_all = None        
+        for batch_id, batch in enumerate(data):
+            num   = self.samples_in_batch(batch)
+            batch = self.to_device(batch)            
 
             if scaler is None:
-                y_pred = model(x)
-                _, scores = model.metrics(x, y_pred, y_true)
+                y_pred = model.predict_step(batch, batch_id)                                
             else:
                 with torch.autocast(device_type=self.device, dtype=self.dtype):
-                    y_pred = model(x)
-                    _, scores = model.metrics(x, y_pred, y_true)
-
+                    y_pred = model.predict_step(batch, batch_id)                    
+            
             samples += num                      # число просмотренных примеров за эпоху            
-            if scores is not None:
-                scores = scores.detach()
-                scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])            
             output_all = y_pred.detach() if output_all is None else torch.vstack([output_all, y_pred.detach() ])            
 
-            if verbose and (time.time()-lst > 1 or b+1 == len(data) ):
+            if verbose and (time.time()-lst > 1 or batch_id+1 == len(data) ):
                 lst = time.time()
-                print(f"\r[{100*(b+1)/len(data):3.0f}%]", end=" ")                
+                print(f"\r[{100*(batch_id+1)/len(data):3.0f}%]  {(time.time()-beg)/60:.2f}m", end=" ")                
 
-        if scores is not None:
-            scores_all = scores_all.cpu()
-        return output_all.cpu(),  scores_all
+        return output_all.cpu()
 
     #---------------------------------------------------------------------------
 
-    def run(self,  epochs =None,  samples=None,            
+    def fit(self,  epochs =None,  samples=None,            
             pre_val:bool=False, period_val:int=1, period_plot:int=100,         
             period_checks:int=1, period_val_beg:int = 4, samples_beg:int = None,
             period_call:int = 0, callback = None): 
         """
         Args:
             * epochs               - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
             * samples              - if defined, then will stop after this number of samples, even if epochs has not ended
@@ -331,23 +370,23 @@
             * period_val_beg = 4   - validation period on the first samples_beg examples
             * samples_beg = None   - the number of samples from the start, after which the validation period will be equal to period_val.
         """
         assert self.optim is not None, "Define the optimizer first"
         self.set_optim_schedulers()        
         self.model.to(self.device)
         if pre_val:
-            losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit(0, self.model, self.data_val, train=False)
+            losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit_epoch(0, self.model, self.data_val, train=False)
             loss_val, score_val = self.mean(losses, scores, counts)
             self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
             print()
 
         epochs = epochs or 1_000_000
         #for epoch in tqdm(range(1, epochs+1)):
         for epoch in range(1, epochs+1):
-            losses, scores, counts, (samples_trn,steps_trn,tm_trn) = self.fit(epoch, self.model, self.data_trn, train=True)
+            losses, scores, counts, (samples_trn,steps_trn,tm_trn) = self.fit_epoch(epoch, self.model, self.data_trn, train=True)
             loss_trn, score_trn = self.mean(losses, scores, counts)
             lr = self.scheduler.get_lr()
             self.add_hist(self.hist['trn'], self.data_trn.batch_size, samples_trn, steps_trn, tm_trn, loss_trn, score_trn, lr)
 
             if self.hist['best']['loss_trn'] is None or self.hist['best']['loss_trn'] > loss_trn:
                 self.hist['best']['loss_trn'] = loss_trn
                 self.hist['best']['samples_loss_trn'] = self.hist['samples']
@@ -356,15 +395,15 @@
             if self.best_score(self.hist['best']['score_trn'], score_trn):            
                 self.hist['best']['score_trn'] = score_trn[0]
                 self.hist['best']['samples_score_trn'] = self.hist['samples']
                 self.hist['trn']['best_score'].append((self.hist['samples'], self.hist['steps'], score_trn[0].item()))
 
             period = period_val_beg if samples_beg and  self.hist['samples'] < samples_beg else period_val
             if  (period and epoch % period == 0) or epoch == epochs:
-                losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit(epoch, self.model, self.data_val, train=False)
+                losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit_epoch(epoch, self.model, self.data_val, train=False)
                 loss_val, score_val = self.mean(losses, scores, counts)
                 self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
 
                 # save best validation loss:
                 if self.hist['best']['loss_val'] is None or self.hist['best']['loss_val'] > loss_val:
                     self.hist['best']['loss_val'] = loss_val
                     self.hist['best']['samples_loss_val'] = self.hist['samples']
```

## Comparing `QuNet-0.0.8.dist-info/LICENSE` & `QuNet-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.8.dist-info/METADATA` & `QuNet-0.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.8
+Version: 0.0.9
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -45,49 +45,53 @@
 
 # 2. create trainer, optimizer and scheduler (if need)                                               
 tariner = Trainer(model, data_trn)    
 trainer.set_optimizer( torch.optim.SGD(model.parameters(), lr=1e-2) )
 trainer.set_scheduler( ExpScheduler(lr1=1e-5, lr2=1e-4, samples=100e3) )
 
 # 3. run training
-trainer.run(epochs=100, period_plot=5)
+trainer.fit(epochs=100, period_plot=5)
 ```
 
 <hr>
 
 ## Model
 
-Model must be a class (successor of nn.Module) with methods:
-* The `forward` function takes input `x` and returns output `y`.
-These can be tensors or tuples (lists) of tensors.
-* The `metrics` function takes  `(x, y_true, y_pred)` and returns the model's scalar loss and tensor quality metric: 
- `(B,1)` for one metric (accuracy, for example) or `(B,n)` for n quality metrics.
+Model must be a class (successor of nn.Module) with functions:
+
+* `forward(x)` function takes input `x` and returns output `y`. 
+This function is not used directly by the coach and usually contains a description of the model.
+* `training_step(batch, batch_id)` - called by the trainer during the training phase. 
+Should return a scalar loss (with computational graph).
+It can also return a dictionary like `{"loss": scalar, "score": tensor}`, where score is a quality metric.
+* `validation_step(batch, batch_id)` - similarly called at the model validation stage.
+If it does the same calculations as `training_step`, it can be omitted.
 
 For example, for 1D linear regression  $y=f(x)$ with mse-loss and metric as |y_pred-y_true|, model looks like:
 ```python
 class Model(nn.Module):
-    def __init__(self):        
+    def __init__(self):      
+        """ Creating Model Parameters """  
         super().__init__() 
         self.fc = nn.Linear( 1, 1 )
 
     def forward(self, x):                            # (B,1)
+        """ Defining Model Calculations """
         return self.fc(x)                            # (B,1)
 
-    def metrics(self, x, y_pred, y_true)             # (B,1) (B,1)  (B,1)        
-        loss   = (y_pred - y_true).pow(2).mean()     # ()     scalar!
-        errors = torch.abs(y_pred.detach()-y_true)   # (B,1)  one metric
-        return loss, errors                          # ()  (B,1)
+    def training_step(self, batch, batch_id):
+        """ Called by the trainer during the training step """
+        x, y_pred = batch                            # the model knows the minbatch format
+        y_true = self(x)                             # (B,1)  forward function call
+        loss   = (y_pred - y_true).pow(2).mean()     # ()     loss for optimization (scalar)!        
+        errors = torch.abs(y_pred.detach()-y_true)   # (B,1)  errors for each sample (one metric)
+        return {'loss':loss, 'score': errors}        # if there is no score, you can simply return loss
 ```
+As we can see, the model description interface is the same as the library interface <a href="https://lightning.ai/">Pytorch Lightning</a>
 
-**Attention**: If the output of the model is one, after the Linear layer the tensor has the shape (B,1).
-Therefore, the target data must also have the form (B,1), otherwise we will get an incorrect loss.
-```python
-X,Y = torch.arange(5).view(-1,1).to(torch.float32),  torch.arange(5).to(torch.float32)
-loss = (X-Y).pow(2).mean()  # 4 С‚Р°Рє РєР°Рє (B,1) - (B,) = (B,1) - (1,B) = (B,B)
-```
 <hr>
 
 ## Data
 
 The `Data` - training or validation data class. It can be overridden or pytorch DataLoader can be used.
 Iterator `__next__` of the `Data`  must return an `X,Y` tuple, where:
 * X - tensor or tuple (list) of tensors for model input,
@@ -124,28 +128,28 @@
 
 You can also use the standard DataLoader with Trainer:
 ```python
 from torchvision            import datasets
 from torchvision.transforms import ToTensor 
 from torch.utils.data       import DataLoader
 
-mnist = datasets.MNIST(root='data', train=True,  transform=ToTensor(), download=True)
-data_trn  = DataLoader(dataset=mnist, batch_size=1024, shuffle=True)
+mnist    = datasets.MNIST(root='data', train=True,  transform=ToTensor(), download=True)
+data_trn = DataLoader(dataset=mnist, batch_size=1024, shuffle=True)
 ```
 <hr>
 
 ## Trainer
 
 The Trainer is given the model, training and validation data.
 Using the `set_optimizer` function, the optimizer is set.
-After that, the function `run` is called:
+After that, the function `fit` is called:
 ```python
 trainer = Trainer(model, data_trn, data_val)
 trainer.set_optimizer( torch.optim.SGD(model.parameters(), lr=1e-2) )
-trainer.run(epochs=100, pre_val=True, period_plot=10)
+trainer.fit(epochs=100, pre_val=True, period_plot=10)
 ```
 You can add different training schedulers, customize the output of training graphs, manage the storage of the best models and checkpoints, and much more.
 
 ```python
 trainer = Trainer(model, data_trn, data_val, device=None, dtype=torch.float32, score_max=False)
 ```
 
@@ -154,15 +158,15 @@
 * `data_val`  - data for validation (instance of Data or DataLoader); may be missing;
 * `score_max` - consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).
 
 Other properties of `Trainer` allow you to customize the appearance of graphs, save models, manage training, and so on.
 They will be discussed in the relevant sections.
 
 ```python
-trainer.run(epochs =None,  samples=None,            
+trainer.fit(epochs =None,  samples=None,            
             pre_val=False, period_val=1, period_plot=100,         
             period_checks=1, period_val_beg = 4, samples_beg = None,
             period_call:int = 0, callback = None):     
 ```
 
 * `epochs`         - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
 * `samples`        - if defined, then training will stop after this number of samples, even if epochs has not ended
@@ -261,15 +265,15 @@
 trainer.copy_best_loss_model  = True  # to copy the best model by val loss
 ```
 These models can be used to roll back if something went wrong (similarly for `trainer.best_loss_model`):
 ```python
 train.model = copy.deepcopy(trainer.best_score_model)   
 ```
 
-If the following folder is defined (by default `None`), then the best model by validation loss, score will be saved on disk and intermediate versions of the model will be saved with the period `period_checks` (argument of `run` function).
+If the following folder is defined (by default `None`), then the best model by validation loss, score will be saved on disk and intermediate versions of the model will be saved with the period `period_checks` (argument of `fit` function).
 ```python
 trainer.folder_loss   = "models/best_loss"   # folder to save the best val loss models
 trainer.folder_score  = "models/best_score"  # folder to save the best val score models
 trainer.folder_checks = "models/checkpoints" # folder to save checkpoints        
 ```
 The best score is the metric of the first column of the second return tensor in the metrics function of the model.
 If `trainer.score_max=True`, then the higher the score, the better (for example, accuracy).
@@ -286,18 +290,21 @@
 
 ## Model State Visualization
 
 <hr>
 
 ## Examples
 
-* Regression_1D - visualization of changes in model parameters
 * <a href="https://colab.research.google.com/drive/179sHb3WyHNrSJKGLfKrXaAzvShmS1SSf?usp=sharing">Interpolation_F(x)</a> - interpolation of a function of one variable (example of setting up a training plot; working with the list of schedulers; adding a custom graph)
-* MNIST - recognition of handwritten digits 0-9
+* <a href="https://colab.research.google.com/drive/1N4b6mwUvH-o-t6VIiuhq7FMuGRabdOm0?usp=sharing">MNIST</a> - recognition of handwritten digits 0-9 (example using pytorch DataLoader, classification task)
+
+* CIFAR  (agumantation)
+
 * Vanishing gradient
+* Regression_1D - visualization of changes in model parameters
 
 <hr>
 
 ## Versions
 
 * 0.0.4 - fixed version for competition IceCube (kaggle)
```

## Comparing `QuNet-0.0.8.dist-info/RECORD` & `QuNet-0.0.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 qunet/__init__.py,sha256=IVocm0vQvQK-MkJmbU_qmmZi6dyccdcqjlLG1FUx7TU,123
 qunet/data.py,sha256=mMVzzTlLC7iwhlyyeAdAxCh0qsmjtkD9BMqNK5ptF98,6484
-qunet/models.py,sha256=bcgxYfqWQHhHRQGURTghGhm2c1fjMcgRiI9Sq_uR5D0,22012
+qunet/models.py,sha256=7-Eun8YQ_jwFFDsBBjLseNyPFDN_TUHqlGBG6mzg3Cg,21899
 qunet/old.py,sha256=wfsu9d4vcptlBT1lgPKHCfqDm8lirDvTTvEEzKGjTig,16977
 qunet/optim.py,sha256=jhoIhpjX9YzEneGc8uUelIdsLidBQgaAmO43Vqz59Xo,10435
 qunet/plots.py,sha256=83OWCZkri0cR_BGvZQVcdcdTtuyGsHR_OC45Oz3DMLM,7131
-qunet/trainer.py,sha256=ytx3hFQ_SpAq0jh6IZD4W5T3VwoSATRU9lfGrfXY5vA,25071
-QuNet-0.0.8.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
-QuNet-0.0.8.dist-info/METADATA,sha256=VQE-7hjvQ6OrZwQlDGhLadlcS52cX3mnFucHED_0bOc,13314
-QuNet-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.8.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.8.dist-info/RECORD,,
+qunet/trainer.py,sha256=3P6RFyjQkSWvtiN0Qm-dIBZXlDIMQYjpWLoW3USqirY,26998
+QuNet-0.0.9.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
+QuNet-0.0.9.dist-info/METADATA,sha256=WCiiflll9RDlLEIVuSE63Y3Sj4q1jVrrUhahuI_N0fk,13877
+QuNet-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.9.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.9.dist-info/RECORD,,
```

