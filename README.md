# Ulefone Armor_3WT

follow repo init instructions for Omni Minimal TWRP (repo init command below) <br>

# Build Instructions

repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-9.0<br>
repo sync<br>
<br>
mkdir device<br>
mkdir device/ulefone<br>
cd device/ulefone<br>
git clone https://github.com/clewisit/android_device_ulefone_Armor_3WT Armor_3WT<br>
cd ../../<br>
<br>
export ALLOW_MISSING_DEPENDENCIES=true<br>
source build/envsetup.sh<br>
lunch omni_Armor_3WT-eng<br>
mka recoveryimage<br>


# Troubleshooting

Python3 errors
fix external/clang/clang-version-inc.py  change all print to print(). change iteritems() to items()<br>
fix bionic/libc/fs_config_generator.py   change all print to print().  change ConfigParser to configparser. change iteritems to items
