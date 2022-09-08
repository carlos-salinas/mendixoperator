# mendixoperator
This is a Helm chart for Mendix Operator (Mendix for Private Cloud component)

## How to publish the chart into local Helm repository (Github pages)

```
helm package mendixoperator 
mv mendixoperator-x.y.z.tgz /mendixoperator
helm repo index mendixoperator/ https://carlos-salinas.github.io/mendixoperator/
git commit -m "Upload new chart version"
git push origin gh-pages
```