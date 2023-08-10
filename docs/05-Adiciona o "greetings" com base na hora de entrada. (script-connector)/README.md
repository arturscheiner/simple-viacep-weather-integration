# Step Name -> Adiciona o "greetings" com base na hora de entrada.
## Component Denominator -> script-connector

## Component Description

Script allows the execution of javascript code extracts (javascript is also known as ECMAScript).

Check this component official documentation: [script-connector](https://docs.digibee.com/documentation/components/tools/script "Digibee script-connector documentation")

## Component Configuration Details
### Documentation

O parâmetro referente à documentação descritiva do componente não foi preenchido ou está indisponível para este componente.

### Parameters

* code
```
var hour = body.requestHour;

if(hour>=6 && hour<12) {
 output = {greetings: "Bom Dia"};
}
else if(hour>+12 && hour<18) {
 output = {greetings: "Boa Tarde"};
}
else {
 output = {greetings: "Boa Noite"};
}

finalResult = Object.assign(body,output)

body
```

* timeout
```
10000
```


## RAW Object

```
{"type":"connector","name":"script-connector","stepName":"Adiciona o \"greetings\" com base na hora de entrada.","params":{"code":"var hour = body.requestHour;\n\nif(hour>=6 && hour<12) {\n output = {greetings: \"Bom Dia\"};\n}\nelse if(hour>+12 && hour<18) {\n output = {greetings: \"Boa Tarde\"};\n}\nelse {\n output = {greetings: \"Boa Noite\"};\n}\n\nfinalResult = Object.assign(body,output)\n\nbody","timeout":10000},"onProcessTrack":null,"onExceptionTrack":null,"id":"ca0553ad-defd-4621-8c29-43ee3a5bfbc7"}
```