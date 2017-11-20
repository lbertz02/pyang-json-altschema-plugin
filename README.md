# pyang-json-altschema-plugin

This is a pyang JSON Schema output plugin. It takes YANG files and tries to produce a JSON Schema that validates JSON content similar to the payload as defined in [RFC7951](https://tools.ietf.org/html/rfc7951).

Here's an example when running from the `test` directory:
```
$ pyang --plugindir ../ -f json-altschema ./test-module.yang > test-module.jsonschema
```

It is a derivatin of the [json-schema plugin](https://github.com/cmoberg/pyang-json-schema-plugin).  It is ultimately intended to produce less schema thatn the original plugin AND also map the schema to a form that can be used in [Swagger](https://swagger.io/).  

