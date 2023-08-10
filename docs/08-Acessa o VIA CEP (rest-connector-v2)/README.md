# Step Name -> Acessa o VIA CEP
## Component Denominator -> generic

## Component Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Documentation

O parâmetro referente à documentação descritiva do componente não foi preenchido ou está indisponível para este componente.

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
715cbb49-3a3e-4abf-90ee-2a98ff285b2b
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
{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"","url":"https://viacep.com.br/ws/{{ DEFAULT(message.userinfo.cep, \"00000-000\") }}/json/","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true}
```

* stepName
```
Acessa o VIA CEP
```

* type
```
connector
```


## RAW Object

```
{"params":{"advanced":false,"disableConnectionPool":false,"compressBody":false,"stopOnServerError":false,"maxRetry":0,"sendBinaryFile":false,"isInsecure":false,"headers":"{\"Content-Type\":\"application/json\"}","operation":"GET","fileName":"","retry":false,"responseCharset":"UTF-8","rawMode":false,"readTimeout":30000,"invalidateSSLSessionsOnEveryCall":false,"rawModeAsBase64":false,"queryParams":"","url":"https://viacep.com.br/ws/{{ DEFAULT(message.userinfo.cep, \"00000-000\") }}/json/","connectTimeout":30000,"saveAsLocalFile":false,"stopOnClientError":false,"forceHttp1":false,"overrideResponseCharset":true},"accountLabel":"","name":"rest-connector-v2","accountLabels":{"custom-1":"","custom-2":""},"stepName":"Acessa o VIA CEP","type":"connector","onExceptionTrack":null,"onProcessTrack":null,"id":"715cbb49-3a3e-4abf-90ee-2a98ff285b2b"}
```