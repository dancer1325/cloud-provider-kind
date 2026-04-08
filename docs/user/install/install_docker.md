# install -- via -- Docker Image

* requirements
    * cloud-provider-kind v0.4.0+

* AVAILABLE | registry.k8s.io/cloud-provider-kind/cloud-controller-manager

* ways to build by your own
    * -- via -- Makefile
        * `make`
        * `sudo mv ./bin/cloud-provider-kind  /usr/local/bin/cloud-provider-kind`
    * run it as a container
        * TODO: require to mount the docker socket inside the container

      ```sh
      docker build . -t cloud-provider-kind
      # using the host network
      docker run --rm --network host -v /var/run/docker.sock:/var/run/docker.sock cloud-provider-kind
      # or the kind network
      docker run --rm --network kind -v /var/run/docker.sock:/var/run/docker.sock cloud-provider-kind
      ```

    * -- via -- [compose.yaml](compose.yml)

      ```sh
      # using the `kind` network (`host` is the default value for NET_MODE)
      NET_MODE=kind docker compose up -d
      ```