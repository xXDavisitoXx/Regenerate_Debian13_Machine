# Regenerate_Debian13_Machine

# Cambiar hostname
hostnamectl set-hostname NUEVO_HOSTNAME

# Actualizar /etc/hosts
nano /etc/hosts

# Regenerar machine-id
rm -f /etc/machine-id
systemd-machine-id-setup

# Regenerar claves SSH
rm -f /etc/ssh/ssh_host_*
dpkg-reconfigure openssh-server

# Verificar machine-id nuevo
cat /etc/machine-id

# Verificar hostname
hostnamectl

# Reiniciar
reboot
