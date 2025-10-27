# Crossplane Keycloak Playground

For the playground we use [Devbox](https://www.jetify.com/docs/devbox/) and [Task](https://taskfile.dev/).

### Prerequisites

1. Install Devbox `curl -fsSL https://get.jetify.com/devbox | bash`
2. Clone this repository and navigate to it
3. Run `devbox shell` to start and enter the development environment

### Start the playground with [kind](https://kind.sigs.k8s.io/)

**1. Setup k8s cluster with keycloak and crossplane**
```bash
task setup-base-cluster
```

**2. Deploy demo Keycloak Realm [examples/kc-realm.yaml](/examples/kc-realm.yaml)**
```bash
kubectl apply -f examples/kc-realm.yaml
```
