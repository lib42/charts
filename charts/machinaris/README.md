# Machinaris Helm Chart

This is a Helm Chart for [Machinaris](https://machinaris.app). A Chia[-fork] farmer & plotter with Web UI.

This chart is not maintained by Machinaris official maintainer!

## What it does

- Simple Setup by sharing a global configuration over all forks
- StatefulSet for every Chia-fork enabled + API Service
- Prometheus metrics export using sidecar exporter
- Automatic environment configuration for machinaris
- Ingress support for Web UI
- mnemonic saved as Secret

## Limitations

- StatefulSets can't be scaled
- Plot/-ting drives are `hostPath`-only
- Services are `ClusterIP`-only [= Ingress required for Web UI]

## Configuration

See: [values.yaml](values.yaml)

## Contributing

This chart has been created for my usecase. So feel free to open issues or PRs. Any kind of contribution is welcome!

## Get Help

If you need help setting up Machinaris or this chart, feel free to join the Machinaris Discord.
