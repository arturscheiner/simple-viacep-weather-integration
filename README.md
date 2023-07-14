## This is the pipeline simple-viacep-weather-integration README:
## This is the pipeline components tree:
```bash
├── 00-Mocked Payload Data (json-generator-connector)
├── 01-Git Config (capsule-v1-demo-devops-commit-message-2.0)
├── 02-Bilhetagema (event-publisher-connector)
├── 03-Recebe o CEP e adiciona o timestamp da requisição (json-generator-connector)
├── 04-Adiciona o "greetings" com base na hora de entrada. (script-connector)
├── 05-Transforma o body em userinfo. (transformer)
├── 06-Grava o userinfo na sessão. (session-management)
├── 07-Acessa o VIA CEP (rest-connector-v2)
├── 08-Recupera o userinfo da sessao (session-management)
└── 09-Choice (choice)
    ├── when-CEP Não Encontrado #Py2q38#
    │   └── 00-Log de Erro na Busca cep (log-connector)
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
