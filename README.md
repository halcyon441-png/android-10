# TWRP Device Tree for the Samsung Galaxy A50s (a50sxx) (Android 10 Q)

## How-to install dependencies
```
sudo apt install -y bison build-essential g++-multilib git make python zip openjdk-8-jdk screen libtinfo5 libncurses5
```

## How-to clone source and device tree:

```
mkdir -p ~/twrp && cd ~/twrp
```
```
repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-10.0
```
```
repo sync
```
```
git clone https://github.com/halcyon441-png/android-10.git    device/samsung/a50sxx
```
## How-to build:

```
export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch omni_a50sxx-eng; mka recoveryimage
```
Сompilation result is in ```twrp/out/target/product/a50sxx```
# ADD BUSYBOX IN /.../twrp/external/ FOLDER.


