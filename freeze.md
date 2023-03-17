# Freeze

Change grub settings:
```bash
sudo vim /etc/default/grub
```

Update the `GRUB_CMDLINE_LINUX_DEFAULT` variable:
```bash
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash amd_iommu=on iommu=pt processor.max_cstate=5 rcu_nocbs=0_11"

GRUB_CMDLINE_LINUX_DEFAULT="quiet splash amd_iommu=off"
```

Update grub settings:
```bash
sudo update-grub
```

Check grub service status:
```bash
systemctl status grub-initrd-fallback
```

Upload crash logs:
```bash
journalctl -rb -1 | nc termbin.com 9999
```

Check the suspend service status:
```bash
systemctl status systemd-suspend
```

Check the login service status:
```bash
systemctl status systemd-logind
```

https://danstechjourney.com/ubuntu-desktop-freezing-after-suspend/

