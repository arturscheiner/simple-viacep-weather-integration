# Step Name -> Log de Erro na Busca cep
## Connector Denominator -> log-connector

## Description

Log allows the creation of log registers inside a pipeline. It helps in the generation of steps traceability when you want so.

Check this component official documentation: [log-connector](https://docs.digibee.com/documentation/components/tools/log "Digibee log-connector documentation")

## Component Configuration Details
### Parameters

* logLevel
```
ERROR
```

* message
```
CEP Não Encontrado: {{ message.body.cep }}
```


## RAW Object

```
{"type":"connector","name":"log-connector","stepName":"Log de Erro na Busca cep","params":{"logLevel":"ERROR","message":"CEP Não Encontrado: {{ message.body.cep }}"},"onProcessTrack":null,"onExceptionTrack":null,"id":"5d6101e2-7116-4502-b705-b11f7c46f7ca"}
```