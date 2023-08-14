# Step Name -> JSON Path Transformer
## Connector Denominator -> generic

## Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Parameters

* failOnError
```
false
```

* id
```
548788f6-5f2f-4204-b06e-420bcb5fdc0f
```

* jsonPath
```
$.store.books[?(@.title=='IT')]
```

* stepName
```
JSON Path Transformer
```

* type
```
json-path-transformer
```


## RAW Object

```
{"type":"json-path-transformer","stepName":"JSON Path Transformer","jsonPath":"$.store.books[?(@.title=='IT')]","failOnError":false,"id":"548788f6-5f2f-4204-b06e-420bcb5fdc0f"}
```