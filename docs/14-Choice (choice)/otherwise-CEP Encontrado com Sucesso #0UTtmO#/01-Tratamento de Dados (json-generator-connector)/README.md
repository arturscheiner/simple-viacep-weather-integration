# Step Name -> Tratamento de Dados
## Connector Denominator -> json-generator-connector

## Description

JSON Generator (Mock) creates a JSON object. This component accepts any input.

Check this component official documentation: [json-generator-connector](https://docs.digibee.com/documentation/components/tools/json-generator "Digibee json-generator-connector documentation")

## Component Configuration Details
### Parameters

* JSON
The json to generate. Double braces expressions are allowed.

```
{
 "UF": {{ message.body.uf }},
 "cidade": {{ message.body.localidade }},
 "cep": {{ message.body.cep }},
 "requestTimestamp": {{ message.userinfo.requestTimestamp }},
 "greetings": {{ message.userinfo.greetings }}
}
```

* FailOnError
If true will stop pipeline with an error, if false will let the pipeline continue but the output will show a property success with value false.

```
false
```

## RAW Object

```
{"name":"json-generator-connector","type":"connector","stepName":"Tratamento de Dados","params":{"json":"{\n \"UF\": {{ message.body.uf }},\n \"cidade\": {{ message.body.localidade }},\n \"cep\": {{ message.body.cep }},\n \"requestTimestamp\": {{ message.userinfo.requestTimestamp }},\n \"greetings\": {{ message.userinfo.greetings }}\n}","failOnError":false},"onProcessTrack":null,"onExceptionTrack":null,"id":"8f5baa09-87be-4188-8ced-fd1164647516"}
```