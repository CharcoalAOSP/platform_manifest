# Welcome to Crescence!

## Getting Started

To initialize your local repository, run:

```bash
repo init --depth=1 -u https://github.com/Crescence-AOSP/platform_manifest.git -b 26h1 --git-lfs
```

Then, sync the repository:

```bash
repo sync --force-sync -j$(nproc --all)
```

## Building the System

Initialize the build environment by sourcing the envsetup.sh script:

```bash
source build/envsetup.sh
```

After cloning the device-specific sources, use breakfast to configure the build for your device:

```bash
breakfast device
```

Then, start the compilation:

```bash
m release
```

## Submitting Patches
To submit your patches, head to [Crescence Review](https://crescence-review.lunia0251.moe/).
