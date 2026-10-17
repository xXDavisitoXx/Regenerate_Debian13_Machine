# Regenerate_Debian13_Machine

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
