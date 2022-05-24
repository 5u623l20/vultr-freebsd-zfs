# FreeBSD ZFS Image for Vultr

This script generates FreeBSD zfs image for [Vultr](https://vultr.com).

☣️ This script must be run in a FreeBSD system which is running on UFS or do not have a zpool named `zroot`.

The script is self explanatory. Just change your `PASSWORD` and `SSH_KEY`.

Once the image is created:
1. Host the image in a webserver
2. Upload the image to Vultr Products->Snapshots->Upload snapshot from remote machine
3. Grab a coffee
4. Create a new VPS Products->Deploy a new server In the Server Image click snapshot; Select the snapshot that was uploaded. Click Deploy now.
5. [Resize the Disk](https://www.vultr.com/docs/resize-zfs-storage-pool-on-freebsd-trueos/) after the server has been provisioned.
6. Enjoy the server. 
