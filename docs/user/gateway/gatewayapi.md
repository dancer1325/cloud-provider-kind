# Gateway API support

* ==
    * implements the `Gateway` and `HTTPRoute` functionalities
    * passes the community conformance tests

* Gateway API controller
    * by default,
        * enabled
    * if you want to configure it -> specify `--gateway-channel` CL's flag /
        * ALLOWED values
            * standard
                * default one
            * experimental
            * disabled

      ```sh
      cloud-provider-kind --gateway-channel standard|experimental|disabled
      ```