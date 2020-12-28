# helm-metallb
This helm chart is used to setup my local dev environment.

Starting out as layer2 - working toward bgp.

Manually create the namespace (this is required until argo is in place)
```bash
$ kubectl create ns metallb-system
```