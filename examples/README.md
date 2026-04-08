# requirements

* `kind create cluster`
* [install Cloud Provider KIND](https://kubernetes-sigs.github.io/cloud-provider-kind/#/?id=main)
* `sudo cloud-provider-kind`
  * == run cloud-provider-kind
  * AUTOMATICALLY enables LoadBalancer support -- for -- Ingress

# cloud-provider-kind
## TODO:
## how does it work?
### create the corresponding LoadBalancer containers / expose those Services
* `docker ps | grep "envoy"`
  * LoadBalancer container-related
