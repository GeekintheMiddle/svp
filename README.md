# svp
Qemu/KVM server on OVH network

### How to install
```
apt-get update & apt-get install qemu-kvm
cd ~
git clone https://github.com/GeekintheMiddle/svp.git
cd svp
mkdir /etc/svp
rsync -av ~/svp/vms /etc/svp/
cp svp /usr/bin/
chmod +x /usr/bin/svp
```

### How to use
```
usage: svp [-h] [--start STARTVM] [--stop STOPVM]

SVP Virtual Machine Manager

optional arguments:
  -h, --help       show this help message and exit
  --start STARTVM  Start Virtual Machine
  --stop STOPVM    Stop Virtual Machine
```

### Examples
```
# Start virtual machine
svp --start template
# Stop virtual machine
svp --stop template
```

## Authors
* **Sven Mollinga** - [GeekintheMiddle](https://www.geekinthemiddle.com)
