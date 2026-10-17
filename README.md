# Regenerate_Debian13_Machine
<p align="center">
  <img src="Images/Regenerate-Debian.Cover.jpg" alt="Regenerate-Debian-Cover" width="100%">
</p>
### Change hostname
```bash
hostnamectl set-hostname NUEVO_HOSTNAME
```

### Update /etc/hosts
```bash
nano /etc/hosts
```

### Regenerate machine-id
```bash
rm -f /etc/machine-id
```
```bash
systemd-machine-id-setup
```

### Regenerate SSH Keygen
```bash
rm -f /etc/ssh/ssh_host_*
```
```bash
dpkg-reconfigure openssh-server
```

### Verifiy  new machine-id
```bash
cat /etc/machine-id
```

### Verify hostname
```bash
hostnamectl
```

### Reboot machine
```bash
reboot
```
