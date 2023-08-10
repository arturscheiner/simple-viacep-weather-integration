# Step Name -> Transforma o body em userinfo.
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
      "output": {
        "*": "userinfo.&"
      }
    }
  }
]
```

## RAW Object

```
{"type":"transformer","stepName":"Transforma o body em userinfo.","transformSpec":[{"operation":"shift","spec":{"output":{"*":"userinfo.&"}}}],"onProcessTrack":null,"onExceptionTrack":null,"id":"d654e494-5e0b-4c5c-9c5a-db668260b15e"}
```