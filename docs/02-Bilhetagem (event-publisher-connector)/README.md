# Step Name -> Bilhetagem
## Component Denominator -> event-publisher-connector

## Component Description

Event Publisher publishes an event for other configured pipelines to listen to it and have a chance to react when the publishing happens.

Check this component official documentation: [event-publisher-connector](https://docs.digibee.com/documentation/components/queues-and-messaging/event-publisher "Digibee event-publisher-connector documentation")

## Component Configuration Details
### Documentation

Envia o payload para a fila de eventos que realiza a bilhetagem.

### Documentation

Envia o payload para a fila de eventos que realiza a bilhetagem.

### Parameters

* body
```
{{ message.$ }}
```

* eventName
```
{{ DEFAULT(message.eventName, "billing-control") }}
```

* showSendEventLog
```
false
```

* stopOnError
```
false
```


## RAW Object

```
{"type":"connector","stepName":"Bilhetagem","name":"event-publisher-connector","params":{"eventName":"{{ DEFAULT(message.eventName, \"billing-control\") }}","body":"{{ message.$ }}","showSendEventLog":false,"stopOnError":false},"id":"4df87046-4b5e-4b9a-89ef-ec7eb4ee5ea3","__documentation__":"Envia o payload para a fila de eventos que realiza a bilhetagem."}
```