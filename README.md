
# Access

When creating instance, select new key and download key, e.g. `~/Downloads/ssh-key-2023-03-13.key`

```bash
# check permissions
ls -la ~/Downloads/ssh-key-2023-03-13.key
chmod 600 ~/Downloads/ssh-key-2023-03-13.key
```

# Intallation of dependencies

```bash
# update sys
sudo apt update
sudo apt upgrade

# add swap space (not only 1GB)
# https://linuxize.com/post/how-to-add-swap-space-on-ubuntu-20-04/
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
echo "/swapfile swap swap defaults 0 0" | sudo tee -a /etc/fstab
sudo swapon --show
```

# Docker

```bash
sudo apt install docker.io
```

# Python

```bash
sudo apt install python3 python3-venv
python3 -m venv venv
```