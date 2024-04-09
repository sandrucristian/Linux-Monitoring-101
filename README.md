# Linux monitor

````
top
````

To manage and view disk partitions in Linux, you can use several commands. Here are some of the most commonly used ones:

**fdisk**: A command-line utility to view and manage disk partitions. Use sudo fdisk -l to list all partitions on all disks.
lsblk: Lists all block devices and their partitions along with sizes. Simply run lsblk to see the information.
df: Displays the amount of disk space used and available on filesystems. Use df -h for a human-readable format.
parted: A tool to create, resize, move, and copy partitions. Invoke it with sudo parted followed by disk operations commands.