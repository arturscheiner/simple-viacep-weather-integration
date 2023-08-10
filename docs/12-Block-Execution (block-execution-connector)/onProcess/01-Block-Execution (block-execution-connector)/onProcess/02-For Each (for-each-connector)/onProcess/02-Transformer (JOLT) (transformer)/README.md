# Step Name -> Transformer (JOLT)
## Component Denominator -> transformer

## Component Description

Transformer (JOLT) allows the manipulation of a JSON through JOLT technology.

Check this component official documentation: [transformer](https://docs.digibee.com/documentation/components/tools/transformer-jolt "Digibee transformer documentation")

## Component Configuration Details
### Documentation

O parâmetro referente à documentação descritiva do componente não foi preenchido ou está indisponível para este componente.

### Parameters

* Type Properties
Area to include the JOLT transformations.

```
[
  {
    "operation": "shift",
    "spec": {
      "body": {
        "*": "body.&"
      },
      "*": "&"
    }
  }
]
```

## RAW Object

```
{"type":"transformer","stepName":"Transformer (JOLT)","transformSpec":[{"operation":"shift","spec":{"body":{"*":"body.&"},"*":"&"}}],"id":"5f2756bf-25da-4f94-ba6b-af72bb888403"}
```