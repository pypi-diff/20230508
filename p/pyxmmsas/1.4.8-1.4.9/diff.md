# Comparing `tmp/pyxmmsas-1.4.8.tar.gz` & `tmp/pyxmmsas-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxmmsas-1.4.8.tar", last modified: Wed Dec 22 18:39:47 2021, max compression
+gzip compressed data, was "pyxmmsas-1.4.9.tar", last modified: Tue Jan  4 12:21:01 2022, max compression
```

## Comparing `pyxmmsas-1.4.8.tar` & `pyxmmsas-1.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2021-12-22 18:39:47.754577 pyxmmsas-1.4.8/
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2020-03-04 18:52:25.000000 pyxmmsas-1.4.8/LICENSE
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      327 2021-12-22 18:39:47.754577 pyxmmsas-1.4.8/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      983 2020-06-22 15:24:40.000000 pyxmmsas-1.4.8/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2021-12-22 18:39:47.750577 pyxmmsas-1.4.8/pyxmmsas/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)   152418 2021-12-22 16:32:36.000000 pyxmmsas-1.4.8/pyxmmsas/__init__.py
--rwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)     3120 2021-11-26 15:46:30.000000 pyxmmsas-1.4.8/pyxmmsas/extract_spectra.py
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2021-12-22 18:39:47.754577 pyxmmsas-1.4.8/pyxmmsas.egg-info/
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      327 2021-12-22 18:39:47.000000 pyxmmsas-1.4.8/pyxmmsas.egg-info/PKG-INFO
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      244 2021-12-22 18:39:47.000000 pyxmmsas-1.4.8/pyxmmsas.egg-info/SOURCES.txt
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)        1 2021-12-22 18:39:47.000000 pyxmmsas-1.4.8/pyxmmsas.egg-info/dependency_links.txt
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      119 2021-12-22 18:39:47.000000 pyxmmsas-1.4.8/pyxmmsas.egg-info/requires.txt
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)        9 2021-12-22 18:39:47.000000 pyxmmsas-1.4.8/pyxmmsas.egg-info/top_level.txt
--rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)       79 2021-12-22 18:39:47.754577 pyxmmsas-1.4.8/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1096 2021-12-22 18:39:11.000000 pyxmmsas-1.4.8/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-01-04 12:21:01.879417 pyxmmsas-1.4.9/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2020-03-04 18:52:25.000000 pyxmmsas-1.4.9/LICENSE
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      327 2022-01-04 12:21:01.879417 pyxmmsas-1.4.9/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      983 2020-06-22 15:24:40.000000 pyxmmsas-1.4.9/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-01-04 12:21:01.879417 pyxmmsas-1.4.9/pyxmmsas/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)   154275 2022-01-04 12:19:12.000000 pyxmmsas-1.4.9/pyxmmsas/__init__.py
+-rwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)     3120 2021-11-26 15:46:30.000000 pyxmmsas-1.4.9/pyxmmsas/extract_spectra.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2022-01-04 12:21:01.879417 pyxmmsas-1.4.9/pyxmmsas.egg-info/
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      327 2022-01-04 12:21:01.000000 pyxmmsas-1.4.9/pyxmmsas.egg-info/PKG-INFO
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      244 2022-01-04 12:21:01.000000 pyxmmsas-1.4.9/pyxmmsas.egg-info/SOURCES.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)        1 2022-01-04 12:21:01.000000 pyxmmsas-1.4.9/pyxmmsas.egg-info/dependency_links.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)      147 2022-01-04 12:21:01.000000 pyxmmsas-1.4.9/pyxmmsas.egg-info/requires.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)        9 2022-01-04 12:21:01.000000 pyxmmsas-1.4.9/pyxmmsas.egg-info/top_level.txt
+-rw-r--r--   0 ferrigno  (1000) ferrigno  (1000)       79 2022-01-04 12:21:01.879417 pyxmmsas-1.4.9/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1205 2022-01-04 12:19:12.000000 pyxmmsas-1.4.9/setup.py
```

### Comparing `pyxmmsas-1.4.8/LICENSE` & `pyxmmsas-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxmmsas-1.4.8/README.md` & `pyxmmsas-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pyxmmsas-1.4.8/pyxmmsas/__init__.py` & `pyxmmsas-1.4.9/pyxmmsas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,17 @@
         xspec.AllData.ignore('bad')
 
         n_spectra = xspec.AllData.nGroups
         spectra = [xspec.AllData(j) for j in range(1, n_spectra + 1)]
 
         for s, ig in zip(spectra, ignore_string):
             s.ignore(ig)
