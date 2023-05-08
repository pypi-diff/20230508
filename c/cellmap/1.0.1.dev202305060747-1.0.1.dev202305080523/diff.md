# Comparing `tmp/cellmap-1.0.1.dev202305060747-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202305080523-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19769 bytes, number of entries: 5
+Zip file size: 19725 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   112785 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305060747.dist-info/RECORD
-5 files, 115199 bytes uncompressed, 19015 bytes compressed:  83.5%
+-rw-r--r--  2.0 unx   112613 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202305080523.dist-info/RECORD
+5 files, 115027 bytes uncompressed, 18971 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060747.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202305080523.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060747.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202305080523.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202305060747.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202305080523.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -304,20 +304,14 @@
     
     ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
     idx_bd_  = []
     if graph_method == 'Delauney':
         source, target, idx_bd_ = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,cut_std=cut_std,return_type='edges_bd')
     elif graph_method == 'knn':
-        # pca = sklearn.decomposition.PCA()
-        # exp_HD_pca = pca.fit_transform(exp_HD)
-        # n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate_pca])
-        # knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
-        # knn.fit(exp_HD_pca[:,:n_pca])
-        # distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
@@ -346,57 +340,63 @@
     rot_flow_ = edge_vel - pot_flow_
     adata.obs[potential_key] = potential - np.min(potential)
 
 
     # Compute potential & rotational flow
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
     vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
-    src_trg_ = np.hstack((source,target))
-    trg_src_ = np.hstack((target,source))
-    pot_flow_2_ = np.hstack((pot_flow_,-pot_flow_))
-    rot_flow_2_ = np.hstack((rot_flow_,-rot_flow_))
     edge_vel_norm = np.linalg.norm(edge_velocity(exp_LD,vel_LD,source,target,normalization=False))
-    # if graph_method == 'Delauney':
-    for i in range(adata.shape[0]):
-        idx_ = src_trg_ == i
-        # ex_s = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]])/np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],ord=2)
-        # vel_potential[i] = 2.*edge_vel_norm*np.mean(pot_flow_2_[idx_]*ex_s.T,axis=1)
-        # vel_rotation[i]  = 2.*edge_vel_norm*np.mean(rot_flow_2_[idx_]*ex_s.T,axis=1)
-        dis_ = np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],axis=1,ord=2)
-        dis_[dis_==0] = 1
-        ex_ = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]]).T/dis_
-        vel_potential[i] = 4.*edge_vel_norm*np.mean(pot_flow_2_[idx_]*ex_,axis=1)
-        vel_rotation[i]  = 4.*edge_vel_norm*np.mean(rot_flow_2_[idx_]*ex_,axis=1)
-    adata.obsm[pot_vkey_] = vel_potential
-    adata.obsm[rot_vkey_] = vel_rotation
-    # elif graph_method == 'knn':
-    #     knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
-    #     knn.fit(exp_LD)
-    #     distances, indices = knn.kneighbors(exp_LD)
-    #     distances, indices = distances[:,1:], indices[:,1:]
-    #     for i in range(adata.shape[0]):
-    #         ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
-    #         vel_potential[i] = -4.*edge_vel_norm*np.mean((pot_flow_[indices[i]]-pot_flow_[i])*ex_s.T,axis=1)
-    #         vel_rotation[i]  = -4.*edge_vel_norm*np.mean((rot_flow_[indices[i]]-rot_flow_[i])*ex_s.T,axis=1)
-    #     adata.obsm[pot_vkey_] = vel_potential
-    #     adata.obsm[rot_vkey_] = vel_rotation
+    if graph_method == 'Delauney':
+        src_trg_ = np.hstack((source,target))
+        trg_src_ = np.hstack((target,source))
+        pot_flow_2_ = np.hstack((pot_flow_,-pot_flow_))
+        rot_flow_2_ = np.hstack((rot_flow_,-rot_flow_))
+        for i in range(adata.shape[0]):
+            idx_ = src_trg_ == i
+            dis_ = np.linalg.norm(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]],axis=1,ord=2)
+            dis_[dis_==0] = 1
+            ex_ = -(exp_LD[src_trg_[idx_]]-exp_LD[trg_src_[idx_]]).T/dis_
+            vel_potential[i] = 4.*edge_vel_norm*np.mean(pot_flow_2_[idx_]*ex_,axis=1)
+            vel_rotation[i]  = 4.*edge_vel_norm*np.mean(rot_flow_2_[idx_]*ex_,axis=1)
+        adata.obsm[pot_vkey_] = vel_potential
+        adata.obsm[rot_vkey_] = vel_rotation
+    elif graph_method == 'knn':
+        for i in range(adata.shape[0]):
+            idx_ = source == i
+            dis_ = np.linalg.norm(exp_LD[source[idx_]]-exp_LD[target[idx_]],axis=1,ord=2)
+            dis_[dis_==0] = 1
+            ex_ = -(exp_LD[source[idx_]]-exp_LD[target[idx_]]).T/dis_
+            vel_potential[i] = 4.*edge_vel_norm*np.mean(pot_flow_[idx_]*ex_,axis=1)
+            vel_rotation[i]  = 4.*edge_vel_norm*np.mean(rot_flow_[idx_]*ex_,axis=1)
+        adata.obsm[pot_vkey_] = vel_potential
+        adata.obsm[rot_vkey_] = vel_rotation
+    
     
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
+    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target,normalization=False))
+    div_ = np.linalg.norm(vel_LD,axis=1)
+    div_[div_==0] = 1
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1]/div_,-vel_LD[:,0]/div_)).T,source,target,normalization=False))
     source_term_ = vorticity_
     streamfunc_ = -np.dot(lap_inv_,source_term_)
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = streamfunc_-np.min(streamfunc_)
 
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
+    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target,normalization=False))
+    div_ = np.linalg.norm(adata.obsm[pot_vkey_],axis=1)
+    div_[div_==0] = 1
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1]/div_,-adata.obsm[pot_vkey_][:,0]/div_)).T,source,target,normalization=False))
     source_term_ = vorticity_
     streamfunc_ = -np.dot(lap_inv_,source_term_)
     adata.obs[pot_vor_key_] = vorticity_
     adata.obs[pot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
-    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
+    # vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target,normalization=False))
+    div_ = np.linalg.norm(adata.obsm[rot_vkey_],axis=1)
+    div_[div_==0] = 1
+    vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1]/div_,-adata.obsm[rot_vkey_][:,0]/div_)).T,source,target,normalization=False))
     source_term_ = vorticity_
     streamfunc_ = -np.dot(lap_inv_,source_term_)
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = streamfunc_-np.min(streamfunc_)
 
     adata.obs[rotation_key] = np.array([np.mean(np.hstack((rot_flow_[source==i],-rot_flow_[target==i]))) for i in range(adata.shape[0])])
```

## Comparing `cellmap-1.0.1.dev202305060747.dist-info/METADATA` & `cellmap-1.0.1.dev202305080523.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202305060747
+Version: 1.0.1.dev202305080523
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

