


Update Values.Yaml file 
(Optional) - To verify Values file

```helm template . --values values.yaml```


```
helm package .
helm install argocd-auto-connector argo-cd-auto-connector-0.1.0.tgz --values values.yaml --namespace=temp-ns --create-namespace
sleep 150
helm uninstall argocd-auto-connector --namespace=temp-ns
```

