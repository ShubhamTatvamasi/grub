# grub


### Reset root password

1. Press `Esc` key to enter into the grub menu.

2. From the GRUB boot prompt, press the `E` button to edit the first boot option.

3. In the GRUB menu, find the kernel line starting with `linux /boot/` and edit `ro` to:
    ```
    rw init=/bin/bash
    ```

4. Press `CTRL+X` to save.


5. Change the password:
    ```bash
    passwd
    ```

6. Reboot:
    ```bash
    reboot -f
    ```


https://www.layerstack.com/resources/tutorials/Resetting-root-password-for-Linux-Cloud-Servers-by-booting-into-Single-User-Mode


