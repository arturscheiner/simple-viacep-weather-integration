# Step Name -> JSON Generator
## Connector Denominator -> json-generator-connector

## Description

JSON Generator (Mock) creates a JSON object. This component accepts any input.

Check this component official documentation: [json-generator-connector](https://docs.digibee.com/documentation/components/tools/json-generator "Digibee json-generator-connector documentation")

## Component Configuration Details
### Parameters

* JSON
The json to generate. Double braces expressions are allowed.

```
{}
```

* FailOnError
If true will stop pipeline with an error, if false will let the pipeline continue but the output will show a property success with value false.

```
false
```

## RAW Object

```
{"name":"json-generator-connector","type":"connector","stepName":"JSON Generator","params":{"json":"{}","failOnError":false},"id":"f418aa9f-e4b1-4ac4-b13d-7b083546f0b6"}
```