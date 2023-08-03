# Step Name -> Choice
## Connector Denominator -> generic

## Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Parameters

* id
```
b339b4cb-478c-4776-af44-f5b58c3078d0
```

* onExceptionTrack
```
null
```

* onProcessTrack
```
null
```

* otherwise
```
CEP Encontrado com Sucesso #0UTtmO#
```

* stepName
```
Choice
```

* type
```
choice
```

* when
```
[{"target":"CEP Não Encontrado #Py2q38#","jsonPath":"$.[?(@.body.erro == \"true\")]"},{"target":"condition-1","jsonPath":"$"}]
```


## RAW Object

```
{"type":"choice","stepName":"Choice","onProcessTrack":null,"onExceptionTrack":null,"id":"b339b4cb-478c-4776-af44-f5b58c3078d0","when":[{"target":"CEP Não Encontrado #Py2q38#","jsonPath":"$.[?(@.body.erro == \"true\")]"},{"target":"condition-1","jsonPath":"$"}],"otherwise":"CEP Encontrado com Sucesso #0UTtmO#"}
```