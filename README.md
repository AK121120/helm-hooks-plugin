# helm-hooks-plugin

Helm plugin for [helm-hooks](https://github.com/AK121120/helm-hooks) - per-hook weights and environment injection.

## Installation (Helm 4)

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
./bin/helm-hooks version
```

## Installation (Helm 3)

For Helm 3, download the binary from GitHub releases:

```bash
# Linux (amd64)
curl -L https://github.com/AK121120/helm-hooks/releases/download/v0.5.0/helm-hooks-linux-amd64 -o helm-hooks
chmod +x helm-hooks

# macOS (arm64)
curl -L https://github.com/AK121120/helm-hooks/releases/download/v0.5.0/helm-hooks-darwin-arm64 -o helm-hooks
chmod +x helm-hooks

# Use with --post-renderer
helm install myapp ./chart --post-renderer ./helm-hooks
```

## Links

- [Main Repository](https://github.com/AK121120/helm-hooks)
- [Releases](https://github.com/AK121120/helm-hooks/releases)
