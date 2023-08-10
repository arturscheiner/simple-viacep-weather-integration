# Step Name -> Append Files
## Connector Denominator -> generic

## Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Parameters

* id
```
16ae572b-d552-4ff7-bf94-2e4ed7bcae35
```

* name
```
append-files-connector
```

* params
```
{"fileName":"{{ message.fileName }}","charset":"UTF-8","rawAppendFiles":"{{ message.files }}","filesRawMode":false,"failOnError":false}
```

* stepName
```
Append Files
```

* type
```
connector
```


## RAW Object

```
{"type":"connector","name":"append-files-connector","stepName":"Append Files","params":{"fileName":"{{ message.fileName }}","charset":"UTF-8","rawAppendFiles":"{{ message.files }}","filesRawMode":false,"failOnError":false},"id":"16ae572b-d552-4ff7-bf94-2e4ed7bcae35"}
```