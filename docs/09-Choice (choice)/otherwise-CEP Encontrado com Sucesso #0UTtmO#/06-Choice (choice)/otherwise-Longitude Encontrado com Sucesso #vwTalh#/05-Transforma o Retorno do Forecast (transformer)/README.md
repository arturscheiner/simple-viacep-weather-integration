# Step Name -> Transforma o Retorno do Forecast
## Connector Denominator -> transformer

## Description

Transformer (JOLT) allows the manipulation of a JSON through JOLT technology.

Check this component official documentation: [transformer](https://docs.digibee.com/documentation/components/tools/transformer-jolt "Digibee transformer documentation")

## Component Configuration Details
### Parameters

* Type Properties
Area to include the JOLT transformations.

```
[
  {
    "operation": "shift",
    "spec": {
      "userinfo": {
        "*": "&"
      },
      "body": {
        "list": {
          "*": {
            "dt": "forecast[&1].timestamp",
            "dt_txt": "forecast[&1].date",
            "@(main.temp)": "forecast[&1].temp",
            "@(main.temp_min)": "forecast[&1].minTemperature",
            "@(main.temp_max)": "forecast[&1].maxTemperature",
            "@(weather[0].main)": "forecast[&1].weatherMain",
            "@(weather[0].description)": "forecast[&1].weatherDescription"
          }
        }
      }
    }
  },
  {
    "operation": "modify-default-beta",
    "spec": {
      "forecast": {
        "*": {
          "weatherConditions": "=concat(@(1,weatherMain),' (',@(1,weatherDescription),),)"
        }
      }
    }
  }
]
```

## RAW Object

```
{"type":"transformer","stepName":"Transforma o Retorno do Forecast","transformSpec":[{"operation":"shift","spec":{"userinfo":{"*":"&"},"body":{"list":{"*":{"dt":"forecast[&1].timestamp","dt_txt":"forecast[&1].date","@(main.temp)":"forecast[&1].temp","@(main.temp_min)":"forecast[&1].minTemperature","@(main.temp_max)":"forecast[&1].maxTemperature","@(weather[0].main)":"forecast[&1].weatherMain","@(weather[0].description)":"forecast[&1].weatherDescription"}}}}},{"operation":"modify-default-beta","spec":{"forecast":{"*":{"weatherConditions":"=concat(@(1,weatherMain),' (',@(1,weatherDescription),),)"}}}}],"onProcessTrack":null,"onExceptionTrack":null,"id":"b8a03000-5823-42cd-b14d-ce4d5c1f8084"}
```