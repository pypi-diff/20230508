# Comparing `tmp/pyobs_core-1.3.7.tar.gz` & `tmp/pyobs_core-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_core-1.3.7.tar", max compression
+gzip compressed data, was "pyobs_core-1.4.0.tar", max compression
```

## Comparing `pyobs_core-1.3.7.tar` & `pyobs_core-1.4.0.tar`

### file list

```diff
@@ -1,287 +1,287 @@
--rw-r--r--   0        0        0     1099 2023-03-27 14:31:59.794384 pyobs_core-1.3.7/LICENSE
--rw-r--r--   0        0        0       80 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/__init__.py
--rw-r--r--   0        0        0     6651 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/application.py
--rw-r--r--   0        0        0        0 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/cli/__init__.py
--rwxr-xr-x   0        0        0     2559 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/cli/pyobs.py
--rwxr-xr-x   0        0        0     8257 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/cli/pyobsd.py
--rw-r--r--   0        0        0      299 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/cli/pyobsw.py
--rw-r--r--   0        0        0     1568 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/__init__.py
--rw-r--r--   0        0        0    15114 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/comm.py
--rw-r--r--   0        0        0      995 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/commlogging.py
--rw-r--r--   0        0        0       31 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/dbus/__init__.py
--rw-r--r--   0        0        0    19591 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/dbus/dbuscomm.py
--rw-r--r--   0        0        0       33 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/dummy/__init__.py
--rw-r--r--   0        0        0     1409 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/dummy/dummycomm.py
--rw-r--r--   0        0        0     4525 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/proxy.py
--rw-r--r--   0        0        0       55 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/__init__.py
--rw-r--r--   0        0        0     8696 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/rpc.py
--rw-r--r--   0        0        0      102 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009/__init__.py
--rw-r--r--   0        0        0     6010 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009/binding.py
--rw-r--r--   0        0        0     1607 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009/rpc.py
--rw-r--r--   0        0        0      174 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009_timeout/__init__.py
--rw-r--r--   0        0        0     2131 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009_timeout/rpc.py
--rw-r--r--   0        0        0      467 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009_timeout/stanza/RPC.py
--rw-r--r--   0        0        0      231 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009_timeout/stanza/__init__.py
--rw-r--r--   0        0        0     3626 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xmppclient.py
--rw-r--r--   0        0        0    18283 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/comm/xmpp/xmppcomm.py
--rw-r--r--   0        0        0     6818 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/environment.py
--rw-r--r--   0        0        0      924 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/__init__.py
--rw-r--r--   0        0        0      165 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/badweather.py
--rw-r--r--   0        0        0     2413 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/event.py
--rw-r--r--   0        0        0     1511 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/exposurestatuschanged.py
--rw-r--r--   0        0        0      528 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/filterchanged.py
--rw-r--r--   0        0        0      904 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/focusfound.py
--rw-r--r--   0        0        0     1090 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/goodweather.py
--rw-r--r--   0        0        0     1243 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/log.py
--rw-r--r--   0        0        0      196 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/moduleclosed.py
--rw-r--r--   0        0        0      196 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/moduleopened.py
--rw-r--r--   0        0        0     1601 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/motionstatuschanged.py
--rw-r--r--   0        0        0     1269 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/move.py
--rw-r--r--   0        0        0     2052 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/newimage.py
--rw-r--r--   0        0        0     1003 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/newspectrum.py
--rw-r--r--   0        0        0     1331 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/offsets.py
--rw-r--r--   0        0        0      181 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/roofclosing.py
--rw-r--r--   0        0        0      185 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/roofopened.py
--rw-r--r--   0        0        0      778 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/taskfailed.py
--rw-r--r--   0        0        0      786 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/taskfinished.py
--rw-r--r--   0        0        0     1689 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/taskstarted.py
--rw-r--r--   0        0        0      415 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/events/testevent.py
--rw-r--r--   0        0        0      138 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/__init__.py
--rw-r--r--   0        0        0    10575 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/image.py
--rw-r--r--   0        0        0      193 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/__init__.py
--rw-r--r--   0        0        0      154 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/altazoffsets.py
--rw-r--r--   0        0        0      110 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/exptime.py
--rw-r--r--   0        0        0      165 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/onskydistance.py
--rw-r--r--   0        0        0      145 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/pixeloffsets.py
--rw-r--r--   0        0        0      154 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/radecoffsets.py
--rw-r--r--   0        0        0     1731 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/meta/skyoffsets.py
--rw-r--r--   0        0        0      651 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/processor.py
--rw-r--r--   0        0        0       94 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/processors/__init__.py
--rw-r--r--   0        0        0      102 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/processors/astrometry/__init__.py
--rw-r--r--   0        0        0      556 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/processors/astrometry/astrometry.py
--rw-r--r--   0        0        0     5890 2023-03-27 14:31:59.798384 pyobs_core-1.3.7/pyobs/images/processors/astrometry/dotnet.py
--rw-r--r--   0        0        0      248 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/detection/__init__.py
--rw-r--r--   0        0        0     2962 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/detection/daophot.py
--rw-r--r--   0        0        0     6704 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/detection/pysep.py
--rw-r--r--   0        0        0      583 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/detection/sourcedetection.py
--rw-r--r--   0        0        0      135 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/exptime/__init__.py
--rw-r--r--   0        0        0     1459 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/exptime/exptime.py
--rw-r--r--   0        0        0     2779 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/exptime/star.py
--rw-r--r--   0        0        0      264 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/__init__.py
--rw-r--r--   0        0        0     1856 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/addmask.py
--rw-r--r--   0        0        0     1510 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/broadcast.py
--rw-r--r--   0        0        0     6281 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/calibration.py
--rw-r--r--   0        0        0     1208 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/createfilename.py
--rw-r--r--   0        0        0     1681 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/removebackground.py
--rw-r--r--   0        0        0     1406 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/smooth.py
--rw-r--r--   0        0        0     1850 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/misc/softbin.py
--rw-r--r--   0        0        0      411 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/__init__.py
--rw-r--r--   0        0        0     1883 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/astrometry.py
--rw-r--r--   0        0        0     1873 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/brighteststar.py
--rw-r--r--   0        0        0     1149 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/fitsheader.py
--rw-r--r--   0        0        0    15066 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/nstar.py
--rw-r--r--   0        0        0     1597 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/offsets.py
--rw-r--r--   0        0        0     5673 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/offsets/projected.py
--rw-r--r--   0        0        0      222 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/photometry/__init__.py
--rw-r--r--   0        0        0      584 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/photometry/photometry.py
--rw-r--r--   0        0        0     3856 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/photometry/photutil.py
--rw-r--r--   0        0        0     4775 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/images/processors/photometry/pysep.py
--rw-r--r--   0        0        0      377 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IAbortable.py
--rw-r--r--   0        0        0      862 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IAcquisition.py
--rw-r--r--   0        0        0     1407 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IAutoFocus.py
--rw-r--r--   0        0        0      282 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IAutoGuiding.py
--rw-r--r--   0        0        0      272 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IAutonomous.py
--rw-r--r--   0        0        0     1041 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IBinning.py
--rw-r--r--   0        0        0      379 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ICalibrate.py
--rw-r--r--   0        0        0      247 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ICamera.py
--rw-r--r--   0        0        0     1776 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IConfig.py
--rw-r--r--   0        0        0     1086 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ICooling.py
--rw-r--r--   0        0        0      660 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IData.py
--rw-r--r--   0        0        0      318 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IDome.py
--rw-r--r--   0        0        0      827 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IExposure.py
--rw-r--r--   0        0        0     1117 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IExposureTime.py
--rw-r--r--   0        0        0     1000 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFilters.py
--rw-r--r--   0        0        0      809 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFitsHeaderAfter.py
--rw-r--r--   0        0        0      815 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFitsHeaderBefore.py
--rw-r--r--   0        0        0      586 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFlatField.py
--rw-r--r--   0        0        0      570 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFocusModel.py
--rw-r--r--   0        0        0     1262 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IFocuser.py
--rw-r--r--   0        0        0      751 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IGain.py
--rw-r--r--   0        0        0     1073 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IImageFormat.py
--rw-r--r--   0        0        0      774 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IImageType.py
--rw-r--r--   0        0        0      977 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ILatLon.py
--rw-r--r--   0        0        0      998 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IModule.py
--rw-r--r--   0        0        0     1281 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IMotion.py
--rw-r--r--   0        0        0      935 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IOffsetsAltAz.py
--rw-r--r--   0        0        0      925 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IOffsetsRaDec.py
--rw-r--r--   0        0        0      888 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IPointingAltAz.py
--rw-r--r--   0        0        0      925 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IPointingHGS.py
--rw-r--r--   0        0        0      894 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IPointingRaDec.py
--rw-r--r--   0        0        0      892 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IPointingSeries.py
--rw-r--r--   0        0        0      545 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IReady.py
--rw-r--r--   0        0        0      203 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IRoof.py
--rw-r--r--   0        0        0      558 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IRotation.py
--rw-r--r--   0        0        0      394 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IRunnable.py
--rw-r--r--   0        0        0      376 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IRunning.py
--rw-r--r--   0        0        0      456 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IScriptRunner.py
--rw-r--r--   0        0        0      259 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ISpectrograph.py
--rw-r--r--   0        0        0      485 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IStartStop.py
--rw-r--r--   0        0        0      493 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ISyncTarget.py
--rw-r--r--   0        0        0      336 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ITelescope.py
--rw-r--r--   0        0        0      532 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/ITemperatures.py
--rw-r--r--   0        0        0      424 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IVideo.py
--rw-r--r--   0        0        0     1469 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IWeather.py
--rw-r--r--   0        0        0     1196 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/IWindow.py
--rw-r--r--   0        0        0     2062 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/__init__.py
--rw-r--r--   0        0        0      208 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/interfaces/interface.py
--rw-r--r--   0        0        0      476 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/__init__.py
--rw-r--r--   0        0        0     2372 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/camerasettings.py
--rw-r--r--   0        0        0    14232 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/fitsheader.py
--rw-r--r--   0        0        0     2723 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/fitsnamespace.py
--rw-r--r--   0        0        0     5869 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/follow.py
--rw-r--r--   0        0        0     4397 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/motionstatus.py
--rw-r--r--   0        0        0     1439 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/pipeline.py
--rw-r--r--   0        0        0     2796 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/waitformotion.py
--rw-r--r--   0        0        0     4998 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/mixins/weatheraware.py
--rw-r--r--   0        0        0     2430 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/__init__.py
--rw-r--r--   0        0        0      264 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/__init__.py
--rw-r--r--   0        0        0    13978 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/adaptive.py
--rw-r--r--   0        0        0    15701 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/basecamera.py
--rw-r--r--   0        0        0     7025 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/basespectrograph.py
--rw-r--r--   0        0        0    15472 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/basevideo.py
--rw-r--r--   0        0        0     9261 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/dummycamera.py
--rw-r--r--   0        0        0     2610 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/camera/dummyspectrograph.py
--rw-r--r--   0        0        0      202 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/flatfield/__init__.py
--rw-r--r--   0        0        0     9085 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/flatfield/flatfield.py
--rw-r--r--   0        0        0     1505 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/flatfield/pointing.py
--rw-r--r--   0        0        0     4397 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/flatfield/scheduler.py
--rw-r--r--   0        0        0      154 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/focus/__init__.py
--rw-r--r--   0        0        0    18119 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/focus/focusmodel.py
--rw-r--r--   0        0        0     8547 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/focus/focusseries.py
--rw-r--r--   0        0        0      189 2023-03-27 14:31:59.802384 pyobs_core-1.3.7/pyobs/modules/image/__init__.py
--rw-r--r--   0        0        0     8201 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/image/imagewatcher.py
--rw-r--r--   0        0        0     2935 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/image/imagewriter.py
--rw-r--r--   0        0        0     3630 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/image/seeing.py
--rw-r--r--   0        0        0    17774 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/module.py
--rw-r--r--   0        0        0      348 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/__init__.py
--rw-r--r--   0        0        0     2488 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/_base.py
--rw-r--r--   0        0        0     7831 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/_baseguiding.py
--rw-r--r--   0        0        0     7038 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/acquisition.py
--rw-r--r--   0        0        0     3877 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/autoguiding.py
--rw-r--r--   0        0        0     1531 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/dummyacquisition.py
--rw-r--r--   0        0        0      828 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/dummyguiding.py
--rw-r--r--   0        0        0     3145 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/pointing/scienceframeguiding.py
--rw-r--r--   0        0        0      183 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/robotic/__init__.py
--rw-r--r--   0        0        0     5647 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/robotic/mastermind.py
--rw-r--r--   0        0        0     6840 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/robotic/pointing.py
--rw-r--r--   0        0        0    17505 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/robotic/scheduler.py
--rw-r--r--   0        0        0      159 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/roof/__init__.py
--rw-r--r--   0        0        0     1311 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/roof/basedome.py
--rw-r--r--   0        0        0     2102 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/roof/baseroof.py
--rw-r--r--   0        0        0     3967 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/roof/dummyroof.py
--rw-r--r--   0        0        0      158 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/telescope/__init__.py
--rw-r--r--   0        0        0    11418 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/telescope/basetelescope.py
--rw-r--r--   0        0        0    10625 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/telescope/dummytelescope.py
--rw-r--r--   0        0        0      101 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/test/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/test/standalone.py
--rw-r--r--   0        0        0      279 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/__init__.py
--rw-r--r--   0        0        0     4945 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/autonomouswarning.py
--rw-r--r--   0        0        0     1663 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/fluentlogger.py
--rw-r--r--   0        0        0     3304 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/httpfilecache.py
--rw-r--r--   0        0        0     4728 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/kiosk.py
--rw-r--r--   0        0        0    19721 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/telegram.py
--rw-r--r--   0        0        0     2980 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/utils/trigger.py
--rw-r--r--   0        0        0       93 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/weather/__init__.py
--rw-r--r--   0        0        0     8102 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/modules/weather/weather.py
--rw-r--r--   0        0        0    18099 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/object.py
--rw-r--r--   0        0        0      134 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/__init__.py
--rw-r--r--   0        0        0      160 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/__init__.py
--rw-r--r--   0        0        0     3766 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/dummytaskschedule.py
--rw-r--r--   0        0        0     2628 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/portal.py
--rw-r--r--   0        0        0      110 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/scripts/__init__.py
--rw-r--r--   0        0        0     5646 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/scripts/autofocus.py
--rw-r--r--   0        0        0    11915 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/scripts/default.py
--rw-r--r--   0        0        0     2064 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/scripts/script.py
--rw-r--r--   0        0        0    10145 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/task.py
--rw-r--r--   0        0        0     5045 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/taskarchive.py
--rw-r--r--   0        0        0    13522 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/lco/taskschedule.py
--rw-r--r--   0        0        0       58 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/scripts/__init__.py
--rw-r--r--   0        0        0     1483 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/scripts/script.py
--rw-r--r--   0        0        0     4545 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/scripts/skyflats.py
--rw-r--r--   0        0        0     2326 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/task.py
--rw-r--r--   0        0        0      702 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/taskarchive.py
--rw-r--r--   0        0        0     1362 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/taskrunner.py
--rw-r--r--   0        0        0     1501 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/robotic/taskschedule.py
--rw-r--r--   0        0        0        0 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/__init__.py
--rw-r--r--   0        0        0      174 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/archive/__init__.py
--rw-r--r--   0        0        0     3221 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/archive/archive.py
--rw-r--r--   0        0        0     7764 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/archive/local_archive.py
--rw-r--r--   0        0        0     8971 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/archive/pyobs_archive.py
--rw-r--r--   0        0        0     1381 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/average.py
--rw-r--r--   0        0        0     2844 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/cache.py
--rw-r--r--   0        0        0      511 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/config.py
--rw-r--r--   0        0        0     1025 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/coordinates.py
--rw-r--r--   0        0        0      802 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/curvefit.py
--rw-r--r--   0        0        0     3608 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/enums.py
--rw-r--r--   0        0        0     7380 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/exceptions.py
--rw-r--r--   0        0        0     8317 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/fits.py
--rw-r--r--   0        0        0      175 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/focusseries/__init__.py
--rw-r--r--   0        0        0      779 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/focusseries/base.py
--rw-r--r--   0        0        0     2768 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/focusseries/photometry.py
--rw-r--r--   0        0        0     6503 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/focusseries/projection.py
--rw-r--r--   0        0        0     2800 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/grids.py
--rw-r--r--   0        0        0     1099 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/http.py
--rw-r--r--   0        0        0      671 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/logger.py
--rw-r--r--   0        0        0     1485 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/modulegui.py
--rw-r--r--   0        0        0      137 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/offsets/__init__.py
--rw-r--r--   0        0        0     3734 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/offsets/applyaltazoffsets.py
--rw-r--r--   0        0        0     3658 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/offsets/applyoffsets.py
--rw-r--r--   0        0        0     3465 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/offsets/applyradecoffsets.py
--rw-r--r--   0        0        0     3324 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/parallel.py
--rw-r--r--   0        0        0     1669 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/pid.py
--rw-r--r--   0        0        0       56 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/pipeline/__init__.py
--rw-r--r--   0        0        0    10047 2023-03-27 14:31:59.806384 pyobs_core-1.3.7/pyobs/utils/pipeline/night.py
--rw-r--r--   0        0        0     6883 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/pipeline/pipeline.py
--rw-r--r--   0        0        0      159 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/__init__.py
--rw-r--r--   0        0        0     1335 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/csv.py
--rw-r--r--   0        0        0     3097 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/http.py
--rw-r--r--   0        0        0      852 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/log.py
--rw-r--r--   0        0        0      963 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/multi.py
--rw-r--r--   0        0        0      360 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/publisher/publisher.py
--rw-r--r--   0        0        0      146 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/simulation/__init__.py
--rw-r--r--   0        0        0     9339 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/simulation/camera.py
--rw-r--r--   0        0        0     7294 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/simulation/telescope.py
--rw-r--r--   0        0        0     3027 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/simulation/world.py
--rw-r--r--   0        0        0      120 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/__init__.py
--rw-r--r--   0        0        0     7619 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/exptimeeval.py
--rw-r--r--   0        0        0    19900 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/flatfielder.py
--rw-r--r--   0        0        0      204 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/pointing/__init__.py
--rw-r--r--   0        0        0      607 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/pointing/base.py
--rw-r--r--   0        0        0     1899 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/pointing/static.py
--rw-r--r--   0        0        0      184 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/__init__.py
--rw-r--r--   0        0        0     2149 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/archive.py
--rw-r--r--   0        0        0      283 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/base.py
--rw-r--r--   0        0        0      543 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/const.py
--rw-r--r--   0        0        0     6567 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/skyflats/scheduler.py
--rw-r--r--   0        0        0      117 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/threads/__init__.py
--rw-r--r--   0        0        0      577 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/threads/checkabort.py
--rw-r--r--   0        0        0     1410 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/threads/lockwithabort.py
--rw-r--r--   0        0        0     1115 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/threads/threadwithreturnvalue.py
--rw-r--r--   0        0        0     2020 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/time.py
--rw-r--r--   0        0        0     7886 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/utils/types.py
--rw-r--r--   0        0        0      257 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/version.py
--rw-r--r--   0        0        0     3354 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/__init__.py
--rw-r--r--   0        0        0     2402 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/archivefile.py
--rw-r--r--   0        0        0     2042 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/file.py
--rw-r--r--   0        0        0       68 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/filelists/__init__.py
--rw-r--r--   0        0        0      185 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/filelists/filelist.py
--rw-r--r--   0        0        0      396 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/filelists/testing.py
--rw-r--r--   0        0        0     5380 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/httpfile.py
--rw-r--r--   0        0        0     4591 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/localfile.py
--rw-r--r--   0        0        0     1794 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/memfile.py
--rw-r--r--   0        0        0     3789 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/smbfile.py
--rw-r--r--   0        0        0     3685 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/sshfile.py
--rw-r--r--   0        0        0     2682 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/tempfile.py
--rw-r--r--   0        0        0     9206 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyobs/vfs/vfs.py
--rw-r--r--   0        0        0     1462 2023-03-27 14:31:59.810384 pyobs_core-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 pyobs_core-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-08 08:42:09.890686 pyobs_core-1.4.0/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/__init__.py
+-rw-r--r--   0        0        0     6651 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/application.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/cli/__init__.py
+-rwxr-xr-x   0        0        0     2559 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/cli/pyobs.py
+-rwxr-xr-x   0        0        0     8257 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/cli/pyobsd.py
+-rw-r--r--   0        0        0      299 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/cli/pyobsw.py
+-rw-r--r--   0        0        0     1568 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/__init__.py
+-rw-r--r--   0        0        0    15114 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/comm.py
+-rw-r--r--   0        0        0      995 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/commlogging.py
+-rw-r--r--   0        0        0       31 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/dbus/__init__.py
+-rw-r--r--   0        0        0    19591 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/dbus/dbuscomm.py
+-rw-r--r--   0        0        0       33 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/dummy/__init__.py
+-rw-r--r--   0        0        0     1409 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/dummy/dummycomm.py
+-rw-r--r--   0        0        0     4525 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/proxy.py
+-rw-r--r--   0        0        0       55 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/__init__.py
+-rw-r--r--   0        0        0     8696 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/rpc.py
+-rw-r--r--   0        0        0      102 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009/__init__.py
+-rw-r--r--   0        0        0     6010 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009/binding.py
+-rw-r--r--   0        0        0     1607 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009/rpc.py
+-rw-r--r--   0        0        0      174 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009_timeout/__init__.py
+-rw-r--r--   0        0        0     2131 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py
+-rw-r--r--   0        0        0      467 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/RPC.py
+-rw-r--r--   0        0        0      231 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009_timeout/stanza/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xmppclient.py
+-rw-r--r--   0        0        0    18283 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/comm/xmpp/xmppcomm.py
+-rw-r--r--   0        0        0     6818 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/environment.py
+-rw-r--r--   0        0        0      924 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/badweather.py
+-rw-r--r--   0        0        0     2413 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/event.py
+-rw-r--r--   0        0        0     1511 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/exposurestatuschanged.py
+-rw-r--r--   0        0        0      528 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/filterchanged.py
+-rw-r--r--   0        0        0      904 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/focusfound.py
+-rw-r--r--   0        0        0     1090 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/goodweather.py
+-rw-r--r--   0        0        0     1243 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/log.py
+-rw-r--r--   0        0        0      196 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/moduleclosed.py
+-rw-r--r--   0        0        0      196 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/moduleopened.py
+-rw-r--r--   0        0        0     1601 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/motionstatuschanged.py
+-rw-r--r--   0        0        0     1269 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/move.py
+-rw-r--r--   0        0        0     2052 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/newimage.py
+-rw-r--r--   0        0        0     1003 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/newspectrum.py
+-rw-r--r--   0        0        0     1331 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/offsets.py
+-rw-r--r--   0        0        0      181 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/roofclosing.py
+-rw-r--r--   0        0        0      185 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/roofopened.py
+-rw-r--r--   0        0        0      778 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/taskfailed.py
+-rw-r--r--   0        0        0      786 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/taskfinished.py
+-rw-r--r--   0        0        0     1689 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/taskstarted.py
+-rw-r--r--   0        0        0      415 2023-05-08 08:42:09.894687 pyobs_core-1.4.0/pyobs/events/testevent.py
+-rw-r--r--   0        0        0      138 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/__init__.py
+-rw-r--r--   0        0        0    11006 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/image.py
+-rw-r--r--   0        0        0      193 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/altazoffsets.py
+-rw-r--r--   0        0        0      110 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/exptime.py
+-rw-r--r--   0        0        0      165 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/onskydistance.py
+-rw-r--r--   0        0        0      145 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/pixeloffsets.py
+-rw-r--r--   0        0        0      154 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/radecoffsets.py
+-rw-r--r--   0        0        0     1731 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/meta/skyoffsets.py
+-rw-r--r--   0        0        0      651 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processor.py
+-rw-r--r--   0        0        0       94 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/astrometry/__init__.py
+-rw-r--r--   0        0        0      556 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/astrometry/astrometry.py
+-rw-r--r--   0        0        0     5890 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/astrometry/dotnet.py
+-rw-r--r--   0        0        0      248 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/detection/__init__.py
+-rw-r--r--   0        0        0     2962 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/detection/daophot.py
+-rw-r--r--   0        0        0     6704 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/detection/pysep.py
+-rw-r--r--   0        0        0      583 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/detection/sourcedetection.py
+-rw-r--r--   0        0        0      135 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/exptime/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/exptime/exptime.py
+-rw-r--r--   0        0        0     2779 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/exptime/star.py
+-rw-r--r--   0        0        0      264 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/__init__.py
+-rw-r--r--   0        0        0     1856 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/addmask.py
+-rw-r--r--   0        0        0     1510 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/broadcast.py
+-rw-r--r--   0        0        0     6281 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/calibration.py
+-rw-r--r--   0        0        0     1208 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/createfilename.py
+-rw-r--r--   0        0        0     1681 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/removebackground.py
+-rw-r--r--   0        0        0     1406 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/smooth.py
+-rw-r--r--   0        0        0     1850 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/misc/softbin.py
+-rw-r--r--   0        0        0      411 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/__init__.py
+-rw-r--r--   0        0        0     1883 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/astrometry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/brighteststar.py
+-rw-r--r--   0        0        0     1149 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/fitsheader.py
+-rw-r--r--   0        0        0    15066 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/nstar.py
+-rw-r--r--   0        0        0     1597 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/offsets.py
+-rw-r--r--   0        0        0     5673 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/offsets/projected.py
+-rw-r--r--   0        0        0      222 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/photometry/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/photometry/photometry.py
+-rw-r--r--   0        0        0     3856 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/photometry/photutil.py
+-rw-r--r--   0        0        0     4775 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/images/processors/photometry/pysep.py
+-rw-r--r--   0        0        0      377 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IAbortable.py
+-rw-r--r--   0        0        0      862 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IAcquisition.py
+-rw-r--r--   0        0        0     1407 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IAutoFocus.py
+-rw-r--r--   0        0        0      282 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IAutoGuiding.py
+-rw-r--r--   0        0        0      272 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IAutonomous.py
+-rw-r--r--   0        0        0     1041 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IBinning.py
+-rw-r--r--   0        0        0      379 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ICalibrate.py
+-rw-r--r--   0        0        0      247 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ICamera.py
+-rw-r--r--   0        0        0     1776 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IConfig.py
+-rw-r--r--   0        0        0     1086 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ICooling.py
+-rw-r--r--   0        0        0      660 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IData.py
+-rw-r--r--   0        0        0      318 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IDome.py
+-rw-r--r--   0        0        0      827 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IExposure.py
+-rw-r--r--   0        0        0     1117 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IExposureTime.py
+-rw-r--r--   0        0        0     1000 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFilters.py
+-rw-r--r--   0        0        0      809 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFitsHeaderAfter.py
+-rw-r--r--   0        0        0      815 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFitsHeaderBefore.py
+-rw-r--r--   0        0        0      586 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFlatField.py
+-rw-r--r--   0        0        0      570 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFocusModel.py
+-rw-r--r--   0        0        0     1262 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IFocuser.py
+-rw-r--r--   0        0        0      751 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IGain.py
+-rw-r--r--   0        0        0     1073 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IImageFormat.py
+-rw-r--r--   0        0        0      774 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IImageType.py
+-rw-r--r--   0        0        0      977 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ILatLon.py
+-rw-r--r--   0        0        0      998 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IModule.py
+-rw-r--r--   0        0        0     1281 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IMotion.py
+-rw-r--r--   0        0        0      935 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IOffsetsAltAz.py
+-rw-r--r--   0        0        0      925 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IOffsetsRaDec.py
+-rw-r--r--   0        0        0      888 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IPointingAltAz.py
+-rw-r--r--   0        0        0      925 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IPointingHGS.py
+-rw-r--r--   0        0        0      894 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IPointingRaDec.py
+-rw-r--r--   0        0        0      892 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IPointingSeries.py
+-rw-r--r--   0        0        0      545 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IReady.py
+-rw-r--r--   0        0        0      203 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IRoof.py
+-rw-r--r--   0        0        0      558 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IRotation.py
+-rw-r--r--   0        0        0      394 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IRunnable.py
+-rw-r--r--   0        0        0      376 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IRunning.py
+-rw-r--r--   0        0        0      456 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IScriptRunner.py
+-rw-r--r--   0        0        0      259 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ISpectrograph.py
+-rw-r--r--   0        0        0      485 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IStartStop.py
+-rw-r--r--   0        0        0      493 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ISyncTarget.py
+-rw-r--r--   0        0        0      336 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ITelescope.py
+-rw-r--r--   0        0        0      532 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/ITemperatures.py
+-rw-r--r--   0        0        0      424 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IVideo.py
+-rw-r--r--   0        0        0     1469 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IWeather.py
+-rw-r--r--   0        0        0     1196 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/IWindow.py
+-rw-r--r--   0        0        0     2062 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/interfaces/interface.py
+-rw-r--r--   0        0        0      476 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/camerasettings.py
+-rw-r--r--   0        0        0    14232 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/fitsheader.py
+-rw-r--r--   0        0        0     2723 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/fitsnamespace.py
+-rw-r--r--   0        0        0     5869 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/follow.py
+-rw-r--r--   0        0        0     4397 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/motionstatus.py
+-rw-r--r--   0        0        0     1439 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/pipeline.py
+-rw-r--r--   0        0        0     2796 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/waitformotion.py
+-rw-r--r--   0        0        0     4998 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/mixins/weatheraware.py
+-rw-r--r--   0        0        0     2430 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/camera/__init__.py
+-rw-r--r--   0        0        0    13978 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/camera/adaptive.py
+-rw-r--r--   0        0        0    15701 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/camera/basecamera.py
+-rw-r--r--   0        0        0     7025 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/camera/basespectrograph.py
+-rw-r--r--   0        0        0    15472 2023-05-08 08:42:09.898687 pyobs_core-1.4.0/pyobs/modules/camera/basevideo.py
+-rw-r--r--   0        0        0     9261 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/camera/dummycamera.py
+-rw-r--r--   0        0        0     2610 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/camera/dummyspectrograph.py
+-rw-r--r--   0        0        0      202 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/flatfield/__init__.py
+-rw-r--r--   0        0        0     9085 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/flatfield/flatfield.py
+-rw-r--r--   0        0        0     1505 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/flatfield/pointing.py
+-rw-r--r--   0        0        0     4397 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/flatfield/scheduler.py
+-rw-r--r--   0        0        0      154 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/focus/__init__.py
+-rw-r--r--   0        0        0    18119 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/focus/focusmodel.py
+-rw-r--r--   0        0        0     8547 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/focus/focusseries.py
+-rw-r--r--   0        0        0      189 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/image/__init__.py
+-rw-r--r--   0        0        0     8201 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/image/imagewatcher.py
+-rw-r--r--   0        0        0     2935 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/image/imagewriter.py
+-rw-r--r--   0        0        0     3630 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/image/seeing.py
+-rw-r--r--   0        0        0    17774 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/module.py
+-rw-r--r--   0        0        0      348 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/__init__.py
+-rw-r--r--   0        0        0     2488 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/_base.py
+-rw-r--r--   0        0        0     7831 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/_baseguiding.py
+-rw-r--r--   0        0        0     7038 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/acquisition.py
+-rw-r--r--   0        0        0     3877 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/autoguiding.py
+-rw-r--r--   0        0        0     1531 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/dummyacquisition.py
+-rw-r--r--   0        0        0      828 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/dummyguiding.py
+-rw-r--r--   0        0        0     3145 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/pointing/scienceframeguiding.py
+-rw-r--r--   0        0        0      183 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/robotic/__init__.py
+-rw-r--r--   0        0        0     5647 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/robotic/mastermind.py
+-rw-r--r--   0        0        0     6840 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/robotic/pointing.py
+-rw-r--r--   0        0        0    17505 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/robotic/scheduler.py
+-rw-r--r--   0        0        0      159 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/roof/__init__.py
+-rw-r--r--   0        0        0     1311 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/roof/basedome.py
+-rw-r--r--   0        0        0     2102 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/roof/baseroof.py
+-rw-r--r--   0        0        0     3967 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/roof/dummyroof.py
+-rw-r--r--   0        0        0      158 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/telescope/__init__.py
+-rw-r--r--   0        0        0    11418 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/telescope/basetelescope.py
+-rw-r--r--   0        0        0    10625 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/telescope/dummytelescope.py
+-rw-r--r--   0        0        0      101 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/test/__init__.py
+-rw-r--r--   0        0        0     1055 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/test/standalone.py
+-rw-r--r--   0        0        0      279 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/__init__.py
+-rw-r--r--   0        0        0     4945 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/autonomouswarning.py
+-rw-r--r--   0        0        0     1663 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/fluentlogger.py
+-rw-r--r--   0        0        0     3304 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/httpfilecache.py
+-rw-r--r--   0        0        0     4728 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/kiosk.py
+-rw-r--r--   0        0        0    19721 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/telegram.py
+-rw-r--r--   0        0        0     2980 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/utils/trigger.py
+-rw-r--r--   0        0        0       93 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/weather/__init__.py
+-rw-r--r--   0        0        0     8102 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/modules/weather/weather.py
+-rw-r--r--   0        0        0    18099 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/object.py
+-rw-r--r--   0        0        0      134 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/__init__.py
+-rw-r--r--   0        0        0     3766 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/dummytaskschedule.py
+-rw-r--r--   0        0        0     2628 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/portal.py
+-rw-r--r--   0        0        0      110 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/scripts/__init__.py
+-rw-r--r--   0        0        0     5646 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/scripts/autofocus.py
+-rw-r--r--   0        0        0    11915 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/scripts/default.py
+-rw-r--r--   0        0        0     2064 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/scripts/script.py
+-rw-r--r--   0        0        0    10145 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/task.py
+-rw-r--r--   0        0        0     5045 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/taskarchive.py
+-rw-r--r--   0        0        0    13522 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/lco/taskschedule.py
+-rw-r--r--   0        0        0       58 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/scripts/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/scripts/script.py
+-rw-r--r--   0        0        0     4545 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/scripts/skyflats.py
+-rw-r--r--   0        0        0     2326 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/task.py
+-rw-r--r--   0        0        0      702 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/taskarchive.py
+-rw-r--r--   0        0        0     1362 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/taskrunner.py
+-rw-r--r--   0        0        0     1501 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/robotic/taskschedule.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/archive/__init__.py
+-rw-r--r--   0        0        0     3221 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/archive/archive.py
+-rw-r--r--   0        0        0     7764 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/archive/local_archive.py
+-rw-r--r--   0        0        0     8971 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/archive/pyobs_archive.py
+-rw-r--r--   0        0        0     1381 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/average.py
+-rw-r--r--   0        0        0     2844 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/cache.py
+-rw-r--r--   0        0        0      511 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/config.py
+-rw-r--r--   0        0        0     1025 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/coordinates.py
+-rw-r--r--   0        0        0      802 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/curvefit.py
+-rw-r--r--   0        0        0     3608 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/enums.py
+-rw-r--r--   0        0        0     7380 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/exceptions.py
+-rw-r--r--   0        0        0     8317 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/fits.py
+-rw-r--r--   0        0        0      175 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/focusseries/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/focusseries/base.py
+-rw-r--r--   0        0        0     2768 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/focusseries/photometry.py
+-rw-r--r--   0        0        0     6503 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/focusseries/projection.py
+-rw-r--r--   0        0        0     2800 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/grids.py
+-rw-r--r--   0        0        0     1099 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/http.py
+-rw-r--r--   0        0        0      671 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/logger.py
+-rw-r--r--   0        0        0     1485 2023-05-08 08:42:09.902687 pyobs_core-1.4.0/pyobs/utils/modulegui.py
+-rw-r--r--   0        0        0      137 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/offsets/__init__.py
+-rw-r--r--   0        0        0     3734 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/offsets/applyaltazoffsets.py
+-rw-r--r--   0        0        0     3658 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/offsets/applyoffsets.py
+-rw-r--r--   0        0        0     3465 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/offsets/applyradecoffsets.py
+-rw-r--r--   0        0        0     3324 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/parallel.py
+-rw-r--r--   0        0        0     1669 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/pid.py
+-rw-r--r--   0        0        0       56 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/pipeline/__init__.py
+-rw-r--r--   0        0        0    10047 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/pipeline/night.py
+-rw-r--r--   0        0        0     6883 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/pipeline/pipeline.py
+-rw-r--r--   0        0        0      159 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/__init__.py
+-rw-r--r--   0        0        0     1335 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/csv.py
+-rw-r--r--   0        0        0     3097 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/http.py
+-rw-r--r--   0        0        0      852 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/log.py
+-rw-r--r--   0        0        0      963 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/multi.py
+-rw-r--r--   0        0        0      360 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/publisher/publisher.py
+-rw-r--r--   0        0        0      146 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/simulation/__init__.py
+-rw-r--r--   0        0        0     9339 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/simulation/camera.py
+-rw-r--r--   0        0        0     7294 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/simulation/telescope.py
+-rw-r--r--   0        0        0     3027 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/simulation/world.py
+-rw-r--r--   0        0        0      120 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/__init__.py
+-rw-r--r--   0        0        0     7619 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/exptimeeval.py
+-rw-r--r--   0        0        0    19900 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/flatfielder.py
+-rw-r--r--   0        0        0      204 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/pointing/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/pointing/base.py
+-rw-r--r--   0        0        0     1899 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/pointing/static.py
+-rw-r--r--   0        0        0      184 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/__init__.py
+-rw-r--r--   0        0        0     2149 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/archive.py
+-rw-r--r--   0        0        0      283 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/base.py
+-rw-r--r--   0        0        0      543 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/const.py
+-rw-r--r--   0        0        0     6567 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/skyflats/scheduler.py
+-rw-r--r--   0        0        0      117 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/threads/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/threads/checkabort.py
+-rw-r--r--   0        0        0     1410 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/threads/lockwithabort.py
+-rw-r--r--   0        0        0     1115 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/threads/threadwithreturnvalue.py
+-rw-r--r--   0        0        0     2020 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/time.py
+-rw-r--r--   0        0        0     7886 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/utils/types.py
+-rw-r--r--   0        0        0      257 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/version.py
+-rw-r--r--   0        0        0     3354 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/__init__.py
+-rw-r--r--   0        0        0     2402 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/archivefile.py
+-rw-r--r--   0        0        0     2042 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/file.py
+-rw-r--r--   0        0        0       68 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/filelists/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/filelists/filelist.py
+-rw-r--r--   0        0        0      396 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/filelists/testing.py
+-rw-r--r--   0        0        0     5380 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/httpfile.py
+-rw-r--r--   0        0        0     4591 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/localfile.py
+-rw-r--r--   0        0        0     1794 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/memfile.py
+-rw-r--r--   0        0        0     3789 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/smbfile.py
+-rw-r--r--   0        0        0     3685 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/sshfile.py
+-rw-r--r--   0        0        0     2682 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/tempfile.py
+-rw-r--r--   0        0        0     9206 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyobs/vfs/vfs.py
+-rw-r--r--   0        0        0     1570 2023-05-08 08:42:09.906688 pyobs_core-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 pyobs_core-1.4.0/PKG-INFO
```

### Comparing `pyobs_core-1.3.7/LICENSE` & `pyobs_core-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/application.py` & `pyobs_core-1.4.0/pyobs/application.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/cli/pyobs.py` & `pyobs_core-1.4.0/pyobs/cli/pyobs.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/cli/pyobsd.py` & `pyobs_core-1.4.0/pyobs/cli/pyobsd.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/__init__.py` & `pyobs_core-1.4.0/pyobs/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/comm.py` & `pyobs_core-1.4.0/pyobs/comm/comm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/commlogging.py` & `pyobs_core-1.4.0/pyobs/comm/commlogging.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/dbus/dbuscomm.py` & `pyobs_core-1.4.0/pyobs/comm/dbus/dbuscomm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/dummy/dummycomm.py` & `pyobs_core-1.4.0/pyobs/comm/dummy/dummycomm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/proxy.py` & `pyobs_core-1.4.0/pyobs/comm/proxy.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/rpc.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009/binding.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009/binding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009/rpc.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/xep_0009_timeout/rpc.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/xep_0009_timeout/rpc.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/xmppclient.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/xmppclient.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/comm/xmpp/xmppcomm.py` & `pyobs_core-1.4.0/pyobs/comm/xmpp/xmppcomm.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/environment.py` & `pyobs_core-1.4.0/pyobs/environment.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/__init__.py` & `pyobs_core-1.4.0/pyobs/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/event.py` & `pyobs_core-1.4.0/pyobs/events/event.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/exposurestatuschanged.py` & `pyobs_core-1.4.0/pyobs/events/exposurestatuschanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/filterchanged.py` & `pyobs_core-1.4.0/pyobs/events/filterchanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/focusfound.py` & `pyobs_core-1.4.0/pyobs/events/focusfound.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/goodweather.py` & `pyobs_core-1.4.0/pyobs/events/goodweather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/log.py` & `pyobs_core-1.4.0/pyobs/events/log.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/motionstatuschanged.py` & `pyobs_core-1.4.0/pyobs/events/motionstatuschanged.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/move.py` & `pyobs_core-1.4.0/pyobs/events/move.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/newimage.py` & `pyobs_core-1.4.0/pyobs/events/newimage.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/newspectrum.py` & `pyobs_core-1.4.0/pyobs/events/newspectrum.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/offsets.py` & `pyobs_core-1.4.0/pyobs/events/offsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/taskfailed.py` & `pyobs_core-1.4.0/pyobs/events/taskfailed.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/taskfinished.py` & `pyobs_core-1.4.0/pyobs/events/taskfinished.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/events/taskstarted.py` & `pyobs_core-1.4.0/pyobs/events/taskstarted.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/image.py` & `pyobs_core-1.4.0/pyobs/images/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,38 @@
     def __init__(
         self,
         data: Optional[NDArray[Any]] = None,
         header: Optional[fits.Header] = None,
         mask: Optional[NDArray[Any]] = None,
         uncertainty: Optional[NDArray[Any]] = None,
         catalog: Optional[Table] = None,
+        raw: Optional[NDArray[Any]] = None,
         meta: Optional[Dict[Any, Any]] = None,
         *args: Any,
         **kwargs: Any,
     ):
         """Init a new image.
 
         Args:
             data: Numpy array containing data for image.
             header: Header for the new image.
             mask: Mask for the image.
             uncertainty: Uncertainty image.
             catalog: Catalog table.
+            raw: If image is calibrated, this should be the raw image.
             meta: Dictionary with meta information (note: not preserved in I/O operations!).
         """
 
         # store
         self.data = data
         self.header = fits.Header() if header is None else header.copy()
         self.mask = None if mask is None else mask.copy()
         self.uncertainty = None if uncertainty is None else uncertainty.copy()
         self.catalog = None if catalog is None else catalog.copy()
