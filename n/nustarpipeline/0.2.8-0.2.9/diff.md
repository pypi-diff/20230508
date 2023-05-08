# Comparing `tmp/nustarpipeline-0.2.8.tar.gz` & `tmp/nustarpipeline-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nustarpipeline-0.2.8.tar", last modified: Tue May  2 11:46:51 2023, max compression
+gzip compressed data, was "nustarpipeline-0.2.9.tar", last modified: Mon May  8 17:46:01 2023, max compression
```

## Comparing `nustarpipeline-0.2.8.tar` & `nustarpipeline-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 11:46:51.800469 nustarpipeline-0.2.8/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.8/LICENSE
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-02 11:46:51.800469 nustarpipeline-0.2.8/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.8/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 11:46:51.800469 nustarpipeline-0.2.8/nustarpipeline/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.8/nustarpipeline/__init__.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.8/nustarpipeline/process.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    90286 2023-05-02 11:32:43.000000 nustarpipeline-0.2.8/nustarpipeline/utils.py
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 11:46:51.800469 nustarpipeline-0.2.8/nustarpipeline.egg-info/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/entry_points.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      107 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/requires.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-05-02 11:46:51.000000 nustarpipeline-0.2.8/nustarpipeline.egg-info/top_level.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1548 2023-05-02 11:46:51.800469 nustarpipeline-0.2.8/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-05-02 11:38:01.000000 nustarpipeline-0.2.8/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-08 17:46:01.643889 nustarpipeline-0.2.9/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.9/LICENSE
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-08 17:46:01.643889 nustarpipeline-0.2.9/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.9/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-08 17:46:01.639889 nustarpipeline-0.2.9/nustarpipeline/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.9/nustarpipeline/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.9/nustarpipeline/process.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    97269 2023-05-08 17:26:45.000000 nustarpipeline-0.2.9/nustarpipeline/utils.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-08 17:46:01.643889 nustarpipeline-0.2.9/nustarpipeline.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      121 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-05-08 17:46:01.000000 nustarpipeline-0.2.9/nustarpipeline.egg-info/top_level.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1563 2023-05-08 17:46:01.643889 nustarpipeline-0.2.9/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-05-08 17:45:46.000000 nustarpipeline-0.2.9/setup.py
```

### Comparing `nustarpipeline-0.2.8/LICENSE` & `nustarpipeline-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.8/PKG-INFO` & `nustarpipeline-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.8
+Version: 0.2.9
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.8/README.md` & `nustarpipeline-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.8/nustarpipeline/process.py` & `nustarpipeline-0.2.9/nustarpipeline/process.py`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.8/nustarpipeline/utils.py` & `nustarpipeline-0.2.9/nustarpipeline/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -891,117 +891,124 @@
     """
     logger.debug('remember PF is a factor  of about 1.4 the other PFs')
     a0 = 0
     if background is not None and background_error is not None:
         a0 = subtract_background(a0, background,background_error)
     return np.sum((c - a0 ) - (np.min(c - a0) ) ) / np.sum( c-a0 )
 
-def pulse_fraction_from_data_rms(counts, counts_err, n_harm=-1, background=None, background_error=None, plot=False, label='', verbose=False):
-    
-    """pulsed fractio computation from fixed number of harmonics
-        following Archibald et al (2014) that uses de Jager et al. (1986)
-        we use and optimal number of harmonics, from Archibald et al. (2014), ppendix A
+def compute_a_b_sigma_a_sigma_b(counts, counts_err, K):
+    """auxiliary function for Pf method by Archibald 2014 (and others)
+
     Args:
-        counts (_type_): pulse profile
-        counts_err (_type_): pulse profile uncertainty
-        n_harm (int, optional): number of used harmonics. If <=0, it determines the optimal number. default -1
+        counts (numpy array): the pulse profile
+        counts_err (numpy array): the pulse profile uncertainties
+        K (int): number of harmonics
 
     Returns:
-        numppy double: pulsed fraction
-    """
-    from matplotlib import cm
-    a0 = np.mean(counts)
-
+        a, b, sigma_a, sigma_b (numpy arrays): these vectors
+    """    
     N = np.size(counts)
-    K = n_harm
-    if n_harm <= 0:
-        K = int(N/2)
-
     A = np.zeros(K)
     B = np.zeros(K)
-
     a = np.zeros(K)
     b = np.zeros(K)
     sigma_a = np.zeros(K)
     sigma_b = np.zeros(K)
-
-    k = 0
-    while k < K:
-        L = np.zeros(N)
-        M = np.zeros(N)
-        P = np.zeros(N)
-        O = np.zeros(N)
-        # print('K=',k+1)
-        for i in range(0, N):
-            # print('aaaah: ',k,i)
-            argsinus = (2 * np.pi * (k + 1) * (i + 1)) / N
-            # print('argsin di '+str(k+1),' '+str(i+1)+' :',argsinus)
-            L[i] = counts[i] * np.cos(argsinus)
-            # print(L)
-            # print('L: ',L[i])
-            M[i] = counts[i] * np.sin(argsinus)
-            # print('M: ',M[i])
-            P[i] = counts_err[i] ** 2 * np.cos(argsinus) ** 2
-            O[i] = counts_err[i] ** 2 * np.sin(argsinus) ** 2
-            #
+    
+    for k in range(K):
+        
+        argsinus = (2 * np.pi * (k + 1) * np.arange(1,N+1, dtype=float)) / N
+        
+        L = counts * np.cos(argsinus)
+        
+        M = counts * np.sin(argsinus)
+        
+        P = counts_err ** 2 * np.cos(argsinus) ** 2
+        O = counts_err ** 2 * np.sin(argsinus) ** 2
+        #
         A[k] = np.sum(L)
-        # print('A:',A[k])
+        
         B[k] = np.sum(M)
-        # print('B: ',B)
+        
         SIGMA_A = np.sum(P)
         SIGMA_B = np.sum(O)
         #
-        a[k] = (1. / N) * A[k]
-        # print(a[k])
-        b[k] = (1. / N) * B[k]
-        sigma_a[k] = (1. / (N ** 2)) * SIGMA_A
-        sigma_b[k] = (1. / (N ** 2)) * SIGMA_B
-        k = k + 1
-
-    if n_harm <=0:
-        m4 = 4*np.arange(1,K+1)
-        cumulative_sum = np.zeros(K)
-        for k in range(1,K):
-            cumulative_sum[k] = np.sum( (a[0:k]/sigma_a[0:k])**2 + (b[0:k]/sigma_b[0:k])**2)
-        #print(cumulative_sum)
-        max_harm = np.argmax(cumulative_sum - m4)+1
-        #print("We stop at %d harmonics" % max_harm)
+        a[k] = A[k] / N
+        
+        b[k] = B[k] / N
+        sigma_a[k] =  SIGMA_A / N**2
+        sigma_b[k] =  SIGMA_B / N**2
+
+    return a, b, sigma_a, sigma_b
+
+def pulse_fraction_from_data_rms(counts, counts_err, n_harm=-1, background=None, background_error=None, plot=False, label='', verbose=False,
+                                 statistics='cstat', level=0.1):
+    
+    """pulsed fractio computation
+        following Archibald et al (2014) that uses de Jager et al. (1986)
+    Args:
+        counts (_type_): pulse profile
+        counts_err (_type_): pulse profile uncertainty
+        n_harm (int, optional): number of used harmonics. If <=0, it determines the optimal number. default -1
+        :param level: minimum confidence level to stop number of harmonics (default 0.1, lower values give less harmonics)
+        :param n_harm: maximum number of harmonics to use (default -1 takes the size of pulse profile)
+        :param plot: plot the pulse profile
+        :param label: to save the plot with name "rms_`label`.pdf", if label=='' it does not save the plot
+        ;parma verbose (bool): if true it returns both pulsed_frac, n_harm, if false just the pulsed_frac
+        ;param background the vector of the background
+        ;param backgroun_error the uncertainty vector of the background        
+        statistics (str, optional) : the method to compute the optimal number of harmonics (chi2, cstat, archibald) de cstat, see the function get_n_harm
+
+
+    Returns:
+        numppy double: pulsed fraction
+    """
+    from matplotlib import cm
+
+    a0 = np.mean(counts)
+    N = np.size(counts)
+ 
+    if n_harm <= 0:
+        K = get_n_harm(counts, counts_err, n_harm_min=2, n_harm_max=-1, statistics=statistics, level=level)
+    elif n_harm > N/2:
+        K = int(N/2)
     else:
-        max_harm = n_harm
-    somma = a[0:max_harm] ** 2 + b[0:max_harm] ** 2
+        K = n_harm
+   
+    a, b, sigma_a, sigma_b = compute_a_b_sigma_a_sigma_b(counts, counts_err, K)
+
+    somma = a[0:K] ** 2 + b[0:K] ** 2
     # print(somma)
-    differenza = sigma_a[0:max_harm] ** 2 + sigma_b[0:max_harm] ** 2
+    differenza = sigma_a[0:K] ** 2 + sigma_b[0:K] ** 2
     bla = somma - differenza
     # print('diff: ',differenza)
     logger.debug('Pre background average %f' % a0)
     if background is not None and background_error is not None:
         a0 = subtract_background(a0, background, background_error)
     logger.debug('Post background average %f' % a0)
 
     PF_rms = np.sqrt(2 * sum(bla)) / a0
 
 
     col = cm.viridis(np.linspace(0, 1,int(500)))
     if plot:
         import matplotlib.pyplot as plt
         f = np.linspace(0, 1, int(N))
-        if n_harm > 1:
-            plt.errorbar(f, counts, yerr=counts_err, fmt='.',color=col[n_harm])
-            plt.plot(f, counts, linestyle='--', color=col[n_harm])
-        else:
-            plt.plot(np.arange(1,K+1), cumulative_sum - m4, color = col[max_harm])
-        #plt.text(0.4,120,str(n_harm)+'  harmonics',color = col[n_harm])
+        
+        plt.errorbar(f, counts, yerr=counts_err, fmt='.',color=col[K])
+        plt.plot(f, counts, linestyle='--', color=col[K])
+        #plt.text(0.4,120,str(K)+'  harmonics',color = col[K])
         plt.xlabel('Phase')
         plt.ylabel('Counts')
         #plt.legend()
         if label != '':
             plt.savefig('rms_%s.pdf' % label)
 
     if verbose:
-        return PF_rms, max_harm
+        return PF_rms, K
     else:
         return PF_rms
 
 def subtract_background(a0, background, background_error):
     """subtracts background from the average
 
     Args:
@@ -1020,19 +1027,22 @@
         background_level = np.sum(background[ind]/background_error[ind]**2) / np.sum(1./background_error[ind]**2)
         logger.debug('Background level %f' % background_level)
         a0_out = a0 - background_level
         if a0 == 0:
             a0_out = background_level
             logger.debug('continuum level is zero')
             #raise Exception
+    else:
+        a0_out = a0
+        logger.warning('Zero background level')
     return a0_out
 
 def get_pulsed_fraction(e_min, e_max, pp, dpp, method_calc_rms='adaptive', output_file=None, force_recompute=False):
     """ thi functions is made to be a wrapper of different 
-    methods to compute the pulsed fraction
+    methods to compute the pulsed fraction (it is incomplete)
 
     Args:
         e_min (_type_): _description_
         e_max (_type_): _description_
         pp (_type_): _description_
         dpp (_type_): _description_
         method_calc_rms (str, optional): _description_. Defaults to 'adaptive'.
@@ -1087,15 +1097,15 @@
 
 def elaborate_pulsed_fraction(ee_pulsed, dee_pulsed, pulsed_frac, dpulsed_frac, debug_plots=True, e1=10, e2=20, ylabel = 'PF',
                               stem='', poly_deg=[3, 3], title='', save_plot=True, e_threshold=0.3, 
                               division_derivative_order=2, max_n_high_lines = 2, forced_gaussian_centroids = [],
                               forced_gaussian_amplitudes = [],
                               forced_gaussian_sigmas = [],
                               y_lim=[0,1], 
-                              noFe=False):
+                              noFe=False, threshold_p_value=1e-4):
     """This function implements the logics to perform a fit of the pulsed fraction.
     It first interpolates the pulsed fraction with a spline to find extremes of the function.
     Then it performs a fit with a polynomial plus gaussians.
     The general idea is to split the pulsed fraction into two regions, based on the flex of the function.
     Then to fit the lower energy checking for a gaussian feature in correspondence of the iron line complex.
     Then we look for minima of the PF in the highe part and inet gussians. 
     If there are too may minima, we reduce them.
@@ -1108,15 +1118,16 @@
         dpulsed_frac (numpy array): pulsed fraction uncertainty
         debug_plots (bool, optional): plot the derivative and the fits. Defaults to True.
         e1 (int, optional): lower energy to search the flex in this interval. Defaults to 10.
         e2 (int, optional): lower energy to search the flex in this interval. Defaults to 20.
         ylabel (str) : label of the y axis. Default 'PF', first, second for amplitude of 1st and 2nd hamonics, respectively
         Note that if you put e1>=e2, we will use only one interval.
         stem (str, optional): a string in fron of output plot names. Defaults to ''.
-        poly_deg (int or list of int, optional): degree of the polynomial. Defaults to 3.
+        poly_deg (int or list of int, optional): degree of the polynomial. Defaults to 3. If <0, it inreases the value until a p-value of 
+                                                at least threshold_p_value is reached
         title (str, optional): title of the plots. Defaults to ''.
         save_plot (bool, optional): if plots should be saved Defaults to True.
         e_threshold (float, optional): if energies of PF minima differ in relative terms less than this values, they are reduced.
                                        ex.: if the algorithm finds minima at 32 and 35 keV, it retains only 32.
                                        This is used also as a range for the centroid search from (1-e_treshold)*e_centroid to 
                                        (1+e_treshold)*e_centroid Defaults to 0.3.
         division_derivative_order (int, optional): order of the derivative to search for the division, if 2 it searches a flex. Defaults to 2.
@@ -1124,14 +1135,15 @@
         forced_gaussian_centroids (list, optional): you can force the initial centroid energies with this parameter. Defaults to [].
         forced_gaussian_amplitudes (list, optional): you can force the initial amplitudes with this parameter, if the length of the list 
                                                     is different from the one of forced_gaussian_centroids, it is unused. Defaults to [].
         forced_gaussian_sigmas (list, optional): you can force the initial sigmas with this parameter, if the length of the list 
                                                  is different from the one of forced_gaussian_centroids, it is unused. Defaults to [].
         y_lim : limits for the plotting. Defaults to [0,1]
         noFe : exclude the 6.4 keV Gaussian feature, defaults to False
+        threshold_p_value : defaults to 1e-4 it is the threshold p-value above which the polynomial degree is acceptable
     Returns:
         two fitting objects for the two ranges (the output of utils.fit_pulsed_frac). if only one is used, the second is None.
      """    
     from scipy import interpolate
 
     if type(poly_deg) is not list:
         poly_deg = [poly_deg]
@@ -1233,15 +1245,16 @@
 
 
     pulsed_fit_low = fit_pulsed_frac(ee_pulsed[ind_low],dee_pulsed[ind_low], 
                                         pulsed_frac[ind_low], dpulsed_frac[ind_low], n_gauss=n_gauss, 
                                        center=center,
                                         sigma=sigma,
                                         amplitude=amplitude, ylabel = ylabel,
-                                       degree_pol=poly_deg[0], plot_final=True, stem=stem+'low', y_lim=y_lim)
+                                       degree_pol=poly_deg[0], plot_final=True, stem=stem+'low', y_lim=y_lim,
+                                       threshold_p_value=threshold_p_value)
 
     if make_double_fit:
 
         e_cyc = get_zeros(fake_en, smoothed_pulsed_frac_deriv, smoothed_pulsed_frac_deriv_2, fake_en>e_turn)
         
         if len(e_cyc)>1:
             logger.info("Checking for too close Gaussians in %d elements" % len(e_cyc))
@@ -1299,15 +1312,15 @@
         
         pulsed_fit_high = fit_pulsed_frac(ee_pulsed[ind_high],dee_pulsed[ind_high], 
                                             pulsed_frac[ind_high], dpulsed_frac[ind_high], n_gauss=n_gauss, 
                                         center=center,
                                             sigma=sigma,
                                             amplitude=amplitude,
                                         degree_pol=high_poly_deg, plot_final=True, stem=stem+'high',
-                                        y_lim=y_lim,ylabel = ylabel)
+                                        y_lim=y_lim,ylabel = ylabel, threshold_p_value=threshold_p_value)
     else:
         pulsed_fit_high = None
 
     
     from matplotlib.pyplot import cm
     comps_low = pulsed_fit_low.eval_components(x=ee_pulsed[ind_low])
     bb_low = (pulsed_frac[ind_low] - pulsed_fit_low.best_fit) / dpulsed_frac[ind_low]
@@ -1352,73 +1365,93 @@
     if save_plot:
         plt.savefig(stem + 'global_pulsed_fitted.pdf')
 
     return pulsed_fit_low, pulsed_fit_high, e_turn
 
 def fit_pulsed_frac(en, den, pf, dpf, stem=None, degree_pol=4, n_gauss=0, center=[],
                     sigma=[], amplitude=[],
-                    plot_final=True, ylabel = 'PF', print_results=True, y_lim=[0,1.1], x_lim=[3,70]):
+                    plot_final=True, ylabel = 'PF', print_results=True, y_lim=[0,1.1], x_lim=[3,70], threshold_p_value=1e-4):
     '''
     this function will fit an input energy range of the pulse profile.
     the fitting function will be a simple polynomial + gaussian
     the aim is to retrieve basic gaussian parameters to be compared
     to those obtained in spectral analysis around Ecycl.
      output files: 1. the fit result
                    2. the fit results to be plotted in a file
                    3. Figure in pdf
     :param en: input energy
     :param den: input energy uncertainty
     :param pf: pulsed fraction
     :param dpf: pulsed fractio uncertainty
     :param stem: output prefix
-    :param degree_pol: degree of the polynomial to fit
+    :param degree_pol: degree of the polynomial to fit. If <0, it inreases the value until a p-value of 
+                                                at least threshold_p_value is reached
     :param n_gauss: number of gaussian lines
     :param center: array of centers of gaussians [[initial_value, min, max]]
     :param sigma: array of sigmas of gaussians [[initial_value, min, max]]
     :param amplitude: array of amplitude of gaussians [[initial_value, min, max]],
                         use negative values for absorption-like
     :param plot_final: if make a final plot
     :param ylabel: ylabel for the plot (defaults to 'PF')
     :param print_results: if results should be printed out in file
+    ;param threshold_p_value: defaults to 1e-4 is the threshold p-value to stop increasing the number of polynomials
     :return:
     '''
     from matplotlib.pyplot import cm
     from lmfit.models import PolynomialModel, GaussianModel
+    from scipy.stats import chi2
 
     if len(center) != n_gauss or len(sigma) != n_gauss or len (amplitude) != n_gauss:
         logger.error("You provided %d centers, %d sigmas, and %d amplitudes for %d gaussians" % (len(center), 
                             len(sigma), len(amplitude), n_gauss))
         return
 
     col = cm.viridis(np.linspace(0, 1, 6))
 
     if stem is not None:
         outputfile = open(stem + '_fit_pf.out', 'w')
     else:
         stem = ''
         outputfile = open('fit_pf.out', 'w')
 
-    poly_mod = PolynomialModel(prefix='poly_', degree=degree_pol)
-    pars = poly_mod.guess(pf, x=en, degree=degree_pol)
-    mod = poly_mod
-
-    for N in range(1, n_gauss+1):
-        logger.debug("%d" % N)
-        logger.debug("%g" % center[N - 1][0])
-        gauss = GaussianModel(prefix='g' + str(N) + '_')
-        pars.update(gauss.make_params())
-        pars['g' + str(N) + '_center'].set(value=center[N - 1][0], min=center[N - 1][1], max=center[N - 1][2])
-        pars['g' + str(N) + '_sigma'].set(sigma[N - 1][0], min=sigma[N - 1][1], max=sigma[N - 1][2])
-        pars['g' + str(N) + '_amplitude'].set(amplitude[N - 1][0], min=amplitude[N - 1][1],
-                                               max=amplitude[N - 1][2])
-        mod = mod + gauss
+    if degree_pol > 0:
+        threshold_p_value = 1e-100
+        running_degree_pol = degree_pol
+    else:
+        running_degree_pol = 1
+    
+    p_value = 0
+
+    while p_value <= threshold_p_value:
+        poly_mod = PolynomialModel(prefix='poly_', degree=running_degree_pol)
+        pars = poly_mod.guess(pf, x=en, degree=running_degree_pol)
+        mod = poly_mod
+
+        for N in range(1, n_gauss+1):
+            logger.debug("%d" % N)
+            logger.debug("%g" % center[N - 1][0])
+            gauss = GaussianModel(prefix='g' + str(N) + '_')
+            pars.update(gauss.make_params())
+            pars['g' + str(N) + '_center'].set(value=center[N - 1][0], min=center[N - 1][1], max=center[N - 1][2])
+            pars['g' + str(N) + '_sigma'].set(sigma[N - 1][0], min=sigma[N - 1][1], max=sigma[N - 1][2])
+            pars['g' + str(N) + '_amplitude'].set(amplitude[N - 1][0], min=amplitude[N - 1][1],
+                                                max=amplitude[N - 1][2])
+            mod = mod + gauss
 
-    #initialfit = mod.eval(pars, x=en)
 
-    out = mod.fit(pf, pars, x=en, weights = 1./dpf)
+        
+        #initialfit = mod.eval(pars, x=en)
+
+        out = mod.fit(pf, pars, x=en, weights = 1./dpf)
+        p_value = 1 - chi2.cdf(x=out.chisqr, df = out.nfree)
+        logger.info('poly_deg %d chi2 %f dof %d p-value %f' % (running_degree_pol , out.chisqr, out.nfree, p_value))
+        running_degree_pol += 1
+        if running_degree_pol >7:
+            logger.info('Reached maximum polynomial degree')
+            break
 
     bb = (pf - out.best_fit) / dpf
 
     comps = out.eval_components(x=en)
     logger.info(comps)
 
     if not plot_final:
@@ -1616,17 +1649,19 @@
         
     simul_rms = []
     simul_harm = []
     fp_back = background
     fp_back_error = background_error
     for i in range(n_simul):
         if use_poisson:
-            fp = random.poisson(np.max( [np.ones(len(counts)), counts], axis=0))
+            fp = random.poisson(counts)
+            if np.sum(counts==0):
+                print("WARNING: some counts are zero in simulation")
             if background is not None:
-                fp_back = random.poisson(np.max( [np.ones(len(background)), background], axis=0))
+                fp_back = random.poisson(np.ones(len(background))*background.mean())
                 fp_back_error = np.sqrt(fp_back)
         else:
             fp = random.normal(counts, np.max( [np.ones(len(counts_err)), counts_err], axis=0))
             if background is not None and background_error is not None:
                 fp_back = random.normal(background, np.max( [np.ones(len(background_error)), background_error], axis=0))
         if 'verbose' in kwargs and kwargs['verbose']:
             x,y = method(fp, counts_err, background=fp_back, background_error=fp_back_error, **kwargs)
@@ -1641,77 +1676,144 @@
         axes[1].hist(simul_harm, bins=10)
 
     if 'verbose' in kwargs and kwargs['verbose']:
         return np.std(simul_rms), np.max(simul_harm), np.min(simul_harm)
     else:
         return np.std(simul_rms)
 
-def fft_pulsed_fraction(x, dx, level=0.1, n_harm_min=2, n_harm_max=-1, plot=False, verbose=False, label='', 
-                        background=None, background_error=None):
-    '''
-    Computes the pulsed fraction using an FFT. It stops as soon as the pulse is described at better than level
-    :param x: pulse profile
-    :param dx: pulse profile uncertainty
-    :param level: confidence level for chi^2 test to stop number of harmonics (default 0.1)
-    :param n_harm_min: minimum number of harmonics to use (default 2)
-    :param n_harm_max: maximum number of harmonics to use (default -1 takes the size of pulse profile)
-    :param plot: plot the pulse profile
-    :param lavel: to save the plot with name "rms_`label`.pdf", if label=='' it does not save the plot
-    ;parma verbose (bool): if true it returns both pulsed_frac, n_harm, if false just the pulsed_frac
-    ;param background the vector of the background
-    ;param backgroun_error the uncertainty vector of the background
-    :return: pulsed fraction (float)
-    '''
-    # import scipy.stats.chisquare as chi2
+def get_n_harm(x, dx=None, level=0.1, n_harm_min=2, n_harm_max=-1, statistics='cstat'):
+    """This returns the number of harmonics necessary to describe the signal in x with uncertainty dx
+    at minimal Significance level (=1- confidence level) (note that for lower values, you get lower harmonics)
+    Available statistics are: cstat, chi2, archibald.
+    cstat is based on Kaastra et al (2017) https://doi.org/10.1051/0004-6361/201629319
+    chi2 is a standard implementation
+    archibald is from Archibald et al. (2014), appendix A (inaccurate !)
+
+    Args:
+        x (numpy array): signal
+        dx (numpy array): signal uncertainty, necesssary only for chi2
+        level (float, optional): minimum confidence . Defaults to 0.1.
+        n_harm_min (int, optional): minimum number of harmonics. Defaults to 2.
+        n_harm_max (int, optional): maximum number of harmonics. Defaults to -1.
+        statistics (str, optional): methods, see above. Defaults to 'cstat'.
+
+    Returns:
+        int: number of necessary harmonics
+    """
+
+    if statistics == 'chi2' and dx is None:
+        raise Exception('For chi2 statistics, you need to provide uncertaintis')
+    
     from scipy.stats import chi2
-    from matplotlib import cm
+    from scipy.stats import norm
+    import cashstatistic as cstat
+    
+    # Quantile (the cumulative probability)
+    q = 1 - (level / 2 )
+    # Critical z-score, calculated using the percent-point function (aka the
+    # quantile function) of the normal distribution
+    z_star = norm.ppf(q)
     n = len(x)
-
     if n_harm_max < n_harm_min or n_harm_max+1 > n/2:
+        logger.debug('n_harm max = %d' % n_harm_max)
         n_harm_max = n / 2 - 1
 
+    n = len(x)
     fft = np.fft.fft(x)
     old_chi2_sf = -1.0
+    old_cstat = 1e10
     for n_harm in range(int(n_harm_min), int(n_harm_max)+1):
         mask = np.ones(n, dtype=np.cdouble)
         mask[n_harm:-(n_harm - 1)] = 0 + 0j
         ifft = np.fft.ifft(fft * mask)
         y = np.real(ifft)
         #Necessary to avoid infinite for zero uncertaity
         ind = dx > 0
         #print(ind)
-        chi2_val = np.sum(((x[ind] - y[ind]) / dx[ind]) ** 2)
-        dof = max(1, n - (1 + 2 * (n_harm - 1)))
-        chi2_sf = chi2.sf(chi2_val, dof)
-        logger.debug(chi2_val, chi2_sf, dof, n_harm)
-        # print(chi2_sf, old_chi2_sf)
-        #Sometimes, we do ot reach the required level, but we cannot describe the pulse significantly better,
-        # so we stop in any case (condition chi2_sf < old_chi2_sf)
-        if chi2_sf > level or (chi2_sf < old_chi2_sf and chi2_sf > level/100.):
-            logger.debug('chi2_sf = %e (level is %.5f) old_chi2_sf = %e' % (chi2_sf, level, old_chi2_sf))
-            break
-        old_chi2_sf = chi2_sf
-        if n_harm == n_harm_max:
-            logger.info('maximum number of harmonics reached')
+        if statistics == 'chi2':
+            chi2_val = np.sum(((x[ind] - y[ind]) / dx[ind]) ** 2)
+            dof = max(1, n - (1 + 2 * (n_harm - 1)))
+            chi2_sf = chi2.sf(chi2_val, dof)
+            logger.debug('%d %f %d %f %f' % (n_harm, chi2_val, dof,  chi2_sf, old_chi2_sf))
+            
+            #Sometimes, we do ot reach the required level, but we cannot describe the pulse significantly better,
+            # so we stop in any case (condition chi2_sf < old_chi2_sf)
+            if chi2_sf > level or (chi2_sf < old_chi2_sf and chi2_sf > level/100.):
+                logger.debug('chi2_sf = %e (level is %.5f) old_chi2_sf = %e' % (chi2_sf, level, old_chi2_sf))
+                break
+            old_chi2_sf = chi2_sf
+            if n_harm == n_harm_max:
+                logger.debug('maximum number of harmonics reached')
+        elif statistics=='cstat':
+            cstat_val = cstat.cash_mod(y,x).sum()
+            c_e, c_v = cstat.cash_mod_expectations(y)
+            tmp1 = np.sum(c_e)
+            tmp2 = z_star * np.sqrt(np.sum(c_v))
+            logger.debug("%d %e %e %e" %(n_harm, cstat_val, tmp1, tmp2 ))
+            if  cstat_val < tmp1 + tmp2 or cstat_val > old_cstat: #cstat_val > tmp1 - tmp2 and
+                logger.debug('cstat = %e (expected is %e +/- %e) old_chi2_sf = %e' % (cstat_val, tmp1, tmp2, old_cstat))
+                break
+            old_cstat = cstat_val
+            if n_harm == n_harm_max:
+                logger.debug('maximum number of harmonics reached')
+        elif statistics == 'archibald':
+            a,b,sigma_a,sigma_b = compute_a_b_sigma_a_sigma_b(x, dx, int(n_harm_max))
+            m4 = 4*np.arange(1,n_harm_max+1)
+            cumulative_sum = np.zeros(int(n_harm_max))
+            for k in range(1,int(n_harm_max)):
+                cumulative_sum[k] = np.sum( (a[0:k]/sigma_a[0:k])**2 + (b[0:k]/sigma_b[0:k])**2)
+            #print(cumulative_sum)
+            n_harm = np.argmax(cumulative_sum - m4) + 1
+            #print("We stop at %d harmonics" % max_harm)
+        else:
+            raise Exception('Statistics %s is not implemented' % statistics)
 
     logger.debug("Used %d harmonics for pulse description" % n_harm)
+
+    return n_harm
+
+def fft_pulsed_fraction(x, dx, level=0.1, n_harm_min=2, n_harm_max=-1, plot=False, verbose=False, label='', 
+                        background=None, background_error=None, statistics='cstat'):
+    '''
+    Computes the pulsed fraction using an FFT. It stops as soon as the pulse is described at better than level
+    :param x: pulse profile
+    :param dx: pulse profile uncertainty
+    :param level: minimum confidence level to stop number of harmonics (default 0.1, lower values give less harmonics)
+    :param n_harm_min: minimum number of harmonics to use (default 2)
+    :param n_harm_max: maximum number of harmonics to use (default -1 takes the size of pulse profile)
+    :param plot: plot the pulse profile
+    :param lavel: to save the plot with name "rms_`label`.pdf", if label=='' it does not save the plot
+    ;parma verbose (bool): if true it returns both pulsed_frac, n_harm, if false just the pulsed_frac
+    ;param background the vector of the background
+    ;param backgroun_error the uncertainty vector of the background
+    ;param statistics : the method to compute the optimal number of harmonics (chi2, cstat, archibald) de cstat, see the function get_n_harm
+    :return: pulsed fraction (float)
+    '''
     
+    from matplotlib import cm
+    n = len(x)
+    n_harm = get_n_harm(x, dx, level=level, n_harm_min=n_harm_min, n_harm_max=n_harm_max, statistics=statistics)
+    fft = np.fft.fft(x)
     a = np.absolute(fft) / n
-
     if background is not None and background_error is not None:
         a[0] = subtract_background(a[0], background,background_error)
     
     pulsed_frac = np.sqrt(np.sum(a[1:n_harm] ** 2) + np.sum(a[-n_harm + 1:] ** 2)) / a[0]
-    col = cm.viridis(np.linspace(0, 1,int(n_harm_max)+1))
+    col = cm.viridis(np.linspace(0, 1,int(n_harm)+1))
     if plot:
         import matplotlib.pyplot as plt
         f = np.linspace(0, 1, n)
         #plt.errorbar(f, x, yerr=dx, fmt='.', label='data %s' % label, color = col[n_harm])
         #plt.plot(f, y, label='%d harmonics' % n_harm, linestyle='--', color = col[n_harm])
         plt.errorbar(f, x, yerr=dx, fmt='.', color=col[n_harm])
+        fft = np.fft.fft(x)
+        mask = np.ones(n, dtype=np.cdouble)
+        mask[n_harm:-(n_harm - 1)] = 0 + 0j
+        ifft = np.fft.ifft(fft * mask)
+        y = np.real(ifft)
         plt.plot(f, y, linestyle='--', color=col[n_harm])
         #plt.text(0.4,120,str(n_harm)+'  harmonics',color = col[n_harm])
         plt.xlabel('Phase')
         plt.ylabel('Counts')
         #plt.legend()
         if label != '':
             plt.savefig('rms_%s.pdf' % label)
@@ -1745,15 +1847,14 @@
 
     return pulsed_frac, dpulsed_frac
 import matplotlib.cm
 
 def plot_matrix_as_image(ee, pp, kind='E', normalize=True,outfile=None, cmap=matplotlib.cm.gist_earth,
                          sliders=False, n_levels=30, min_level=None, max_level=None, source_name=None):
     '''
-
     :param ee: y-scale (time or energy)
     :param pp: Energy-Phase or Time-Phase matrix (# of rows must equal len(ee))
     :param kind: * 'E' energy phase
                  * 'T' Time-phase
                  * 'NE' energy phase with energy normalized to the cyclotron energy
     :param normalize: normalize each pulse at its average and divide by the standard deviation
     :param outfile: the file to save the figure as image (optional)
@@ -2302,7 +2403,58 @@
     name = input_name
     simbad = Simbad.query_object(name)
     c = SkyCoord(simbad['RA'], simbad['DEC'], unit=[u.hour, u.deg])
     c.fk5
     logger.info("Coordinates for %s are RA=%.4f, Dec=%.4f" % (name, c.ra.deg[0], c.dec.deg[0]))
 
     return c.ra.deg[0], c.dec.deg[0]
+
+def lmfit_chain_to_dict(dict_name, my_chain, high_part = True):
+    """reformats the mcmc results to be used as
+    pysas.dump_latex_table(dict_param, utils.mcmc_latex_dict))
+    where dict_param is the output of this function
+
+    Args:
+        dict_name (str): name of the disctionary to be put in the table
+        my_chain (object): first output of utils.explore_fit_mcmc
+        high_part (bool, optional): this flag changes the name of gaussians from gX to ggX. Defaults to True.
+
+    Returns:
+        dict: a dictionary of parameters as expected by pysas.dump_latex_table
+    """
+    quantiles = my_chain.flatchain.quantile([0.32, 0.5, 0.68])
+    
+    out_dict = { dict_name : {} }
+    
+    for kk in quantiles.keys():
+        
+        if high_part:
+            key_name = kk.replace('g','gg')
+        else:
+            key_name = kk
+        out_dict[dict_name].update( {key_name: [ quantiles[kk][0.50], quantiles[kk][0.32], quantiles[kk][0.68]]})
+    out_dict[dict_name].update({'cstat' : [my_chain.chisqr, my_chain.nfree, my_chain.nfree]})
+    return out_dict
+
+mcmc_latex_dict = {
+    'poly_c0' : '$c_0$',
+    'poly_c1' : '$c_1$',
+    'poly_c2' : '$c_2$',
+    'poly_c3' : '$c_3$',
+    'poly_c4' : '$c_4$',
+    'poly_c5' : '$c_5$',
+    'poly_c6' : '$c_6$',
+    'poly_c7' : '$c_7$',
+    'g1_amplitude': '$A_\\mathrm{Fe}$',
+    'g1_center': '$E_\\mathrm{Fe}$',
+    'g1_sigma': '$\\sigma_\\mathrm{Fe}$',
+    'gg1_amplitude': '$A_\\mathrm{Cyc}$',
+    'gg1_center': '$E_\\mathrm{Cyc}$',
+    'gg1_sigma': '$\\sigma_\\mathrm{Cyc}$',
+    'gg2_amplitude': '$A_\\mathrm{Cyc2}$',
+    'gg2_center': '$E_\\mathrm{Cyc2}$',
+    'gg2_sigma': '$\\sigma_\\mathrm{Cyc2}$',
+    'cstat' : '$\\Chi^2_\\mathrm{red}$/d.o.f.',
+}
+
+
+
```

### Comparing `nustarpipeline-0.2.8/nustarpipeline.egg-info/PKG-INFO` & `nustarpipeline-0.2.9/nustarpipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.8
+Version: 0.2.9
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.8/setup.cfg` & `nustarpipeline-0.2.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.8
+current_version = 0.2.9
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
 
@@ -60,14 +60,15 @@
 	PyYAML
 	requests
 	bs4
 	lmfit
 	corner
 	stingray
 	emcee
+	cashstatistic
 tests_require = 
 	pytest
 	mypy
 	pylint
 
 [options.entry_points]
 console_scripts =
```

