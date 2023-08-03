# Step Name -> Adiciona mais algumas informações no userinfo
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
 "userinfo" : {
 "lat": {{ message.body[0].lat }},
 "lon": {{ message.body[0].lon }},
 "country": {{ message.body[0].country }},
 "stateName": {{ message.body[0].state }},
 "state": {{ message.userinfo.UF }},
 "gentile": {{ message.userinfo.gentile }},
 "city": {{ message.userinfo.cidade }},
 "zipCode": {{ message.userinfo.cep }},
 "greetings": {{ message.userinfo.greetings }},
 "requestTimestamp": {{ message.userinfo.requestTimestamp }}
 }
}
```

* FailOnError
If true will stop pipeline with an error, if false will let the pipeline continue but the output will show a property success with value false.

```
false
```

## RAW Object

```
{"name":"json-generator-connector","type":"connector","stepName":"Adiciona mais algumas informações no userinfo","params":{"json":"{\n \"userinfo\" : {\n \"lat\": {{ message.body[0].lat }},\n \"lon\": {{ message.body[0].lon }},\n \"country\": {{ message.body[0].country }},\n \"stateName\": {{ message.body[0].state }},\n \"state\": {{ message.userinfo.UF }},\n \"gentile\": {{ message.userinfo.gentile }},\n \"city\": {{ message.userinfo.cidade }},\n \"zipCode\": {{ message.userinfo.cep }},\n \"greetings\": {{ message.userinfo.greetings }},\n \"requestTimestamp\": {{ message.userinfo.requestTimestamp }}\n }\n}","failOnError":false},"onProcessTrack":null,"onExceptionTrack":null,"id":"d81c6b3c-4572-415f-b81e-b62145c3f8e3"}
```