-
+        # print(xspec.Fit.statistic)
+        xspec.Fit.perform()
+        # print("Fitted ", xspec.Fit.statistic)
         sampled_fit_statistics.append(xspec.Fit.statistic)
 
     best_fit_statistic = sampled_fit_statistics[0]
     sorted_sampled_fit_statistics = sorted(sampled_fit_statistics[1:], reverse=True)
 
     arg_min = np.argmin(np.abs(np.array(sorted_sampled_fit_statistics) - best_fit_statistic))
     goodness = float(arg_min) / float(len(sorted_sampled_fit_statistics) - 1)
@@ -415,93 +417,102 @@
     return n_spectra, models
 
 
 def epic_bxa_run(xspec, xspec_model_file,
                  pn_spec="PNsource_spectrum_rbn.pi",
                  mos1_spec="MOS1source_spectrum_rbn.pi",
                  mos2_spec="MOS2source_spectrum_rbn.pi",
-                 ignore_string=['**-0.5,10.0-**'],
-                 outputfiles_basename='bxa-', run_sampling=False, jeffreys_priors=['norm'],
-                 sampling_efficiency=0.3,
-                 n_live_points=400, evidence_tolerance=0.5, perform_fit=False, save_xcm=True,
-                 compute_errors=True):
+                 ignore_string=3*['**-0.5,10.0-**'],
+                 outputfiles_basename='bxa-',  jeffreys_priors=['norm', 'nH'], Lepsilon=0.1,
+                 frac_remain=0.5,
+                 n_live_points=400, evidence_tolerance=0.5):
+    """
+    :param xspec: instance of xspec
+    :param xspec_model_file: xspec model file to load
+    :param pn_spec: spectrum file name
+    :param mos1_spec: spectrum file name (if 'none' skips)
+    :param mos2_spec: spectrum file name (if 'none' skips)
+    :param ignore_string: Ignore string for Xspec
+    :param outputfiles_basename: def. 'bxa-'
+    :param jeffreys_priors: paramters for Jeffrey's priors, no need to specify the component number (Def.) ['norm', 'nH']
+    :param n_live_points: number of live points (400 to 1000 is recommended).
+    :param evidence_tolerance: uncertainty on the evidence to achieve
+    :param Lepsilon: numerical model inaccuracies in the statistic (default: 0.1).
+        Increase if run is not finishing because it is trying too hard to resolve
+        unimportant details caused e.g., by atable interpolations.
+    :param frac_remain: fraction of the integration remainder allowed in the live points.
+        Setting to 0.5 in mono-modal problems can be acceptable and faster.
+        The default is 0.01 (safer).
+    :return: transformations, results
+    """
     import bxa.xspec as bxa
-    import pymultinest
 
     n_spectra, models = epic_load_spectra_set_model(xspec, xspec_model_file,
                                                     pn_spec,
                                                     mos1_spec,
                                                     mos2_spec, ignore_string)
 
     transformations = []
 
     for mm in models:
-
         comp_names = mm.componentNames
         for cc in comp_names:
             comp = getattr(mm, cc)
             for par_name in comp.parameterNames:
                 par = getattr(comp, par_name)
-
                 if par.frozen or par.link != '':
                     print(par_name, ' linked or frozen ')
                     continue
-
                 if par_name not in jeffreys_priors:  # 'norm'
                     transformations.append(bxa.create_uniform_prior_for(mm, par))
                     print('uniform prior for %s %s' % (cc, par_name))
                 elif par_name in jeffreys_priors:
                     transformations.append(bxa.create_jeffreys_prior_for(mm, par))
                     print('jeffreys prior for %s %s' % (cc, par_name))
                 else:
                     raise RuntimeError('cannot define prior for parameter %' % par_name)
 
