# Step Name -> Adiciona Tratamento Gentil com base no estado-cidade.
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
      "*": "userinfo.&",
      "@UF": "userinfo.UF",
      "UF": {
        "SP": {
          "@(2,cidade)": {
            "São Paulo": {
              "#Paulista": "userinfo.gentile"
            },
            "*": {
              "#Paulistano": "userinfo.gentile"
            }
          }
        },
        "RJ": {
          "@(2,cidade)": {
            "Rio de Janeiro": {
              "#Carioca": "userinfo.gentile"
            },
            "*": {
              "#Fluminense": "userinfo.gentile"
            }
          }
        },
        "AC": {
          "#Acriano": "userinfo.gentile"
        },
        "AL": {
          "#Alagoano": "userinfo.gentile"
        },
        "AP": {
          "#Amapaense": "userinfo.gentile"
        },
        "AM": {
          "#Amazonense": "userinfo.gentile"
        },
        "BA": {
          "#Baiano": "userinfo.gentile"
        },
        "CE": {
          "#Cearense": "userinfo.gentile"
        },
        "DF": {
          "#Basiliense": "userinfo.gentile"
        },
        "ES": {
          "#Capixaba": "userinfo.gentile"
        },
        "GO": {
          "#Goiano": "userinfo.gentile"
        },
        "MA": {
          "#Maranhense": "userinfo.gentile"
        },
        "MT": {
          "#Mato-Grossense": "userinfo.gentile"
        },
        "MS": {
          "#Sul-Mato-Grossense": "userinfo.gentile"
        },
        "MG": {
          "#Mineiro": "userinfo.gentile"
        },
        "PA": {
          "#Paraense": "userinfo.gentile"
        },
        "PB": {
          "#Paraibano": "userinfo.gentile"
        },
        "PR": {
          "#Paranaense": "userinfo.gentile"
        },
        "PE": {
          "#Pernambucano": "userinfo.gentile"
        },
        "PI": {
          "#Piauiense": "userinfo.gentile"
        },
        "RN": {
          "#Potiguar": "userinfo.gentile"
        },
        "RS": {
          "#Gaucho": "userinfo.gentile"
        },
        "RO": {
          "#Rondoniano": "userinfo.gentile"
        },
        "RR": {
          "#Roraimense": "userinfo.gentile"
        },
        "SC": {
          "#Catarinense": "userinfo.gentile"
        },
        "SE": {
          "#Sergipano": "userinfo.gentile"
        },
        "TO": {
          "#Tocantinense": "userinfo.gentile"
        }
      }
    }
  }
]
```

## RAW Object

```
{"type":"transformer","stepName":"Adiciona Tratamento Gentil com base no estado-cidade.","transformSpec":[{"operation":"shift","spec":{"*":"userinfo.&","@UF":"userinfo.UF","UF":{"SP":{"@(2,cidade)":{"São Paulo":{"#Paulista":"userinfo.gentile"},"*":{"#Paulistano":"userinfo.gentile"}}},"RJ":{"@(2,cidade)":{"Rio de Janeiro":{"#Carioca":"userinfo.gentile"},"*":{"#Fluminense":"userinfo.gentile"}}},"AC":{"#Acriano":"userinfo.gentile"},"AL":{"#Alagoano":"userinfo.gentile"},"AP":{"#Amapaense":"userinfo.gentile"},"AM":{"#Amazonense":"userinfo.gentile"},"BA":{"#Baiano":"userinfo.gentile"},"CE":{"#Cearense":"userinfo.gentile"},"DF":{"#Basiliense":"userinfo.gentile"},"ES":{"#Capixaba":"userinfo.gentile"},"GO":{"#Goiano":"userinfo.gentile"},"MA":{"#Maranhense":"userinfo.gentile"},"MT":{"#Mato-Grossense":"userinfo.gentile"},"MS":{"#Sul-Mato-Grossense":"userinfo.gentile"},"MG":{"#Mineiro":"userinfo.gentile"},"PA":{"#Paraense":"userinfo.gentile"},"PB":{"#Paraibano":"userinfo.gentile"},"PR":{"#Paranaense":"userinfo.gentile"},"PE":{"#Pernambucano":"userinfo.gentile"},"PI":{"#Piauiense":"userinfo.gentile"},"RN":{"#Potiguar":"userinfo.gentile"},"RS":{"#Gaucho":"userinfo.gentile"},"RO":{"#Rondoniano":"userinfo.gentile"},"RR":{"#Roraimense":"userinfo.gentile"},"SC":{"#Catarinense":"userinfo.gentile"},"SE":{"#Sergipano":"userinfo.gentile"},"TO":{"#Tocantinense":"userinfo.gentile"}}}}],"onProcessTrack":null,"onExceptionTrack":null,"id":"b5f94f87-0363-48fc-9103-242b8ef42c48"}
```