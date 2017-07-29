## TWRP device tree for Symphony Xplorer V80 (V80)

Add to `.repo/local_manifests/V80.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/symphony/V80" name="android_device_symphony_V80" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_V80-eng
make -j5 recoveryimage
```