-    if run_sampling:
-        analyzer = bxa.nested_run(transformations,
-                                  outputfiles_basename=outputfiles_basename,
-                                  sampling_efficiency=sampling_efficiency,
-                                  n_live_points=n_live_points, evidence_tolerance=evidence_tolerance,
-                                  verbose=True,  # show a bit of progress
-                                  resume=True  # MultiNest supports resuming a crashed/aborted run
-                                  )
-    else:
-        analyzer = pymultinest.Analyzer(n_params=len(transformations),
-                                        outputfiles_basename=outputfiles_basename)
-        xspec.AllChains.clear()
-        xspec.AllChains += outputfiles_basename + 'chain.fits'
-
-    best_fit = analyzer.get_best_fit()
-
-    print('Best log likelihood is %g' % best_fit['log_likelihood'])
-
-    s = analyzer.get_stats()
-
-    pars = []
-
-    for t, b, m in zip(transformations, best_fit['parameters'], s['marginals']):
-        if 'log(' in t['name']:
-            # t['model'](t['index']).values=10**m['median']
-
-            pars += [t['model'], {t['index']: 10 ** b}]
-            print(' %20s: %.3f ' % (t['name'].replace('log(', '').replace(')', ''), 10 ** b))
-            print(' %20s: %.3f  %.3f %.3f ' % (t['name'].replace('log(', '').replace(')', ''),
-                                               10 ** m['median'], 10 ** m['q10%'], 10 ** m['q90%']))
-
-        else:
-            pars += [t['model'], {t['index']: b}]
-            print(' %20s: %.3f' % (t['name'], b))
-            print(' %20s: %.3f  %.3f %.3f ' % (t['name'], m['median'], m['q10%'], m['q90%']))
+    analyzer = bxa.BXASolver(transformations, outputfiles_basename=outputfiles_basename)
+    results = analyzer.run(resume=True, n_live_points=n_live_points, evidence_tolerance=evidence_tolerance,
+                           Lepsilon=Lepsilon, frac_remain=frac_remain)
+    # else:
+    #     analyzer = pymultinest.Analyzer(n_params=len(transformations),
+    #                                     outputfiles_basename=outputfiles_basename)
+    #     xspec.AllChains.clear()
+    #     xspec.AllChains += outputfiles_basename + 'chain.fits'
 
-    xspec.AllModels.setPars(*pars)
-    print('Cstat=', xspec.Fit.statistic, 'Chi2=', xspec.Fit.testStatistic, 'dof=', xspec.Fit.dof)
-
-    fit_results = plot_save_xcm(xspec, outputfiles_basename,
-                                perform_fit, save_xcm=save_xcm, compute_errors=compute_errors)
+    # best_fit = analyzer.get_best_fit()
+    #
+    # print('Best log likelihood is %g' % best_fit['log_likelihood'])
+    #
+    # s = analyzer.get_stats()
+    #
+    # pars = []
+    #
+    # for t, b, m in zip(transformations, best_fit['parameters'], s['marginals']):
+    #     if 'log(' in t['name']:
+    #         # t['model'](t['index']).values=10**m['median']
+    #
+    #         pars += [t['model'], {t['index']: 10 ** b}]
+    #         print(' %20s: %.3f ' % (t['name'].replace('log(', '').replace(')', ''), 10 ** b))
+    #         print(' %20s: %.3f  %.3f %.3f ' % (t['name'].replace('log(', '').replace(')', ''),
+    #                                            10 ** m['median'], 10 ** m['q10%'], 10 ** m['q90%']))
+    #
+    #     else:
+    #         pars += [t['model'], {t['index']: b}]
+    #         print(' %20s: %.3f' % (t['name'], b))
+    #         print(' %20s: %.3f  %.3f %.3f ' % (t['name'], m['median'], m['q10%'], m['q90%']))
+    #
+    # xspec.AllModels.setPars(*pars)
+    # print('Cstat=', xspec.Fit.statistic, 'Chi2=', xspec.Fit.testStatistic, 'dof=', xspec.Fit.dof)
+    #
+    # fit_results = plot_save_xcm(xspec, outputfiles_basename,
+    #                             perform_fit, save_xcm=save_xcm, compute_errors=compute_errors)
 
-    return transformations, fit_results
+    return transformations, results
 
 
 def plot_save_xcm(xspec, outputfiles_basename, perform_fit=False, save_xcm=True, compute_errors=True):
     import os
     if save_xcm:
         xcmfile = outputfiles_basename + 'model.xcm'
         if os.path.exists(xcmfile):