+        self.raw = None if raw is None else raw.copy()
         self.meta = {} if meta is None else copy.deepcopy(meta)
 
         # add basic header stuff
         if data is not None:
             self.header["NAXIS1"] = data.shape[1]
             self.header["NAXIS2"] = data.shape[0]
 
@@ -156,14 +159,18 @@
         if "UNCERT" in data:
             image.uncertainty = data["UNCERT"].data
 
         # catalog
         if "CAT" in data:
             image.catalog = Table(data["CAT"].data)
 
+        # raw
+        if "RAW" in data:
+            image.raw = data["RAW"].data
+
         # finished
         return image
 
     @property
     def unit(self) -> str:
         """Returns units of pixels in image."""
         return str(self.header["BUNIT"]).lower() if "BUNIT" in self.header else "adu"
@@ -176,14 +183,15 @@
         """Returns a copy of this image."""
         return Image(
             data=self.data,
             header=self.header,
             mask=self.mask,
             uncertainty=self.uncertainty,
             catalog=self.catalog,
+            raw=self.raw,
             meta=self.meta,
         )
 
     def __truediv__(self, other: "Image") -> "Image":
         """Divides this image by other."""
         img = self.copy()
         if img.data is None or other.data is None:
@@ -219,14 +227,20 @@
 
         # errors?
         if self.uncertainty is not None:
             hdu = ImageHDU(self.uncertainty.data)
             hdu.name = "UNCERT"
             hdu_list.append(hdu)
 
