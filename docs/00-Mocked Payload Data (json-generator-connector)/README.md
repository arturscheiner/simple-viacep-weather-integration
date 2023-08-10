# Step Name -> Mocked Payload Data
## Component Denominator -> json-generator-connector

## Component Description

JSON Generator (Mock) creates a JSON object. This component accepts any input.

Check this component official documentation: [json-generator-connector](https://docs.digibee.com/documentation/components/tools/json-generator "Digibee json-generator-connector documentation")

## Component Configuration Details
### Documentation

Aqui criamos um payload mockado, que é utilizado para a execução do fluxo do pipeline.

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
{"name":"json-generator-connector","type":"connector","stepName":"Mocked Payload Data","params":{"json":"{\n \"data\": {{ NOW() }},\n \"queryAndPath\":{\n \"cep\": \"12230-087\"\n }\n}","failOnError":false},"id":"3848aec7-f639-4036-a735-0de702ce8e05","__documentation__":"Aqui criamos um payload mockado, que é utilizado para a execução do fluxo do pipeline."}
```