Basic example of using CAMEL REST DSL with an OpenAPI Schema for a contract-first API approach

To execute:

```

jbang '-Dcamel.jbang.version=4.5.0' camel@apache/camel run restopenapi-endpoints.camel.yaml --dev --logging-level=info --open-api=open-api.v1.schema.yaml

```


When the backend (DB) is available, you should see something like that:

    ![results](/images/sshot.png)

