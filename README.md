# Krew Index

Custom [Krew](https://krew.sigs.k8s.io/) plugin index for [KubeWise](https://github.com/tochemey/kubewise) — the Kubernetes cost and performance "what-if" simulator.

## Setup

Add this index to krew:

```bash
kubectl krew index add kubewise https://github.com/tochemey/krew-index.git
```

## Installation

```bash
kubectl krew install kubewise/whatif
```

## Available Plugins

| Plugin    | Description                                          |
|-----------|------------------------------------------------------|
| `whatif`  | Kubernetes cost and performance what-if simulator    |

## Usage

Once installed, use `kubectl whatif` to snapshot your cluster, simulate changes, and see cost impact:

```bash
kubectl whatif snapshot
kubectl whatif rightsize
kubectl whatif consolidate --node-type=m6i.xlarge
kubectl whatif spot
```

For full documentation, see the [KubeWise README](https://github.com/tochemey/kubewise).

## License

Apache License 2.0. See [LICENSE](LICENSE) for details.
