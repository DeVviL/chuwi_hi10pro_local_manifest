Local manifests to build CyanogenMod/LineageOS 14 for [Chuwi Hi10 Pro]

How to build:
-------------

Initialize repo:

    repo init -u git://github.com/LineageOS/android.git -b cm-14.1
    curl --create-dirs -L -o .repo/local_manifests/manifest_intel_cherrytrail.xml -O -L https://raw.githubusercontent.com/DeVviL/android_local_manifest/cm-14.1/manifest_intel_cherrytrail.xml
    repo sync

### Chuwi Hi10 Pro:

    curl -L -o .repo/local_manifests/manifest_intel_chuwi_hi10pro.xml -O -L https://raw.githubusercontent.com/DeVviL/android_local_manifest/cm-14.1/manifest_intel_chuwi_hi10pro.xml
    repo sync

Compile:

    . build/envsetup.sh
    brunch chuwi_hi10pro

