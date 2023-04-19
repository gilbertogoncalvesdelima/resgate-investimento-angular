## Resgate-investimento-angular (Gilberto Gonçalves de Lima Whatsapp: +551196223-5618)

# ResgateInvest

This project was generated with
[Angular CLI](https://github.com/angular/angular-cli) version 15.2.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The
application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can
also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the
`dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via
[Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To
use this command, you need to first add a package that implements end-to-end
testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the
[Angular CLI Overview and Command Reference](https://angular.io/cli) page.

### Criar uma mini aplicação em angular 13+ que simula um resgate personalizado de

fundos de investimentos em ações. Serão avaliados:

• Integração com api rest

• Navegação entre telas

• Validação de formulários conforme regras de negócios

• Padrões de codificação • Testes unitários com karma/jasmine Obs.: Os layouts
dos protótipos são só ilustrativos, podem usar os frameworks de estilo de sua
preferência. (Ex.: Bootstrap)

### Fluxo de navegação

• Lista de investimentos o Executar uma chamada get no endereço
https://run.mocky.io/v3/ca4ec77d-b941-4477-8a7f-95d4daf7a653 o Montar a tela
conforme o protótipo fazendo a integração com a resposta da execução do serviço
acima. o Ao clicar em um plano que não está em carência (indicadorCarencia =
'N'), navegar para próxima tela.

• Resgate personalizado o Montar a tela conforme o protótipo usando as
informações do investimento selecionado na tela anterior. o Digitar os valores
que deseja resgatar de cada ação e clicar em confirmar resgate o Após clicar em
confirmar resgate, exibir os modais de erro ou sucesso Regras

• Lista de investimentos o Fundos de investimentos em carência
(indicadorCarencia = 'S') não pode realizar resgate, deve ficar desabilitado na
lista de investimentos e não permitir avançar para tela de resgate.

• Resgate personalizado o Realizar o cálculo do saldo da ação usando o campo
percentual, que é o percentual que essa ação representa no valor total do
investimento. o Valor a resgatar de cada ação não pode ser maior que saldo
acumulado da mesma, deve ser exibido um alerta abaixo do input quando isso
acontecer. Ex (O valor a resgatar não pode ser maior que R$ 2.614,13) o A cada
interação nos inputs, deve ser atualizado o campo valor total do resgate. o
Colocar mascaras de moeda nos inputs de valor a resgatar, para não permitir a
digitação de letras e formatar campos de saldos. Ex (R$ 2.614,13)

URL: Moc https://run.mocky.io/v3/ca4ec77d-b941-4477-8a7f-95d4daf7a653

## Cenário de teste 01 - Clicar em confirmar com mais de um campo a resgatar com valor inválido

• Clicar no investimento I

• Digitar um valor acima do disponível na primeira ação. Ex: BBAS3 tem 11 mil de
saldo acumulado, digitar 12 mil no campo valor a resgatar

• Digitar um valor abaixo do disponível na segunda ação. Ex: VALE3 tem 8 mil de
saldo acumulado, digitar 9 mil no campo valor a resgatar

• Clicar em confirmar Resultado esperado: Deve aparecer um modal alertando que
foi digitado um ou mais valor acima do permitido, e exibir quais ações estão com
erro. Ex: 03 - Modal de sucesso 02 - Clicar em confirmar com todos os campos com
valor validos

• Clicar no investimento I • Digitar um valor abaixo ou igual ao disponível na
primeira e segunda ação. Ex: BBAS3 tem 11 mil de saldo acumulado, digitar 11 mil
no campo valor a resgatar Ex: VALE3 tem 8 mil de saldo acumulado, digitar 2 mil
no campo valor a resgatar

• Digitar um valor abaixo ou igual ao disponível na terceira ação.

• Clicar em confirmar Resultado esperado: Deve aparecer um modal com a mensagem
que o resgate foi efetuado com sucesso, e quando clicar em novo resgate, voltar
para tela inicial. Ex: 03 - Modal de sucesso

Mocky: https://designer.mocky.io/

https://www.mocky.io/
