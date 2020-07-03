## Copying and configure pull secrets to a created namespace

This example shows how to organize copying secrets to new namespaces after it's creation.

The source secrets labeled `pull-secret: yes` are copied from the namespace defined as `MAIN_NAMESPACE` in the controller deployment to other namespaces in the Kubernetes cluster in the following cases:

* after a secret with the label `pull-secret: yes` is created or changed in the namespace defined as `MAIN_NAMESPACE` in the controller deployment
* after a new namespace is created


Image does exist in:

```
quay.io/jorgemoralespou/image-puller-secret-operator:latest
```