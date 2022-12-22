# Helm Chart Starter

This repository contains starter templates for [Helm](https://helm.sh).

## Usage with [helm-starter](https://github.com/salesforce/helm-starter)

```bash
helm starter fetch https://github.com/christianknell/helm-starter.git
```

To use a starter, run:

```bash
helm create <CHART_NAME> --starter helm-starter/<STARTER_NAME>
```

For example to use the default starter template, run:
```bash
helm create <CHART_NAME> --starter helm-starter/default
```

## Update with [helm-starter](https://github.com/salesforce/helm-starter)

```bash
helm starter update helm-starter
```
