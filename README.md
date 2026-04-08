# Kubernetes Cloud Provider for KIND

* cloud-provider-kind
  * 's goal
    * enable you to,
      * test Kind Kubernetes features / -- depend on a -- cloud-provider
  * ⭐️NATIVELY support⭐️
    * Kubernetes Ingress
    * [Gateway API](https://gateway-api.sigs.k8s.io/)
  * run -- as -- standalone binary | your host
  * allows
    * 👀| your Kind clusters, 
      * provision NEW load balancer containers -- for -- your services👀
  * how does it work?
    * monitor ALL your KIND clusters & Services / Type = LoadBalancer
    * create the corresponding LoadBalancer containers / expose those Services

    ```sh
    bin/cloud-provider-kind
    I0416 19:58:18.391222 2526219 controller.go:98] Creating new cloud provider for cluster kind
    I0416 19:58:18.398569 2526219 controller.go:105] Starting service controller for cluster kind
    I0416 19:58:18.399421 2526219 controller.go:227] Starting service controller
    I0416 19:58:18.399582 2526219 shared_informer.go:273] Waiting for caches to sync for service
    I0416 19:58:18.500460 2526219 shared_informer.go:280] Caches are synced for service
    ...
    ```

* KIND
  * use cases
    * test Kubernetes 
  * characteristics
    * versatile
    * efficient
    * cheap
  * ⚠️limitations⚠️
    * ❌NOT enable you to test features / depend on cloud-providers❌
      * _Example:_ Load Balancers

## Talks

* [Keep Calm and Load Balance on KIND](https://www.youtube.com/watch?v=U6_-y24rJnI)
  * TODO:

## documentation

* [here](/docs/README.md)