+        # raw?
+        if self.raw is not None:
+            hdu = ImageHDU(self.raw.data)
+            hdu.name = "RAW"
+            hdu_list.append(hdu)
+
         # write it
         hdu_list.writeto(f, *args, **kwargs)
 
     def to_bytes(self) -> bytes:
         """Write to a bytes array and return it."""
         with io.BytesIO() as bio:
             self.writeto(bio)
```

### Comparing `pyobs_core-1.3.7/pyobs/images/meta/skyoffsets.py` & `pyobs_core-1.4.0/pyobs/images/meta/skyoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processor.py` & `pyobs_core-1.4.0/pyobs/images/processor.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/astrometry/astrometry.py` & `pyobs_core-1.4.0/pyobs/images/processors/astrometry/astrometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/astrometry/dotnet.py` & `pyobs_core-1.4.0/pyobs/images/processors/astrometry/dotnet.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/detection/daophot.py` & `pyobs_core-1.4.0/pyobs/images/processors/detection/daophot.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/detection/pysep.py` & `pyobs_core-1.4.0/pyobs/images/processors/detection/pysep.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/detection/sourcedetection.py` & `pyobs_core-1.4.0/pyobs/images/processors/detection/sourcedetection.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/exptime/exptime.py` & `pyobs_core-1.4.0/pyobs/images/processors/exptime/exptime.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/exptime/star.py` & `pyobs_core-1.4.0/pyobs/images/processors/exptime/star.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/addmask.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/addmask.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/broadcast.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/broadcast.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/calibration.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/calibration.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/createfilename.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/createfilename.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/removebackground.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/removebackground.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/smooth.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/smooth.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/misc/softbin.py` & `pyobs_core-1.4.0/pyobs/images/processors/misc/softbin.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/astrometry.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/astrometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/brighteststar.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/brighteststar.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/fitsheader.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/fitsheader.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/nstar.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/nstar.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/offsets.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/offsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/offsets/projected.py` & `pyobs_core-1.4.0/pyobs/images/processors/offsets/projected.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/photometry/photometry.py` & `pyobs_core-1.4.0/pyobs/images/processors/photometry/photometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/photometry/photutil.py` & `pyobs_core-1.4.0/pyobs/images/processors/photometry/photutil.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/images/processors/photometry/pysep.py` & `pyobs_core-1.4.0/pyobs/images/processors/photometry/pysep.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IAcquisition.py` & `pyobs_core-1.4.0/pyobs/interfaces/IAcquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IAutoFocus.py` & `pyobs_core-1.4.0/pyobs/interfaces/IAutoFocus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IBinning.py` & `pyobs_core-1.4.0/pyobs/interfaces/IBinning.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IConfig.py` & `pyobs_core-1.4.0/pyobs/interfaces/IConfig.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/ICooling.py` & `pyobs_core-1.4.0/pyobs/interfaces/ICooling.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IData.py` & `pyobs_core-1.4.0/pyobs/interfaces/IData.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IExposure.py` & `pyobs_core-1.4.0/pyobs/interfaces/IExposure.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IExposureTime.py` & `pyobs_core-1.4.0/pyobs/interfaces/IExposureTime.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFilters.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFilters.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFitsHeaderAfter.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFitsHeaderAfter.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFitsHeaderBefore.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFitsHeaderBefore.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFlatField.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFlatField.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFocusModel.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFocusModel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IFocuser.py` & `pyobs_core-1.4.0/pyobs/interfaces/IFocuser.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IGain.py` & `pyobs_core-1.4.0/pyobs/interfaces/IGain.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IImageFormat.py` & `pyobs_core-1.4.0/pyobs/interfaces/IImageFormat.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IImageType.py` & `pyobs_core-1.4.0/pyobs/interfaces/IImageType.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/ILatLon.py` & `pyobs_core-1.4.0/pyobs/interfaces/ILatLon.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IModule.py` & `pyobs_core-1.4.0/pyobs/interfaces/IModule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IMotion.py` & `pyobs_core-1.4.0/pyobs/interfaces/IMotion.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IOffsetsAltAz.py` & `pyobs_core-1.4.0/pyobs/interfaces/IOffsetsAltAz.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IOffsetsRaDec.py` & `pyobs_core-1.4.0/pyobs/interfaces/IOffsetsRaDec.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IPointingAltAz.py` & `pyobs_core-1.4.0/pyobs/interfaces/IPointingAltAz.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IPointingHGS.py` & `pyobs_core-1.4.0/pyobs/interfaces/IPointingHGS.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IPointingRaDec.py` & `pyobs_core-1.4.0/pyobs/interfaces/IPointingRaDec.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IPointingSeries.py` & `pyobs_core-1.4.0/pyobs/interfaces/IPointingSeries.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IReady.py` & `pyobs_core-1.4.0/pyobs/interfaces/IReady.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IRotation.py` & `pyobs_core-1.4.0/pyobs/interfaces/IRotation.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/ITemperatures.py` & `pyobs_core-1.4.0/pyobs/interfaces/ITemperatures.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IWeather.py` & `pyobs_core-1.4.0/pyobs/interfaces/IWeather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/IWindow.py` & `pyobs_core-1.4.0/pyobs/interfaces/IWindow.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/interfaces/__init__.py` & `pyobs_core-1.4.0/pyobs/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/camerasettings.py` & `pyobs_core-1.4.0/pyobs/mixins/camerasettings.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/fitsheader.py` & `pyobs_core-1.4.0/pyobs/mixins/fitsheader.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/fitsnamespace.py` & `pyobs_core-1.4.0/pyobs/mixins/fitsnamespace.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/follow.py` & `pyobs_core-1.4.0/pyobs/mixins/follow.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/motionstatus.py` & `pyobs_core-1.4.0/pyobs/mixins/motionstatus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/pipeline.py` & `pyobs_core-1.4.0/pyobs/mixins/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/waitformotion.py` & `pyobs_core-1.4.0/pyobs/mixins/waitformotion.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/mixins/weatheraware.py` & `pyobs_core-1.4.0/pyobs/mixins/weatheraware.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/__init__.py` & `pyobs_core-1.4.0/pyobs/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/adaptive.py` & `pyobs_core-1.4.0/pyobs/modules/camera/adaptive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/basecamera.py` & `pyobs_core-1.4.0/pyobs/modules/camera/basecamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/basespectrograph.py` & `pyobs_core-1.4.0/pyobs/modules/camera/basespectrograph.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/basevideo.py` & `pyobs_core-1.4.0/pyobs/modules/camera/basevideo.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/dummycamera.py` & `pyobs_core-1.4.0/pyobs/modules/camera/dummycamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/camera/dummyspectrograph.py` & `pyobs_core-1.4.0/pyobs/modules/camera/dummyspectrograph.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/flatfield/flatfield.py` & `pyobs_core-1.4.0/pyobs/modules/flatfield/flatfield.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/flatfield/pointing.py` & `pyobs_core-1.4.0/pyobs/modules/flatfield/pointing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/flatfield/scheduler.py` & `pyobs_core-1.4.0/pyobs/modules/flatfield/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/focus/focusmodel.py` & `pyobs_core-1.4.0/pyobs/modules/focus/focusmodel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/focus/focusseries.py` & `pyobs_core-1.4.0/pyobs/modules/focus/focusseries.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/image/imagewatcher.py` & `pyobs_core-1.4.0/pyobs/modules/image/imagewatcher.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/image/imagewriter.py` & `pyobs_core-1.4.0/pyobs/modules/image/imagewriter.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/image/seeing.py` & `pyobs_core-1.4.0/pyobs/modules/image/seeing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/module.py` & `pyobs_core-1.4.0/pyobs/modules/module.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/_base.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/_base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/_baseguiding.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/_baseguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/acquisition.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/acquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/autoguiding.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/autoguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/dummyacquisition.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/dummyacquisition.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/dummyguiding.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/dummyguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/pointing/scienceframeguiding.py` & `pyobs_core-1.4.0/pyobs/modules/pointing/scienceframeguiding.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/robotic/mastermind.py` & `pyobs_core-1.4.0/pyobs/modules/robotic/mastermind.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/robotic/pointing.py` & `pyobs_core-1.4.0/pyobs/modules/robotic/pointing.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/robotic/scheduler.py` & `pyobs_core-1.4.0/pyobs/modules/robotic/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/roof/basedome.py` & `pyobs_core-1.4.0/pyobs/modules/roof/basedome.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/roof/baseroof.py` & `pyobs_core-1.4.0/pyobs/modules/roof/baseroof.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/roof/dummyroof.py` & `pyobs_core-1.4.0/pyobs/modules/roof/dummyroof.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/telescope/basetelescope.py` & `pyobs_core-1.4.0/pyobs/modules/telescope/basetelescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/telescope/dummytelescope.py` & `pyobs_core-1.4.0/pyobs/modules/telescope/dummytelescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/test/standalone.py` & `pyobs_core-1.4.0/pyobs/modules/test/standalone.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/autonomouswarning.py` & `pyobs_core-1.4.0/pyobs/modules/utils/autonomouswarning.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/fluentlogger.py` & `pyobs_core-1.4.0/pyobs/modules/utils/fluentlogger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/httpfilecache.py` & `pyobs_core-1.4.0/pyobs/modules/utils/httpfilecache.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/kiosk.py` & `pyobs_core-1.4.0/pyobs/modules/utils/kiosk.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/telegram.py` & `pyobs_core-1.4.0/pyobs/modules/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/utils/trigger.py` & `pyobs_core-1.4.0/pyobs/modules/utils/trigger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/modules/weather/weather.py` & `pyobs_core-1.4.0/pyobs/modules/weather/weather.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/object.py` & `pyobs_core-1.4.0/pyobs/object.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/dummytaskschedule.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/dummytaskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/portal.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/portal.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/scripts/autofocus.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/scripts/autofocus.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/scripts/default.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/scripts/default.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/scripts/script.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/scripts/script.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/task.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/task.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/taskarchive.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/taskarchive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/lco/taskschedule.py` & `pyobs_core-1.4.0/pyobs/robotic/lco/taskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/scripts/script.py` & `pyobs_core-1.4.0/pyobs/robotic/scripts/script.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/scripts/skyflats.py` & `pyobs_core-1.4.0/pyobs/robotic/scripts/skyflats.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/task.py` & `pyobs_core-1.4.0/pyobs/robotic/task.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/taskarchive.py` & `pyobs_core-1.4.0/pyobs/robotic/taskarchive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/taskrunner.py` & `pyobs_core-1.4.0/pyobs/robotic/taskrunner.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/robotic/taskschedule.py` & `pyobs_core-1.4.0/pyobs/robotic/taskschedule.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/archive/archive.py` & `pyobs_core-1.4.0/pyobs/utils/archive/archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/archive/local_archive.py` & `pyobs_core-1.4.0/pyobs/utils/archive/local_archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/archive/pyobs_archive.py` & `pyobs_core-1.4.0/pyobs/utils/archive/pyobs_archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/average.py` & `pyobs_core-1.4.0/pyobs/utils/average.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/cache.py` & `pyobs_core-1.4.0/pyobs/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/coordinates.py` & `pyobs_core-1.4.0/pyobs/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/curvefit.py` & `pyobs_core-1.4.0/pyobs/utils/curvefit.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/enums.py` & `pyobs_core-1.4.0/pyobs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/exceptions.py` & `pyobs_core-1.4.0/pyobs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/fits.py` & `pyobs_core-1.4.0/pyobs/utils/fits.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/focusseries/base.py` & `pyobs_core-1.4.0/pyobs/utils/focusseries/base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/focusseries/photometry.py` & `pyobs_core-1.4.0/pyobs/utils/focusseries/photometry.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/focusseries/projection.py` & `pyobs_core-1.4.0/pyobs/utils/focusseries/projection.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/grids.py` & `pyobs_core-1.4.0/pyobs/utils/grids.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/http.py` & `pyobs_core-1.4.0/pyobs/utils/http.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/logger.py` & `pyobs_core-1.4.0/pyobs/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/modulegui.py` & `pyobs_core-1.4.0/pyobs/utils/modulegui.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/offsets/applyaltazoffsets.py` & `pyobs_core-1.4.0/pyobs/utils/offsets/applyaltazoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/offsets/applyoffsets.py` & `pyobs_core-1.4.0/pyobs/utils/offsets/applyoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/offsets/applyradecoffsets.py` & `pyobs_core-1.4.0/pyobs/utils/offsets/applyradecoffsets.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/parallel.py` & `pyobs_core-1.4.0/pyobs/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/pid.py` & `pyobs_core-1.4.0/pyobs/utils/pid.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/pipeline/night.py` & `pyobs_core-1.4.0/pyobs/utils/pipeline/night.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/pipeline/pipeline.py` & `pyobs_core-1.4.0/pyobs/utils/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/publisher/csv.py` & `pyobs_core-1.4.0/pyobs/utils/publisher/csv.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/publisher/http.py` & `pyobs_core-1.4.0/pyobs/utils/publisher/http.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/publisher/log.py` & `pyobs_core-1.4.0/pyobs/utils/publisher/log.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/publisher/multi.py` & `pyobs_core-1.4.0/pyobs/utils/publisher/multi.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/simulation/camera.py` & `pyobs_core-1.4.0/pyobs/utils/simulation/camera.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/simulation/telescope.py` & `pyobs_core-1.4.0/pyobs/utils/simulation/telescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/simulation/world.py` & `pyobs_core-1.4.0/pyobs/utils/simulation/world.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/exptimeeval.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/exptimeeval.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/flatfielder.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/flatfielder.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/pointing/base.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/pointing/base.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/pointing/static.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/pointing/static.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/archive.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/archive.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/priorities/const.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/priorities/const.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/skyflats/scheduler.py` & `pyobs_core-1.4.0/pyobs/utils/skyflats/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/threads/checkabort.py` & `pyobs_core-1.4.0/pyobs/utils/threads/checkabort.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/threads/lockwithabort.py` & `pyobs_core-1.4.0/pyobs/utils/threads/lockwithabort.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/threads/threadwithreturnvalue.py` & `pyobs_core-1.4.0/pyobs/utils/threads/threadwithreturnvalue.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/time.py` & `pyobs_core-1.4.0/pyobs/utils/time.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/utils/types.py` & `pyobs_core-1.4.0/pyobs/utils/types.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/__init__.py` & `pyobs_core-1.4.0/pyobs/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/archivefile.py` & `pyobs_core-1.4.0/pyobs/vfs/archivefile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/file.py` & `pyobs_core-1.4.0/pyobs/vfs/file.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/httpfile.py` & `pyobs_core-1.4.0/pyobs/vfs/httpfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/localfile.py` & `pyobs_core-1.4.0/pyobs/vfs/localfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/memfile.py` & `pyobs_core-1.4.0/pyobs/vfs/memfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/smbfile.py` & `pyobs_core-1.4.0/pyobs/vfs/smbfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/sshfile.py` & `pyobs_core-1.4.0/pyobs/vfs/sshfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/tempfile.py` & `pyobs_core-1.4.0/pyobs/vfs/tempfile.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyobs/vfs/vfs.py` & `pyobs_core-1.4.0/pyobs/vfs/vfs.py`

 * *Files identical despite different names*

### Comparing `pyobs_core-1.3.7/pyproject.toml` & `pyobs_core-1.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 [tool.poetry]
 name = "pyobs-core"
 packages = [{ include = "pyobs" }]
