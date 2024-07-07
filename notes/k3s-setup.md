## Setting up K3s
I'm using [K3s](https://k3s.io/) to set up a Kubernetes cluster on the laptop. K3s is a lightweight Kubernetes distribution that is easy to install and manage.


### Installing K3s
```bash
curl -sfL https://get.k3s.io | sh -
```

### Troubleshooting

If encountering issues with localhost:8080 connection refused:
```bash
Faulty kubeconfig file?
UFW Disabled?
```
