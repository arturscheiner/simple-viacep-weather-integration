# Step Name -> Busca Longitude e Latitude
## Connector Denominator -> generic

## Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Parameters

* accountLabel
```

```

* accountLabels
```
{"custom-1":"","custom-2":""}
```

* id
```
2492187d-855f-46fa-b656-3c8ff7eae0eb
```

* name
```
rest-connector-v2
```

* onExceptionTrack
```
null
```

* onProcessTrack
```
null
```

* params
```
{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"{\"q\":\"\\\"{{ message.userinfo.cidade }}\\\",\\\"{{ message.userinfo.UF }}\\\",BR\",\"appid\":\"b6bf0adc4a6610fdf952ef22a1507b9b\"}","url":"http://api.openweathermap.org/geo/1.0/direct","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true}
```

* stepName
```
Busca Longitude e Latitude
```

* type
```
connector
```


## RAW Object

```
{"params":{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"{\"q\":\"\\\"{{ message.userinfo.cidade }}\\\",\\\"{{ message.userinfo.UF }}\\\",BR\",\"appid\":\"b6bf0adc4a6610fdf952ef22a1507b9b\"}","url":"http://api.openweathermap.org/geo/1.0/direct","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true},"accountLabel":"","name":"rest-connector-v2","accountLabels":{"custom-1":"","custom-2":""},"stepName":"Busca Longitude e Latitude","type":"connector","onExceptionTrack":null,"onProcessTrack":null,"id":"2492187d-855f-46fa-b656-3c8ff7eae0eb"}
```