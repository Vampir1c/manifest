beanstalk-manifest
======================

Local Manifest for GraberROMs - Based off Beanstalk. 
Only use this manifest for our officially supported devices.

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

Make a build directory:

	mkdir Andoid (or whatever name you choose)
	cd Android (or the name  you chose)
	mkdir .repo/local_manifests

Init repo only for Beanstalk base first:

    repo init -u git://github.com/scotthartbti/android.git -b kk44

Sync up once:

    repo sync

Then download additional repo's for officially supported devices:

    curl -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.github.com/GraberRoms/manifest/cm-11.0/kitstalk.xml
 
    	( or Download: https://github.com/GraberRoms/manifest/blob/cm-11.0/roomservice.xml
		and place it in ~/Android/.repo/local_manifests/kitstalk.xml (or ~/'name you chose'/.repo/local_manifests/ )

Then to sync up:

    repo sync
