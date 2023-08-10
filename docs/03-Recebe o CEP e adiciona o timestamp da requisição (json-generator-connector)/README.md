# Step Name -> Recebe o CEP e adiciona o timestamp da requisição
## Component Denominator -> json-generator-connector

## Component Description

JSON Generator (Mock) creates a JSON object. This component accepts any input.

Check this component official documentation: [json-generator-connector](https://docs.digibee.com/documentation/components/tools/json-generator "Digibee json-generator-connector documentation")

## Component Configuration Details
### Documentation

O parâmetro referente à documentação descritiva do componente não foi preenchido ou está indisponível para este componente.

### Parameters

* JSON
The json to generate. Double braces expressions are allowed.

```
{
 "userinfo" : {
 "cep" : {{ message.queryAndPath.cep }},
 "requestTimestamp": {{ NOW() }}
 },
 "body": {
 "cep" : {{ message.queryAndPath.cep }},
 "requestTimestamp": {{ NOW() }}, 
 "requestHour": {{ FORMATDATE(NOW(), "timestamp", "HH", null, "GMT-3", "pt-BR", null) }}
 }

}


### Se existe consulta (marca data e hora da consulta) se não existe, cadastra
```

* FailOnError
If true will stop pipeline with an error, if false will let the pipeline continue but the output will show a property success with value false.

```
false
```

## RAW Object

```
{"name":"json-generator-connector","type":"connector","stepName":"Recebe o CEP e adiciona o timestamp da requisição","params":{"json":"{\n \"userinfo\" : {\n \"cep\" : {{ message.queryAndPath.cep }},\n \"requestTimestamp\": {{ NOW() }}\n },\n \"body\": {\n \"cep\" : {{ message.queryAndPath.cep }},\n \"requestTimestamp\": {{ NOW() }}, \n \"requestHour\": {{ FORMATDATE(NOW(), \"timestamp\", \"HH\", null, \"GMT-3\", \"pt-BR\", null) }}\n }\n\n}\n\n\n### Se existe consulta (marca data e hora da consulta) se não existe, cadastra","failOnError":false},"onProcessTrack":null,"onExceptionTrack":null,"id":"9c8c71b1-76d3-4d46-a69b-298d83dcb7d7"}
```