@@ -641,16 +652,15 @@
                            mark_panels=False, fontsize=plt.rcParams['font.size'], log_scale_labels=[]):
     '''
     fit_by_bin : dictionary fir fit parameters in given format (see rearrange_fit_parameters)
     pn : the object pn (EPICPN) to derive some observation properties
     t1, dt1, r, dr, hr, dhr : rate and hardness ratio (see also plot_fit_parameters_norate for a version without light curve)
     plot_latex : use the latex backend
     latex_label_dict : a dictionary with keys the fit parameters of the fit_by_bin dictionary and item the y labels of the plot
-    skip_factors : skip normalization factors (not used)
-    skipped : a list of dictionary keys to skip in plotting
+    skipped : a list of dictionary keys to skip in plotting def. ['factor', 'cstat', 'plot_filename'],
     save_plot : to skip the saving of plots
     dpi : plot resolution
     plot_unbinned : if plot HR vs Count_rate unbinned
     test_correlation : test for correlation between the parameters
     n_sample : correlation bootstrap sample
     threshold_prob : maximum null-hypothesis probability to plot the line
     mask : a mask for parameters in form of boolean array or None only for linear regression
@@ -811,18 +821,22 @@
                         mark_panels='False', fontsize=plt.rcParams['font.size'], log_scale_labels=[]):
     '''
     fit_by_bin : dictionary fir fit parameters in given format (see rearrange_fit_parameters)
     pn : the object pn (EPICPN) to derive some observation properties
     t1, dt1, r, dr, hr, dhr : rate and hardness ratio (see also plot_fit_parameters_norate for a version without light curve)
     plot_latex : use the latex backend
     latex_label_dict : a dictionary with keys the fit parameters of the fit_by_bin dictionary and item the y labels of the plot
-    skip_factors : skip normalization factors (not used)
-    skipped : a list of dictionary keys to skip in plotting
+    skipped : a list of dictionary keys to skip in plotting def. ['factor', 'cstat', 'plot_filename'],
     save_plot : to skip the saving of plots
     dpi : plot resolution
