# install -- via -- `go install`

* steps
    ```sh
    go install sigs.k8s.io/cloud-provider-kind@latest
    # install the binary | $GOBIN
    #   by default, | ~/go/bin
    
    # if $GOBIN is NOT | PATH & you want to make the binary AVAILABLE | ELSEWHERE -> run it
    #   Reason:🧠/usr/local/bin is included | PATH🧠
    sudo install ~/go/bin/cloud-provider-kind /usr/local/bin
    ```

* recommended one
    * Reason:🧠ONLY OFFICIAL one is supported🧠
