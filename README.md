# mkkubeconfig

Generate a usable `KUBECONFIG` file for a given service account

## Usage

```bash
mkkubeconfig <namespace> <service-account> > "~/.kube/myserviceaccount.yaml"

export KUBECONFIG="~/.kube/myserviceaccount.yaml"
kubectl get pods
```

## Installation

### Manual

Copy `mkkubeconfig` into the `bin` directory of your choice

### Chef Habitat

```bash
hab pkg install --binlink jarvus/mkkubeconfig
```

## Acknowledgements

Adapted from <https://gist.github.com/ericchiang/d2a838ddad3f44436ae001a342e1001e>
