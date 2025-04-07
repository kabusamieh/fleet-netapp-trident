# Fleet Helm Deployment

This example will deploy the [NetApp Trident Operator](https://www.netapp.com/cloud-services/trident/)
packaged as a Helm chart.
The app will be deployed into the `netapp-trident` namespace.


```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: helm
  namespace: fleet-default
spec:
  repo: https://github.com/kabusamieh/fleet-netapp-trident
  paths:
  - helm
```