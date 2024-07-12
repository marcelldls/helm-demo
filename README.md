# Helm-demo

To render `demo-chart`:
```
helm template demo-chart
```

To render `demo-parent-chart`:
```
helm dependency build demo-parent-chart
helm template demo-parent-chart
```

To see fetched dependancies:
```
mkdir -p extract && tar xf demo-parent-chart/charts/demo-chart-1.0.0.tgz -C extract
```