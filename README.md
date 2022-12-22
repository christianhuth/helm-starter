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

## Needed changes after creation

After running the above command to create a chart from a starter template you still have to apply some changes to the created files.

1. `Chart.yaml`:
   1. change `appVersion`
   2. change `description`
   3. change `version`
   4. add `home`
   5. add `icon`
   6. add `maintainers`
   7. add `sources`
2. `values.yaml`:
   1. change `image.repository`
   2. change `image.tag`
3. `README.md.gotmpl`:
   1. replace `<CHARTNAME>` with the real name of the chart
   2. add an `<INTRODUCTION>`
   3. replace `<APPLICATION_NAME>` and `<APPLICATION_LINK>` with the real values

That's basically all you have to do to have a clean starting point.
The provided [./values.yaml](values.yaml) comes already with annotations for usage with [helm-docs](https://github.com/norwoodj/helm-docs).
See [these instructions](https://github.com/christianknell/helm-charts/tree/main/development) on how to create a README.md in an automatic fashion.

## Update with [helm-starter](https://github.com/salesforce/helm-starter)

```bash
helm starter update helm-starter
```
