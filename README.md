## Desafio DDD - Utilizando Domain Events

**Descrição:** 

1. O primeiro evento deverá acontecer quando um novo Customer é criado. Nesse ponto, crie 2 handlers exibindo um "console.log". 

Handler1: EnviaConsoleLog1Handler. Mensagem: "Esse é o primeiro console.log do evento: CustomerCreated".
Handler2: EnviaConsoleLog2Handler. Mensagem: "Esse é o segundo console.log do evento: CustomerCreated". 

2. O segundo evento deverá ser disparado quando o endereço do Customer é trocado (método changeAddress()). Nesse caso, o ID, Nome, bem como os dados do endereço devem ser passados ao evento.

Handler: EnviaConsoleLogHandler. Mensagem: "Endereço do cliente: {id}, {nome} alterado para: {endereco}".
Todos os testes devem ser realizados para garantir o bom funcionamento dos eventos.


## Implementação do Desafio 

#### Para a parte 1 foi criado as classes

* envia-console-log1.handler.ts
* envia-console-log2.handler.ts
* customer-created.event.ts

#### Para a parte 2 foi criado as classes

* envia-console-log.handler.ts
* customer-address-changed.ts

#### Para a implementação dos testes foi criado a classe

* customer-event.spec.ts

#### Descrição dos testes implementados

1. o registro do evento quando um customer é criado.
2. o desregistro do evento quando um customer está criado.
3. a notificação do evento quando um endereço do customer é alterado.


#### Executando o teste

1. Vá até o diretório do teste
```
cd src/domain/customer/event
```

2. Em seguida, execute o seguinte comando:

```
npm test customer-event.spec.ts
```
