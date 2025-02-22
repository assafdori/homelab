## Setting up an old laptop as an Ubuntu server that can run Kubernetes.

I have an old laptop that I don't use anymore. It's a Lenovo ThinkPad with an Intel Core i7 CPU, 8GB of RAM, and a 500GB hard drive. I've been thinking about what to do with it, and I've decided to turn it into a Kubernetes cluster.

### Installing Ubuntu Server

I'm using [Ubuntu Server 22.04 LTS](https://ubuntu.com/server).

### Setting up the network

I need to set up the network. I'm going to use a static IP address.

### Disabling lid close action

I don't want the laptop to go to sleep when I close the lid, so I need to disable the lid close action.

```bash
sudo vi /etc/systemd/logind.conf

# Uncomment the following line
HandleLidSwitch=ignore

# Uncomment the following line
HandleLidSwitchDocked=ignore

# Restart the systemd-logind service
sudo service systemd-logind restart
```

### Enabling SSH

I need to enable SSH.


### Installing Docker

I need to install Docker on the laptop.
