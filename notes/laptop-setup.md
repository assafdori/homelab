## Turning my old laptop into a Kubernetes cluster.

I have an old laptop that I don't use anymore. It's a Lenovo ThinkPad with an Intel Core i7 CPU, 8GB of RAM, and a 500GB hard drive. I've been thinking about what to do with it, and I've decided to turn it into a Kubernetes cluster.

### Installing Ubuntu Server

I'm using [Ubuntu Server 22.04 LTS](https://ubuntu.com/server).

### Disabling lid close action

I don't want the laptop to go to sleep when I close the lid, so I need to disable the lid close action.

```bash
sudo vi /etc/systemd/logind.conf

# Uncomment the following line
HandleLidSwitch=ignore

# Uncomment the following line
HandleLidSwitchDocked=ignore
```

### Enabling SSH

I need to enable SSH.


### Installing Docker

I need to install Docker on the laptop.
