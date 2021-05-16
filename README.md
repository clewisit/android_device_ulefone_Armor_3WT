# android_device_ulefone_Armor_3WT

follow repo init instructions for Omni Minimal TWRP <br>
<br>
In your TWRP build folder, create a roomservice.xml file in .repo/local_manifests.  Edit the file and give it the following contents: 
<code>
  <?xml version="1.0" encoding="UTF-8"?>
<manifest>
    <project name="clewisit/android_device_ulefone_Armor_3WT" path="device/ulefone/Armor_3WT" remote="github" revision="twrp-9.0" />
</manifest>
</code>

# Build Instructions

repo sync
export ALLOW_MISSING_DEPENDENCIES=true<br>
source build/envsetup.sh<br>
lunch omni_Armor_3WT-eng<br>
mka recoveryimage<br>
