# grub


In the GRUB menu, find the kernel line starting with `linux /boot/` and add `init=/bin/bash` at the end of the line.



```bash
mount -o remount,rw /
```




in the `linux` line change read only to:
```
ro -> 
```
