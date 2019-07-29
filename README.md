# Pontte Coding Challenge

## 1. Descrição

Seu desafio é criar uma aplicação REST para geração, edição e listagem de contratos de emprëstimos. Uma aplicação simples e rápida de ser desenvolvida. Temos alguns requisitos descritos neste documento para ser seguidos.
O desenvolvimento deve ser feito em Node.js ou Python, e o banco de dados fica de sua escolha. O uso de bliblioteca que ajude no desenvolvimento fica livre, mas use com parcimonia, queremos validar o seu código e não o seu conhecimento com biblioteca.

Vamos usar esse teste para validar a sua lógica, design da sua solução, código legivel, estruturação do código, entre outros fatores.



## 2. Requisitos
- Para cada contrato existe 3 estados (Criação, Upload de Imagens e Aprovação)
- O contrato sempre irá inciar no estado de *Criação*.
- O contrato deve seguir o fluxo de estado de uma forma linear, nunca podendo estar mais de 1 estado ao mesmo tempo. (Conforme descrito no *tópico 3*)
- Somente quando o usuário enviar todos os dados **obrigatórios** ao estado que se encontra, ele pode navegar para o próximo estado. (Dados descrito no *tópico 4*)
- Não pode ser salvo dados de estatos futuros.
- Pode ser atualizados os dados do estado que o contrato se encontra e dos estados anteriores.
- Caso o contrato seja Aprovado ou Repovado, o usuário não pode mais realizar a edição.



## 3. Fluxo dos Estados
```
----------------          ------------------------          ----------------
|    Criacão    |    ->   |   Upload de Imagens   |    ->   |   Aprovação  |
----------------          ------------------------          ----------------
```



## 4. Dados de cada Estados

**Criação**
 - Nome (obrigatório)
 - Email (obrigatório)
 - CPF (obrigatório)
 - Valor do empréstimo (obrigatório)
 - Renda mensal
 - Data de nascimento
 - Estado civil
 - Endereço

**Upload de Imagens**
 - CNH ou CPF (obrigatório)
 - Comprovante de renda
 - Imagens do imóvel

**Aprovação**
 - Status (Aprovação ou reprovação do contrato)


## 5. Diferencial
- Desenvolver a aplicação sobre a arquitetura Serverless.
- Documentação de todo código e dos endpoints.
- Testes unitários e ou de integração.


Qualquer duvida pode entrar em contato via email.

*Não precisa desenvolver uma interface gráfica*
