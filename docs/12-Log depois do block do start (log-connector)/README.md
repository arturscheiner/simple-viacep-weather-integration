# Step Name -> Log depois do block do start
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
Error processing message {{ message.$.myField }}
```


## RAW Object

```
{"type":"connector","name":"log-connector","stepName":"Log depois do block do start","params":{"logLevel":"ERROR","message":"Error processing message {{ message.$.myField }}"},"id":"ddd8119e-070b-47f8-b438-be2f70182b17","__documentation__":""}
```