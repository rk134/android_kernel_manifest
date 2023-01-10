[<center><img src="https://raw.githubusercontent.com/sourajitk/STX-Logo/main/stx-2021-kernel.png" height="50%" width="50%;" /></center>](https://github.com/StatiXOS)

## Repo Init ##
```bash
repo init -u https://github.com/rk134/android_kernel_manifest.git -b android-msm-RMX3360-5.4-android13
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Build ##
For Clang builds
```bash
BUILD_CONFIG=kernel/msm-5.4/build.config.msm.lahaina VARIANT=qgki LTO=full BUILD_KERNEL=1 build/build.sh
```
### Submitting Patches ###

Please refer to this for submitting patches: https://github.com/StatiXOS/android_manifest#submitting-patches
