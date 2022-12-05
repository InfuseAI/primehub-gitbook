# How to configure PrimeHub

### What We Need?

PrimeHub repo clone is supposed to be at the local environment when PrimeHub installation.

```bash
git clone https://github.com/InfuseAI/primehub
```

### Where is Configuration File?

#### Multi-nodes

In terms of **multi-node**, the path to `primehub.yaml` is similar to below. Replace `<Kubernetes_cluster>` by the real case.

```bash
# Modify it with values of configuration
~/.primehub/config/<Kubernetes_cluster>/helm_override/primehub.yaml
```

#### Single-node

In terms of **single-node**, the path to `primehub.yaml` is as below since using _MicroK8s_

```bash
# Modify it with values of configuration
~/.primehub/config/microk8s/helm_override/primehub.yaml
```

### How to Apply New Configuration?

Run `primehub-install`, it will update PrimeHub according to the `primehub.yaml`. It will take minutes to finish the update.

```bash
# Go to install directory of PrimeHub repo
cd primehub/install
./primehub-install upgrade primehub
```