+    x_scale_multiplier : scale x-axis by (def = 1)
+    xlabel : label for x-axis 'Time [s] (date is added if pn is porovided)'
+    mark_panels : mark panels with letters
+    fontsize : change the font size
+    log_scale_labels : parameters to be ploteed in log scale
     '''
 
     from matplotlib import rc
     plt.rcParams.update({'font.size': fontsize})
 
     fit_by_par = rearrange_fit_parameters(fit_by_bin)
     n_pars = len(fit_by_par.keys()) + 1
@@ -918,15 +932,15 @@
         try:
             axes[i].set_ylabel(latex_label_dict[ylabel])
         except:
             print("Label " + ylabel + ' not found in latex_label_dict')
             axes[i].set_ylabel(ylabel)
         i += 1
     if pn is not None:
-        axes[i - 1].set_xlabel('%s since %s' % (xlabel, pn.date_obs))
+        axes[i - 1].set_xlabel('%s since %s' % (xlabel, pn.date_obs.replace('T', ' ')))
         axes[0].set_title('%s (%s)' % (pn.target, pn.obs_id))
     else:
         axes[i - 1].set_xlabel(xlabel)
 
     plt.rcParams['figure.figsize'] = old_size
 
     rc('text', usetex=False)
@@ -1914,14 +1928,17 @@
 
         REFYLMIN = hdu.header['REFYLMIN']
         REFYLMAX = hdu.header['REFYLMAX']
 
         xscale = (REFXLMAX - REFXLMIN) / image.shape[0]
         yscale = (REFYLMAX - REFYLMIN) / image.shape[0]
 
+        xscale_wcs = hdu.header['REFXCDLT']
+#        yscale_wcs = hdu.header['REFYCDLT']
+
         f_header.close()
 
         # Checck the maximum of image
         ind_max = np.unravel_index(np.argmax(image, axis=None), image.shape)
         print("Image maximum is at ", my_wcs.wcs_pix2world(ind_max[1], ind_max[0], 0))
         if make_plots:
             ax.scatter(ind_max[1], ind_max[0], s=40, marker='+', color='white')
@@ -2081,15 +2098,17 @@
             fig1.savefig(self.workdir + '/%s.png' % (filename.split('.')[-2].split('/')[-1]))
             fig2.savefig(self.workdir + '/%s_psf.png' % (filename.split('.')[-2].split('/')[-1]))
 
         sas_source_coord = 'x_src=%.1f\ny_src=%.1f\nr_src=%.1f\n' % (physical_x, physical_y, physical_r_max)
         sas_back_coord = 'x_bkg=%.1f\ny_bkg=%.1f\nr_bkg=%.1f\n' % (physical_back_x, physical_back_y, physical_r_back)
 
         print("source physical coordinates\n" + sas_source_coord)
+        print("source extraction radius %.2f arcmin" % (physical_r_max * np.abs(xscale_wcs) * 60.))
         print("background physical coordinates\n" + sas_back_coord)
+        print("background extraction radius %.2f arcmin" % (physical_r_back * np.abs(xscale_wcs) * 60.))
 
         return sas_source_coord, sas_back_coord
 
     def print_infos(self):
         print('We observe the target %s with obs_id=%s, from %s to %s' % (
         self.target, self.obs_id, self.date_obs, self.date_end))
 
@@ -2657,15 +2676,16 @@
                 tstart = data['START']
                 tstop = data['STOP']
 
                 ontime = np.sum(tstop - tstart)
 
                 p_f.close()
 
-                print("The sum of GTI for %s is %.3f ks" % (self.instrument, ontime / 1e3))
+                print("The sum of GTI for %s is %.3f ks the elapsed time %.3f ks" % (self.instrument, ontime / 1e3,
+                                                                                     (tstop.max()-tstart.min())/1e3))
             except:
                 print('%s GTI file does not exist' % self.instrument)
 
     def filter_with(self, other_instrument, tmin=0, tmax=1e13, run_script=True):
 
         # Not used, currently
 
@@ -3093,14 +3113,16 @@
         # Image Conversion factors
         REFXLMIN = hdu.header['REFXLMIN']
         REFXLMAX = hdu.header['REFXLMAX']
 
         REFYLMIN = hdu.header['REFYLMIN']
         REFYLMAX = hdu.header['REFYLMAX']
 
+        xscale_wcs = hdu.header['REFXCDLT']
+
         xscale = (REFXLMAX - REFXLMIN) / image.shape[0]
         yscale = (REFYLMAX - REFYLMIN) / image.shape[0]
 
         f_header.close()
         f_header_timing.close()
 
         rawx_histo = image_timing.sum(axis=0)
@@ -3174,14 +3196,16 @@
             sas_source_coord += 'rawx_high=%.1f\nrawx_low=%.1f\n' % (ind_max + crval1, ind_max + crval1)
 
         sas_back_coord = 'x_bkg=%.1f\ny_bkg=%.1f\nwidth_bkg=%.1f\nheight_bkg=%.1f' % (
             physical_back_x, physical_back_y, box_width * xscale, box_height * yscale)
 
         print("source physical coordinates\n" + sas_source_coord)
         print("background physical coordinates\n" + sas_back_coord)
+        print('Background size %.3f x %.3f arcmin' % (box_width * xscale * np.abs(xscale_wcs)*60,
+                                               box_height * yscale * np.abs(xscale_wcs)*60))
 
         return sas_source_coord, sas_back_coord
 
     ev_filter_expression_base = '#XMMEA_EM && (PI IN (500:12000)) && (PATTERN<=0) && (FLAG==0) ' + \
                                 '&& (TIME IN (%.2f:%.2f))'
 
     #     sas_commands_spec_src_mos = '''
```

### Comparing `pyxmmsas-1.4.8/pyxmmsas/extract_spectra.py` & `pyxmmsas-1.4.9/pyxmmsas/extract_spectra.py`

 * *Files identical despite different names*

### Comparing `pyxmmsas-1.4.8/setup.py` & `pyxmmsas-1.4.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 #print ('packs',packs)
 #
 
 include_package_data = True
 
 setup(name='pyxmmsas',
       scripts=[],
-      version="1.4.8",
+      version="1.4.9",
       description='It is wrapper for SAS and performs spectral analysis and plots',
       author='Carlo Ferrigno',
       author_email='carlo.ferrigno@unige.ch',
       packages=['pyxmmsas'],
       install_requires=["astropy!=3.0.*,!=3.1,!=3.1.1,>=2.0.12",
                         "numpy",
                         "astroquery",
                         "matplotlib",
                         "scipy",
                         "photutils",
                         "optimalgrouping>=1.0.3",
-                        "adaptivelcbin"
+                        "adaptivelcbin",
+                        "cython",
+                        "ultranest",
+                        "bxa>=4.0.5"
                     ],
       url="https://gitlab.astro.unige.ch/ferrigno/pysas",
       python_requires='>=3.0',
       license='MIT'
       )
```

