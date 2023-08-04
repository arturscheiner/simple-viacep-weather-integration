## This is the pipeline simple-viacep-weather-integration README:
## This is the pipeline components tree:
```bash
├── 00-Mocked Payload Data (json-generator-connector)
├── 01-Git Config (capsule-v1-demo-devops-commit-message-2.0)
├── 02-Bilhetagem (event-publisher-connector)
├── 03-Recebe o CEP e adiciona o timestamp da requisição (json-generator-connector)
├── 04-Adiciona o "greetings" com base na hora de entrada. (script-connector)
├── 05-Transforma o body em userinfo. (transformer)
├── 06-Grava o userinfo na sessão. (session-management)
├── 07-Acessa o VIA CEP (rest-connector-v2)
├── 08-Recupera o userinfo da sessao (session-management)
├── 09-Log (log-connector)
├── 10-Log (log-connector)
├── 11-Block-Execution (block-execution-connector)
│   ├── onProcess
│   │   └── 00-Log (log-connector)
│   └── onException
│       ├── 00-Throw Error (throw-error-connector)
│       ├── 01-JSON Path Transformer (json-path-transformer)
│       ├── 02-Throw Error (throw-error-connector)
│       └── 03-Log (log-connector)
└── 12-Log depois do block (log-connector)

```
