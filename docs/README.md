```
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
│   │   ├── 00-Log (log-connector)
│   │   ├── 01-Block-Execution (block-execution-connector)
│   │   │   ├── onProcess
│   │   │   │   ├── 00-Blob Storage (Azure) (Azure-Blob-Storage-Connector)
│   │   │   │   ├── 01-Log (log-connector)
│   │   │   │   └── 02-For Each (for-each-connector)
│   │   │   │       ├── onProcess
│   │   │   │       │   ├── 00-Template Transformer (template-transformer)
│   │   │   │       │   ├── 01-JSON Transformer (json-transformer-connector)
│   │   │   │       │   └── 02-Transformer (JOLT) (transformer)
│   │   │   │       └── onException
│   │   │   │           └── 00-JSON String to JSON Transformer (json-string-to-json-transformer)
│   │   │   └── onException
│   │   │       └── 00-Log (log-connector)
│   │   └── 02-Log depois do block dentro do block (log-connector)
│   └── onException
│       ├── 00-Throw Error (throw-error-connector)
│       ├── 01-JSON Path Transformer (json-path-transformer)
│       ├── 02-Throw Error (throw-error-connector)
│       └── 03-Log (log-connector)
├── 12-Log depois do block do start (log-connector)
├── 13-JSON Transformer (json-transformer-connector)
└── 14-Choice (choice)
    ├── when-CEP Não Encontrado #Py2q38#
    │   ├── 00-Log de Erro na Busca cep (log-connector)
    │   ├── 01-Throw Error (throw-error-connector)
    │   └── 02-Log (log-connector)
    ├── when-condition-1
    │   ├── 00-Log (log-connector)
    │   ├── 01-WGet (Download HTTP) (wget-connector)
    │   ├── 02-Blob Storage (Azure) (Azure-Blob-Storage-Connector)
    │   └── 03-Log (log-connector)
    ├── when-condition-2
    │   ├── 00-Log (log-connector)
    │   ├── 01-SAP (IDoc and RFC) (sap-connector)
    │   ├── 02-Dropbox (dropbox-connector)
    │   └── 03-Google Drive (google-drive-connector)
    └── otherwise-CEP Encontrado com Sucesso #0UTtmO#
        ├── 00-Log de Sucesso na Busca CEP (log-connector)
        ├── 01-Tratamento de Dados (json-generator-connector)
        ├── 02-Adiciona Tratamento Gentil com base no estado-cidade. (transformer)
        ├── 03-Salva informações do usuário em Sessão (session-management)
        ├── 04-Busca Longitude e Latitude (rest-connector-v2)
        ├── 05-Carrega informações do usuário (session-management)
        └── 06-Choice (choice)
            ├── when-Longitude Não Encontrado #eKXbiV#
            │   └── 00-Log de Erro na Busca cep (log-connector)
            └── otherwise-Longitude Encontrado com Sucesso #vwTalh#
                ├── 00-Log de Sucesso na Busca CEP (log-connector)
                ├── 01-Adiciona mais algumas informações no userinfo (json-generator-connector)
                ├── 02-Salvar Informações do Usuário em Sessão (session-management)
                ├── 03-OpenWeather (rest-connector-v2)
                ├── 04-Carrega Informações do Usuário da Sessão (session-management)
                └── 05-Transforma o Retorno do Forecast (transformer)

```
