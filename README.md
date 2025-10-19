# device_xiaomi_amethyst-twrp14-OSS
repo init -u https://github.com/nebrassy/platform_manifest_twrp_aosp.git -b twrp-14
repo sync

export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_amethyst-ap2a-eng
mka recoveryimage
