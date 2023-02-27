# Freeze

Change grub settings:
```bash
sudo vim /etc/default/grub
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


https://danstechjourney.com/ubuntu-desktop-freezing-after-suspend/

