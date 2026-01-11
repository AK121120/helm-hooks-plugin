# helm-hooks-plugin

Helm 4 plugin for [helm-hooks](https://github.com/AK121120/helm-hooks).

## Installation

```bash
helm plugin install https://github.com/AK121120/helm-hooks-plugin
```

## Usage

```bash
helm install myapp ./chart --post-renderer helm-hooks
helm upgrade myapp ./chart --post-renderer helm-hooks
```

## Version

```bash
helm-hooks version
```

## Alternative Installation (Helm 3)

For Helm 3 users, download the binary directly:

```bash
# Linux
curl -sSL https://github.com/AK121120/helm-hooks/releases/latest/download/helm-hooks-linux-amd64 -o helm-hooks
chmod +x helm-hooks

# Use with --post-renderer
helm install myapp ./chart --post-renderer ./helm-hooks
```

Or pull from container registry:
```bash
docker pull quay.io/gkananthakrishna/helm-hooks:latest
```

## Links

- [Main Repository](https://github.com/AK121120/helm-hooks)
- [Releases](https://github.com/AK121120/helm-hooks/releases)
- [Container Image](https://quay.io/gkananthakrishna/helm-hooks)
