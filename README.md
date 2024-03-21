# Deploy Librespeed in Kubernetes

![Librespeed](/images/overview.png)

## Build commands

To deploy `librespeed` in kubernetes go to the folder from the cloned repo that has all of the `yaml` manifest files.

Run this command from that directory

``` shell
kubectl create -k .
```

![Create-CLI](/images/create.png)

Once completed you can check the status of everything with this command

``` shell
kubectl get pod,deployment,pvc,svc -n librespeed
```

![Status-CLI](/images/status.png)

## Deleting deployment of Librespeed

To remove run this command

``` shell
kubectl delete namespace librespeed
```
