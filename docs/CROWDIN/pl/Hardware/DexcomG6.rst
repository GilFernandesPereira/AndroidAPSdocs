Dexcom G6
************
Basics first
===============

* Follow general CGM hygiene and setting sensor recommendation `here <../Hardware/GeneralCGMRecommendation.html>`_.
* For G6 transmitters manufactured after fall/end of 2018 please make sure to use one of the `latest nightly built xDrip+ versions <https://github.com/NightscoutFoundation/xDrip/releases>`_. Those transmitters have a new firmware and latest stable version of xDrip+ (2019/01/10) cannot deal with it.

General hints for looping with G6
================================

Oczywiste jest, że korzystanie z G6 jest być może nieco bardziej skomplikowane niż wygląda to na początku. Aby bezpiecznie z niego korzystać, należy pamiętać o kilku punktach: 

* If you are using the native data with the calibration code in xDrip or Spike, the safest thing to do is not allow preemptive restarts of the sensor.
* If you must use preemptive restarts, then make sure you insert at a time of day where you can observe the change and calibrate if necessary. 
* If you are restarting sensors, either do it without the factory calibration for safest results on days 11 and 12, or ensure you are ready to calibrate and keep an eye on variation.
* Pre-soaking of the G6 with factory calibration is likely to give variation in results. Jeśli pracujesz z namaczaniem wstępnym, aby uzyskać najlepsze wyniki, prawdopodobnie będziesz musiał skalibrować sensor.
* If you aren’t being observant about the changes that may be taking place, it may be better to revert to non-factory-calibrated mode and use the system like a G5.

To learn more about the details and reasons for these recommendations read the `complete article <http://www.diabettech.com/artificial-pancreas/diy-looping-and-cgm/>`_ published by Tim Street at `www.diabettech.com <http://www.diabettech.com>`_.

If using G6 with xdrip+
===============================

* If not already set up then download `xdrip <https://github.com/NightscoutFoundation/xDrip>`_ and follow instructions on nightscout (`G5 <http://www.nightscout.info/wiki/welcome/nightscout-with-xdrip-and-dexcom-share-wireless/xdrip-with-g5-support>`_).
* Select xdrip in ConfigBuilder (setting in AndroidAPS).
* Adjust settings in xDrip+ according to `xDrip+ settings page <../Configuration/xdrip.html>`_
* If AAPS does not receive BG values when phone is in airplane mode use `Identify receiver` as describe on `xDrip+ settings page <../Configuration/xdrip.html>`_.

If using G6 with patched Dexcom app
=========================================================
* Download the apk from `https://github.com/dexcomapp/dexcomapp <https://github.com/dexcomapp/dexcomapp>`_, and choose the version that fits your needs (mg/dl or mmol/l version, G6).

   * Folder 2.3 is for users of AndroidAPS 2.3, folder 2.4 for users of AAPS 2.4.
   * Open https://play.google.com/store/search?q=dexcom%20g6 on your computer. Region will be visible in URL.
   
   .. image:: ../images/DexcomG6regionURL.PNG
     :alt: Region in Dexcom G6 URL

* Stop sensor and uninstall the original Dexcom app, if not already done.
* Install downloaded apk
* Start sensor
* Select Dexcom App (patched) in ConfigBuilder (setting in AndroidAPS).

Troubleshooting G6
====================

General Troubleshoothing for CGMs can be found `here <./GeneralCGMRecommendation.html#Troubleshooting>`_.

New transmitter with running sensor
--------------------------------------
If you happen to change transmitter during a running sensor session you might try to remove the transmitter without damaging the sensor mount. A video can be found at `https://youtu.be/AAhBVsc6NZo <https://youtu.be/AAhBVsc6NZo>`_.


