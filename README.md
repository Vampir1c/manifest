beanstalk-manifest (or any other CM Base)
======================

Local Manifest for (these) CM Base ROMs/Officially Supported devices.

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

Make a build directory:

	mkdir Andoid (or whatever name you choose)
	cd Android (or the name  you chose)
	mkdir .repo/local_manifests

To utilize this manifest as a local for CM based ROMs with (these) CM supported devices, use commands like these:

    
    curl -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.github.com/pjgraberTWO/beanstalk-manifest/cm-11.0/roomservice.xml
 
    	( or Download: https://github.com/pjgraberTWO/beanstalk-manifest/blob/cm-11.0/roomservice.xml
		and place it in ~/Android/.repo/local_manifests/roomservice.xml (or ~/'name you chose'/.repo)

Then to sync up:

    repo sync
