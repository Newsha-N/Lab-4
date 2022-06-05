# Hey! I'm Filing Here

Building a file system similar to the Linux ext2 file system.
## Building
    'make'
## Running

./ext2-create 
dumpe2fs cs111-base.img 
fsck.ext2 cs111-base.img 
mkdir mnt 
sudo mount -o loop cs111-base.img mnt 

total 3
 2 drwxr-xr-x 3    0    0 1024 Jun  4 17:12 .
12 drwxrwx--- 1    0  109  416 Jun  4  2022 ..
13 lrw-r--r-- 1 1000 1000   11 Jun  4 17:12 hello -> hello-world
12 -rw-r--r-- 1 1000 1000   12 Jun  4 17:12 hello-world
11 drwxr-xr-x 2    0    0 1024 Jun  4 17:12 lost+found
 
## Cleaning up
sudo umount mnt 
rmdir mnt
make clean 