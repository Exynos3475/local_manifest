LineageOS 14.1 for Exynos3475 devices
------------------------------------

Create directories

	$ mkdir cm-14.1
	$ cd cm-14.1

Init the base manifest

	$ repo init -u git://github.com/LineageOS/android.git -b cm-14.1
  
Add the local manifest

  Take the xml file for your device and copy it to .repo/local_manifests/

Then sync up with this command:

	$ repo sync --force-sync -q

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_DEVICE-userdebug
	$ mka bacon
