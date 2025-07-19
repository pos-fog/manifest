# PixelOS

## Getting Started

To get started with the PixelOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

To initialize your local repository, use command:

```bash
repo init -u https://github.com/pos-fog/manifest.git -b sixteen --git-lfs
```

Then sync up:

```bash
repo sync -j14 -c --optimized-fetch --no-clone-bundle --no-tags
```

## Building the System

Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
breakfast devicecodename
```

Start compilation

```bash
mka bacon
```

---

Note:  

**aosp_target_release**: bp2a (change if required)
**buildtype**: user, userdebug, eng


