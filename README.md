# Ulefone Armor_3WT

follow repo init instructions for Omni Minimal TWRP (repo init command below) <br>

# Build Instructions

repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0
repo sync<br>

mkdir device
mkdir device/ulefone
cd device/ulefone
git clone https://github.com/clewisit/android_device_ulefone_Armor_3WT Armor_3WT
cd ../../

export ALLOW_MISSING_DEPENDENCIES=true<br>
source build/envsetup.sh<br>
lunch omni_Armor_3WT-eng<br>
mka recoveryimage<br>
