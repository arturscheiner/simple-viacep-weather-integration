## This is the pipeline simple-viacep-weather-integration README:
## This is the pipeline components tree:
```bash
├── 00-Mocked Payload Data (json-generator-connector)
├── 01-Git Config (capsule-v1-demo-devops-commit-message-2.0)
├── 02-Bilhetagem (event-publisher-connector)
├── 03-Recebe o CEP e adiciona o timestamp da requisição (json-generator-connector)
├── 04-Block-Execution (block-execution-connector)
│   ├── onException
│   │   ├── 00-Throw Error (throw-error-connector)
│   │   ├── 01-JSON Path Transformer (json-path-transformer)
│   │   ├── 02-Throw Error (throw-error-connector)
│   │   └── 03-Log (log-connector)
│   └── onProcess
│       └── 00-Log (log-connector)
└── 05-Adiciona o "greetings" com base na hora de entrada. (script-connector)

```
