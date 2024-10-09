# Regras de Mitigação de Risco - Cartão de Crédito

## Cadastro de Usuários
- CPF, Nome e Data de Nascimento (Não é feita nenhuma checagem em bureau)
- Email verificado
- Número de Telefone verificado
- Coleta de Selfie (Liveness)
- Coleta do DeviceId (ID único para o App no dispositivo)

> A compra de créditos só pode ser realizada com o usuário cadastrado e logado.

## Cadastro do cartão de pagamento

Para o uso do cartão de crédito, o mesmo deve ser tokenizado. Nesse processo são seguidas as seguintes etapas:

1) Transação Zero Auth para verificação da validade do cartão sem realização de cobrança.
2) Processo de tokenização realizado com a solicitação do CVV.

## Realização do Pagamento


### No Aplicativo

Para toda transação realizada com cartão de crédito, mesmo com o cartão já tokenizado, o app solicita que o usuário digite o CVV. A última localização do usuário, disponível no momento, também é enviada.


### No Backend

No backend temos 3 níveis de verificação de parâmetros da transação:

- Parâmetros Gerais
- Parâmetros por Conta
- Parâmetros por PAR (Payment Account Reference)

#### Parâmetros Gerais

| Parâmetro  | Observação |
| :-------------------------------------- | -----------------------: |  
| Valor Mínimo por Transação | --- |
| Valor Máximo por Transação com PAR | --- |
| Valor Máximo por Transação sem PAR | Recomendamos um valor baixo para a 1a transação |
| Valor Máximo por Transação Noturna | após às das 20hs |
| Valor Máximo por Transação em Domingos | Domingos e Feriados Cadastrados |


#### Parâmetros por Conta

| Parâmetro  | Observação |
| :-------------------------------------- | -----------------------: |  
| Limite de Compra Diário  | Soma de todas as compras realizadas pela conta
| Limite de Compra Mensal  | Soma de todas as compras realizadas pela conta


#### Parâmetros por PAR

O que é PAR?

O PAR é um identificador exclusivo associado ao titular de uma conta de pagamento (ou seja, ao portador do cartão), **não ao cartão em si**. Isso significa que, independentemente de qual cartão físico ou token virtual esteja sendo usado (seja num celular, relógio ou mesmo numa nova emissão do cartão físico), o PAR permanece o mesmo para aquele titular de conta.

> O PAR é recebido apenas `após a primeira transação do cartão realizada com sucesso`. Desta forma, para a primeira transação do PAN, não temos como aplicar as regras abaixo.

> A verificação por PAR é feita não apenas no escopo da própria conta, mas para um somatório de pagamentos realizados pelo PAR no sistema.

| Parâmetro  | Observação |
| :-------------------------------------- | -----------------------: |  
| Qtde máxima de compras diária | --- |
| Qtde máxima de compras mensal | --- |
| Limite de Compra Mensal | --- |
| Limite de Compra Diário | --- |


#### Lista de Restrição por PAR

Em caso de chargeback, ou alguma transação suspeita, o PAR relacionado à essa transação pode ser colocado em uma lista de restrição. Nenhuma transação de cartão ou token relacionado a esse PAR será permitida.

#### Cielo Velocity

[Velocity](https://suporte.braspag.com.br/hc/pt-br/articles/20957216519579-Como-gerenciar-as-regras-do-Velocity-Check)





