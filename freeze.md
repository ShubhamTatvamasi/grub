# Freeze

Change grub settings:
```bash
sudo vim /etc/default/grub
```

Update grub settings:
```bash
sudo update-grub
```

Upload crash logs:
```bash
journalctl -rb -1 | nc termbin.com 9999
```

https://danstechjourney.com/ubuntu-desktop-freezing-after-suspend/

