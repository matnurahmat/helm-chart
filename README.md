# helm-chart

> make directori helm-chart-sources

```
mkdir -p ./
helm-chart-sources
```

> create helm chart

```
helm create helm-chart-sources/helm-chart-test 
```

Lint the chart

`helm lint helm-chart-sources/*`

Create the Helm chart package

```
helm package helm-chart-sources/*

```
Create the Helm chart repository index

```
helm repo index --url https://matnurahmat.github.io/helm-chart/ .
```

Configure the “helm-chart” repository as a Github pages site


~~~~

Configure helm client

```
helm repo add myhelmrepo https://mattiaperi.github.io/helm-chart/
```

Update and Test the Helm chart repository

```
helm repo update

helm serch test
```

Add new charts to an existing repository

```
helm repo index --url https://matnurahmat.github.io/helm-chart/ --merge index.yaml .
```