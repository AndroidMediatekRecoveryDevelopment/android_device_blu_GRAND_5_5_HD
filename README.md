## TWRP device tree for BLU Grand 5.5 HD (GRAND_5_5_HD)

Add to `.repo/local_manifests/GRAND_5_5_HD.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/blu/GRAND_5_5_HD" name="android_device_blu_GRAND_5_5_HD" remote="hejsekvojtech" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_GRAND_5_5_HD-eng
make -j5 recoveryimage
```
