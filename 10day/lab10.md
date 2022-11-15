# Adding our first disk and partitioning it.
Before implementing steps below, turn off your virtual machine and create a new snapshot, to avoid losing data and current configurations.
1. Open Virtualbox application, select your virtual machine and open it's settings, select Storage part from the left, and add a virtual disk(10 GB is enough for now) to the Controller:SATA  (note: your vmachine should be turned off, before adding extra disk)
2. Now ssh to your virtual machine, and list block devices. 
Virtual hard disk that you added usually called /dev/sdb(or it might be sdc,sdd...,if you already have sdb disk), when you list devices.
3. Using gdisk /dev/sdb, open gdisk command prompt, type 'm' to get help.
   a. Print the partition table to see some information about your device.
   b. Create a new partition, enter partition number, skip first sector, specify last sector
like +500M or +1G. Use default hex code, 8300. 
   c. Type 'p' to print created partition.
   d. Type 'w' to save and exit.
   f. Using lsblk list your block devices again, and you should see now your sdb1 partition.
4. Using mkfs command build a filesystem on /dev/sdb1. Use xfs or ext4 filesystem type.
5. Using lsblk -f list block devices with fstype.
6. Create a folder in /mnt/ directory, and mount your partition to this folder.
7. Open /etc/fstab and add a line to permanently mount your created partition to a folder, otherwise
your mounted partition will unmount after restarting virtual machine.
8. No with the command 'df' check the space usage of the new partition and specify the option to display the filesystem type.

# Creating LVM group. TAB completion and manuals help a lot.
1. Open gdisk again, and create 2nd partition,skip first sector, last sector size = 5 GB, choose partition type = Linux LVM. List partitions in gdisk to check the result, then write table and exit gdisk.
2. Check your new partition with lsblk, if it doesn't show up, type partprobe command, it will inform OS of partition table changes. Now it should appear.
3. Using pvcreate command prepare your partition to be used by LVM.
4. Display physical volumes using pvs, to check that you initialized physical volume for Volume group usage.
5. Using vgcreate create volume group.
6. List Volume groups using vgs command.
7. Using lvcreate command create logical volume, size should be 1GB. 
8. List logical volumes using lvs. 
9. Build a filesystem on your logical volume using mkfs command(logical volumes are located in /dev/mapper/ folder), filesystem type should be xfs or ext4.
10. Create a folder in home directory and mount your lvolume to this folder. 
11. Now using lvextend take all space from Volume group and add to your logical volume using -l option.
12. Resize your filesystem on logical volume, using resize2fs(for ext4) or xfs_growfs(for xfs).
13. Now check the result using df -h if size changed.

# Extending Volume group
1. Create 3rd partition, choose size and partition type should be Linux LVM. Write and exit gdisk.
2. Using pvcreate select created partition and add to physical volumes.
3. Using vgextend add new physical volume(partition)to previously created volume group not the system one. 
4. List volume groups and look at the #PV column, it should change.