-version = "1.3.7"
+version = "1.4.0"
 description = "robotic telescope software"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
-scipy = "^1.7"
-pandas = "^1.1"
-astropy = "^5.0"
+python = ">=3.9,<3.12"
+scipy = "^1.10.1"
+pandas = "^2.0.1"
+astropy = "^5.2.2"
 astroplan =  "^0.8"
-numpy = "^1.21"
-paramiko = "^2.8"
-pytz = "^2021.3"
+numpy = "^1.24.3"
+paramiko = "^3.1.0"
+pytz = "^2023.3"
 PyYAML = "^6.0"
-py-expression-eval = "^0.3"
-requests = "^2.26"
-ccdproc = "^2.2"
-photutils = "^1.2"
-lmfit = "^1.0"
-tornado = "^6.1"
-python-telegram-bot = "^13.8"
-typing-extensions = "^4.0"
+py-expression-eval = "^0.3.14"
+requests = "^2.30.0"
+ccdproc = "^2.4.0"
+photutils = "^1.7.0"
+lmfit = "^1.2.1"
+tornado = "^6.3.1"
+python-telegram-bot = "^20.2"
+typing-extensions = "^4.5.0"
 sep = [{ version = "^1.2", platform = "linux" }]
 python-daemon = [{ version = "^2.3", platform = "linux" }]
