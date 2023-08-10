# Step Name -> Template Transformer
## Component Denominator -> template-transformer

## Component Description

Template Transformer generates XML, HTML, text and other data from a specified template. The component can receive data to dynamically fill the template from a JSON received in its input message.

Check this component official documentation: [template-transformer](https://docs.digibee.com/documentation/components/tools/template-transformer "Digibee template-transformer documentation")

## Component Configuration Details
### Documentation

O parâmetro referente à documentação descritiva do componente não foi preenchido ou está indisponível para este componente.

### Parameters

* Model Path - A dotted notation representation of the fields that should be used as source model and then transformed by the template.

```
body
```

* Body - The template (string value) to be replaced during runtime with data from the model

```
<soap:Envelope xmlns:soap="http://www.w3.org/2003/05/soap-envelope" xmlns:web="http://www.webservicex.net/">
   <soap:Header/>
   <soap:Body>
      <web:GetNAICSByID>
         <!--Optional:-->
         <web:NAICSCode>${naic.code}</web:NAICSCode>
      </web:GetNAICSByID>
   </soap:Body>
</soap:Envelope>
```

* Preserve Original
When enabled, original fields will be preserved. Original fields are preserved on a new field prefixed by _ (underline)

```
true
```

## RAW Object

```
{"type":"template-transformer","stepName":"Template Transformer","modelPath":"body","template":"<soap:Envelope xmlns:soap=\"http://www.w3.org/2003/05/soap-envelope\" xmlns:web=\"http://www.webservicex.net/\">\r\n   <soap:Header/>\r\n   <soap:Body>\r\n      <web:GetNAICSByID>\r\n         <!--Optional:-->\r\n         <web:NAICSCode>${naic.code}</web:NAICSCode>\r\n      </web:GetNAICSByID>\r\n   </soap:Body>\r\n</soap:Envelope>","preserveOriginal":true,"id":"65a6e3fc-74fc-4c4d-b2e0-381f2620415f"}
```