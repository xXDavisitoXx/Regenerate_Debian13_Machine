# Regenerate_Debian13_Machine

# Cambiar hostname
```bash
hostnamectl set-hostname NUEVO_HOSTNAME
```

# Actualizar /etc/hosts
```bash
nano /etc/hosts
```

# Regenerar machine-id
```bash
rm -f /etc/machine-id
```
```bash
systemd-machine-id-setup
```

# Regenerar claves SSH
```bash
rm -f /etc/ssh/ssh_host_*
```
```bash
dpkg-reconfigure openssh-server
```

# Verificar machine-id nuevo
```bash
cat /etc/machine-id
```

# Verificar hostname
```bash
hostnamectl
```

# Reiniciar
```bash
reboot
```
