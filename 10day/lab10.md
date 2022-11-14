# Adding our first disk and partitioning it.
1. Open Virtualbox application, select your virtual machine and open it's settings, select Storage part from the left, and add a virtual disk(5GB is enough for now) to the Controller:SATA  (note: your vmachine should be turned off, before adding extra disk)
2. Now ssh to your virtual machine, and list block devices. 
Virtual hard disk that you added usually called /dev/sdb, when you list devices.
3. Using gdisk /dev/sdb, open gdisk command prompt, type 'm' to get help.
   a. Print the partition table to see some information about your device.
   b. Create a new partition, enter partition number, skip first sector, specify last sector
like +500M or +1G. Use default hex code, 8300. 
   c. Type 'p' to print created partition.
   d. Type 'w' to save and exit.
   f. Using lsblk list your block devices again, and you should see now your sdb1 partition.
4. Using mkfs command create a filesystem on /dev/sdb1. Use xfs or ext4 filesystem type.
5. Using lsblk -f list block devices with fstype.
6. Create a folder in /mnt/ directory, and attach your partition to this folder.
7. 
