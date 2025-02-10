Basic example of using CAMEL REST DSL with an OpenAPI Schema for a contract-first API approach

The path, URL and specification is abstrated and separated from the implementation

the path is in te OpenAPI document: [path](https://github.com/masauve/camel-account-pipeline/blob/290ffa217c73426bf8de5089ce6f3a0853ea5360/openapi/open-api.v1.schema.yaml#L10)

the implementation is link to the specification by operationId:

Specification: [operationId](https://github.com/masauve/camel-account-pipeline/blob/290ffa217c73426bf8de5089ce6f3a0853ea5360/openapi/open-api.v1.schema.yaml#L20)


To execute:

```

jbang '-Dcamel.jbang.version=4.5.0' camel@apache/camel run restopenapi-endpoints.camel.yaml --dev --logging-level=info --open-api=open-api.v1.schema.yaml

```


When the backend (DB) is available, you should see something like that:

![results](/images/sshot.png)

