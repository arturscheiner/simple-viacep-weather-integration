estou aqui
# Step Name -> OpenWeather
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
2d5ec0a1-7b47-4e3a-b1ef-ed543cd8aec5
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
{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"{\"lat\":\"{{ message.userinfo.lat }}\",\"lon\":\"{{ message.userinfo.lon }}\",\"appid\":\"b6bf0adc4a6610fdf952ef22a1507b9b\",\"units\":\"metric\"}","url":"https://api.openweathermap.org/data/2.5/forecast","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true}
```

* stepName
```
OpenWeather
```

* type
```
connector
```


## RAW Object

```
{"params":{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"{\"lat\":\"{{ message.userinfo.lat }}\",\"lon\":\"{{ message.userinfo.lon }}\",\"appid\":\"b6bf0adc4a6610fdf952ef22a1507b9b\",\"units\":\"metric\"}","url":"https://api.openweathermap.org/data/2.5/forecast","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true},"accountLabel":"","name":"rest-connector-v2","accountLabels":{"custom-1":"","custom-2":""},"stepName":"OpenWeather","type":"connector","onExceptionTrack":null,"onProcessTrack":null,"id":"2d5ec0a1-7b47-4e3a-b1ef-ed543cd8aec5"}
```