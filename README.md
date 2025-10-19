# device_xiaomi_amethyst-twrp14-OSS


## Getting Started ##
To initialize your local repository using the AOSP trees to build TWRP, use a command like this:

    repo init -u https://github.com/nebrassy/platform_manifest_twrp_aosp.git -b twrp-14

Then to sync up:

    repo sync
	
Then to setup the build:

     cd <source-dir>; export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_amethyst-ap2a-eng
	 
The build target :
- Recovery partition: `mka recoveryimage`