LineageOS 17.1 for Exynos3475 devices
------------------------------------

Create directories

	$ mkdir lineage-17.1
	$ cd lineage-17.1

Init the base manifest

**For some reason, we need to use older manifest for now**

	$ repo init -u git://github.com/wecouldcalliteven/android.git -b lineage-17.1
  
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
