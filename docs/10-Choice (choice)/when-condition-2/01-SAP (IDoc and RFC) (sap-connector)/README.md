# Step Name -> SAP (IDoc and RFC)
## Connector Denominator -> generic

## Description

Digibee components are a powerful way to simplify the process of building integration flows. By using pre-built connectors and logic components, you can quickly and easily create complex integrations that connect different applications and services.

Check Digibee's official documentation: [generic](https://docs.digibee.com/documentation "Digibee documentation")

## Component Configuration Details
### Parameters

* accountLabel
```
mysql
```

* id
```
72e0db74-5009-4176-bf34-de4e6423c4b2
```

* name
```
sap-connector
```

* params
```
{"failOnError":false,"operation":"RFC","asHost":"localhost","lang":"en","client":"400","sysnr":"01","RFC":"YYPCL_RFC_ORDEM_FATURA","sapRequestTemplate":"<?xml version=\"1.0\" encoding=\"ASCII\"?><YYPCL_RFC_ORDEM_FATURA:Request xmlns:YYPCL_RFC_ORDEM_FATURA=\"http://sap.fusesource.org/rfc/QAS/YYPCL_RFC_ORDEM_FATURA\" P_ERDAT_INI=\"2018-07-01T00:00:00.000\" P_ERDAT_FIM=\"2018-08-01T00:00:00.000\" CLIENTE=\"\" VKORG=\"0050\" AUART=\"\" />"}
```

* stepName
```
SAP (IDoc and RFC)
```

* type
```
connector
```


## RAW Object

```
{"type":"connector","accountLabel":"mysql","name":"sap-connector","stepName":"SAP (IDoc and RFC)","params":{"failOnError":false,"operation":"RFC","asHost":"localhost","lang":"en","client":"400","sysnr":"01","RFC":"YYPCL_RFC_ORDEM_FATURA","sapRequestTemplate":"<?xml version=\"1.0\" encoding=\"ASCII\"?><YYPCL_RFC_ORDEM_FATURA:Request xmlns:YYPCL_RFC_ORDEM_FATURA=\"http://sap.fusesource.org/rfc/QAS/YYPCL_RFC_ORDEM_FATURA\" P_ERDAT_INI=\"2018-07-01T00:00:00.000\" P_ERDAT_FIM=\"2018-08-01T00:00:00.000\" CLIENTE=\"\" VKORG=\"0050\" AUART=\"\" />"},"id":"72e0db74-5009-4176-bf34-de4e6423c4b2"}
```