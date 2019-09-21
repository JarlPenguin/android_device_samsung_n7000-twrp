## TWRP device tree for Samsung Galaxy Note (International)
## n7000

Add to `.repo/local_manifests/n7000.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="JarlPenguin/android_device_samsung_n7000" path="device/samsung/n7000" remote="github" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_n7000-eng
mka recoveryimage
```

Kernel source: https://github.com/LineageOS/android_kernel_samsung_smdk4412/tree/cm-14.1
