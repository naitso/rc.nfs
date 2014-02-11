rc.nfs
======

About
-----

This bash script help a linux users to mount a NFS share on your linux system

How to use?
-----------

Save and edit the script, edit it according to your needs (change the top variables)
Now you can change file mode bits:
	
	chmod +x ./rc.nfs

Now you can call the script 
	
	./rc.nfs

or if you prefer use cron to check and "automount" the share every X minute, see the example below

	Run hourly cron jobs at 30 minutes after the hour:
	30 * * * * /path/of/rc.nfs 1> /dev/null


NOTE
-----

This script must be executed by root (or sudo) users that have the right permissions to mount something to the system.


Software Required
-----------------

This software must be installed on your system before to execute this script

nc (Netcat network utility)
util-linux (a huge collection of essential utilities)
nfs-utils (Network File System daemons and utilities)


