# snap-test

```bash
export SNAPCRAFT_ENABLE_EXPERIMENTAL_EXTENSIONS=1
sudo /bin/bash -c "echo "net.ipv4.conf.all.forwarding=1" > /etc/sysctl.d/99-forwarding.conf"
sudo systemctl stop docker.service
sudo systemctl stop docker.socket
sudo systemctl restart systemd-sysctl
```