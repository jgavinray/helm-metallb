# helm-metallb
This helm chart is used to setup my local dev environment.

Starting out as layer2 - working toward bgp.

Manually create the namespace (this is required until argo is in place)
```bash
$ kubectl create ns metallb-system
```

This repository is working as is. 
The biggest issue with getting this to work has been my own lack of understanding of networking.
At the time of this writing the Unifi Dream Machine PRO that I am using on my local network is unable to make a network smaller than a /24 CIDR (255 IP addresses). 
My original goal was to use two /25s ranges so that two networks within a range could exist but that was not possible.