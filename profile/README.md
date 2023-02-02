## Overview
This is a mirror copy of AOSP

## Building AOSP

|Config                       |Build Verified  |
|-----------------------------|----------------|
|aosp_arm64-user              | x              |
|aosp_arm64-userdebug         | x              |

```bash
# Setup the environment.
source build/envsetup.sh

# Choose a lunch target.   For example, 'lunch aosp_arm64-userdebug', or just use lunch directly.
lunch aosp_arm64-userdebug

# Compile.  (Substitute the TARGET_PRODUCT and TARGET_BUILD_VARIANT, as needed)
build/soong/soong_ui.bash --make-mode TARGET_PRODUCT=aosp_arm64 TARGET_BUILD_VARIANT=userdebug dist
```

## Android Reference

- [Building Android](https://source.android.com/docs/setup/build/building)
- [Android Build Environment](https://source.android.com/docs/setup/start/initializing)