-astroquery = "^0.4"
-slixmpp = "^1.7"
-aiohttp = "^3.8"
-single-source = "^0.2"
+astroquery = "^0.4.6"
+slixmpp = "^1.8.3"
+aiohttp = "^3.8.4"
+single-source = "^0.3.0"
 asyncinotify = [{ version = "^2.0", platform = "linux" }]
-dbus-next = "^0.2"
+dbus-next = "^0.2.3"
+reproject = "^0.10.0"
 
 [tool.poetry.dev-dependencies]
-types-cryptography = "^3.3"
-types-enum34 = "^1.1"
-types-ipaddress = "^1.0"
-types-paramiko = "^2.7"
-types-pytz = "^2021.3"
-types-PyYAML = "^5.4"
-types-requests = "^2.25"
-types-setuptools = "^57.4"
-types-toml = "^0.10"
-types-tornado = "^5.1"
-mypy = "^0.920"
-pytest = "^6.2"
-pytest-asyncio = "^0.16"
+types-cryptography = "^3.3.23.2"
+types-enum34 = "^1.1.8"
+types-ipaddress = "^1.0.8"
+types-paramiko = "^3.0.0.9"
+types-pytz = "^2023.3.0.0"
+types-PyYAML = "^6.0.12.9"
+types-requests = "^2.29.0.0"
+types-setuptools = "^67.7.0.1"
+types-toml = "^0.10.8.6"
+types-tornado = "^5.1.1"
+mypy = "^1.2.0"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
 black = ">21.0"
