# grub


In the GRUB menu, find the kernel line starting with `linux /boot/` and add `init=/bin/bash` at the end of the line.


Press `CTRL+X` to save.

Mount the file system:
```bash
mount -o remount,rw /
```



https://www.layerstack.com/resources/tutorials/Resetting-root-password-for-Linux-Cloud-Servers-by-booting-into-Single-User-Mode



in the `linux` line change read only to:
```
ro -> 
```
