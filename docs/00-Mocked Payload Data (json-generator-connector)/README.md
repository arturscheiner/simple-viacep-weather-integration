# Step Name -> Mocked Payload Data
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
 "data": {{ NOW() }},
 "queryAndPath":{
 "cep": "12230-087"
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
{"name":"json-generator-connector","type":"connector","stepName":"Mocked Payload Data","params":{"json":"{\n \"data\": {{ NOW() }},\n \"queryAndPath\":{\n \"cep\": \"12230-087\"\n }\n}","failOnError":false},"id":"3848aec7-f639-4036-a735-0de702ce8e05","__documentation__":""}
```