-pre-commit = "^2.16"
+pre-commit = "^3.3.1"
 
 [tool.poetry.scripts]
 pyobs = 'pyobs.cli.pyobs:main'
 pyobsd = 'pyobs.cli.pyobsd:main'
 pyobsw = 'pyobs.cli.pyobsw:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target-version = ['py39']
+target-version = ['py39', 'py311']
```

### Comparing `pyobs_core-1.3.7/PKG-INFO` & `pyobs_core-1.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pyobs-core
-Version: 1.3.7
+Version: 1.4.0
 Summary: robotic telescope software
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: aiohttp (>=3.8,<4.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: astroplan (>=0.8,<0.9)
-Requires-Dist: astropy (>=5.0,<6.0)
-Requires-Dist: astroquery (>=0.4,<0.5)
+Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Requires-Dist: astroquery (>=0.4.6,<0.5.0)
 Requires-Dist: asyncinotify (>=2.0,<3.0) ; sys_platform == "linux"
-Requires-Dist: ccdproc (>=2.2,<3.0)
-Requires-Dist: dbus-next (>=0.2,<0.3)
-Requires-Dist: lmfit (>=1.0,<2.0)
-Requires-Dist: numpy (>=1.21,<2.0)
-Requires-Dist: pandas (>=1.1,<2.0)
-Requires-Dist: paramiko (>=2.8,<3.0)
-Requires-Dist: photutils (>=1.2,<2.0)
-Requires-Dist: py-expression-eval (>=0.3,<0.4)
+Requires-Dist: ccdproc (>=2.4.0,<3.0.0)
+Requires-Dist: dbus-next (>=0.2.3,<0.3.0)
+Requires-Dist: lmfit (>=1.2.1,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: paramiko (>=3.1.0,<4.0.0)
+Requires-Dist: photutils (>=1.7.0,<2.0.0)
+Requires-Dist: py-expression-eval (>=0.3.14,<0.4.0)
 Requires-Dist: python-daemon (>=2.3,<3.0) ; sys_platform == "linux"
-Requires-Dist: python-telegram-bot (>=13.8,<14.0)
-Requires-Dist: pytz (>=2021.3,<2022.0)
-Requires-Dist: requests (>=2.26,<3.0)
-Requires-Dist: scipy (>=1.7,<2.0)
+Requires-Dist: python-telegram-bot (>=20.2,<21.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: reproject (>=0.10.0,<0.11.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sep (>=1.2,<2.0) ; sys_platform == "linux"
-Requires-Dist: single-source (>=0.2,<0.3)
-Requires-Dist: slixmpp (>=1.7,<2.0)
-Requires-Dist: tornado (>=6.1,<7.0)
-Requires-Dist: typing-extensions (>=4.0,<5.0)
+Requires-Dist: single-source (>=0.3.0,<0.4.0)
+Requires-Dist: slixmpp (>=1.8.3,<2.0.0)
+Requires-Dist: tornado (>=6.3.1,<7.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
```

