[<center><img src="https://raw.githubusercontent.com/sourajitk/STX-Logo/main/stx-2021-kernel.png" height="50%" width="50%;" /></center>](https://github.com/StatiXOS)

## Repo Init ##
```bash
repo init -u https://github.com/JackA1ltman/android_kernel_manifest.git -b oneplus/sm8350_b_16.0.0_oneplus9rt
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Build ##
For Clang builds
```bash
BUILD_CONFIG=kernel/msm-5.4/build.config.msm.martini VARIANT=qgki LTO=full BUILD_KERNEL=1 build/build.sh
```
