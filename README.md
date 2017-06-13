# MicroGFlashableZip
This repository contains flashable zip files for the MicroG GMS Core Project for Android / LineageOS

This are flashable zip files for the microG project. 
MicroGCompleteFOSS.zip requires an arm64 LineageOS 14.1
MicroGCompleteFOSSUniversalArm64.zip requires an arm64 Android 7 (Android 6 should work too, but is untested)

MicroGCompleteFOSS.zip  installs the addonsu for root (requires LineageOS 14.1):
https://download.lineageos.org/extras

Both zip files

- apply NanoMod-patcher for signature faking
https://github.com/Nanolx/NanoMod 
https://forum.xda-developers.com/apps/magisk/module-nanomod-5-0-20170405-microg-t3584928
https://www.androidfilehost.com/?a=show&w=files&flid=150729

- install F-Droid client 0.102.3 (later versions got an unusable cluttered user interface)
https://f-droid.org/repo/org.fdroid.fdroid_102350.apk
https://f-droid.org/repo/org.fdroid.fdroid_102350_src.tar.gz

- install Maps API v1
https://forum.xda-developers.com/showthread.php?t=1715375
https://github.com/mar-v-in/MapsAPI

- install microG GMSCore
https://github.com/microg/android_packages_apps_GmsCore
https://github.com/microg 
https://forum.xda-developers.com/android/apps-games/app-microg-gmscore-floss-play-services-t3217616

- install microG GsfProxy
https://github.com/microg/android_packages_apps_GsfProxy
https://github.com/microg 
https://forum.xda-developers.com/android/apps-games/app-microg-gmscore-floss-play-services-t3217616

- install UnifiedNlp Backend that uses Apple's service to resolve wifi locations
https://github.com/microg/AppleWifiNlpBackend

- install UnifiedNlp geocoder backend
https://github.com/microg/NominatimGeocoderBackend

- install microG FakeStore
https://github.com/microg/android_packages_apps_FakeStore
https://github.com/microg 
https://forum.xda-developers.com/android/apps-games/app-microg-gmscore-floss-play-services-t3217616

- apply patches to prevent Google Play Store auto updating itself (in case you install this instead of FakeStore), 
since at the moment only Google Play Store 5.1.11 works flawlessly with MicroG GMSCore

The zip file is already prepared for manual inclusion of the original Google Play Store, the Swipe library and Sound search for Google play. 
To install these, open the zip file with 7zip and put the apk file in the corresponding folder.

Sound search for Google play: data/app/com.google.android.ears/base.apk AND external_sd/app/com.google.android.ears/base.apk
Swipe library: system/lib64/libjni_latinimegoogle.so
Google Play Store: system/priv-app/Phonesky/Phonesky.apk

Sources for parts under a copyleft license can be found in the SourceCode folder of the MicroGCompleteSources.zip file. 
You can also find the links to the other projects there. 

