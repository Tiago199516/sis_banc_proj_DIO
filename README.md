# :dollar: Sistema Bancário com python

Este projeto é um Sistema bancário com Python proposto pelo bootcamp Santander da DIO.

## O desafio:

Fomos contratados por um banco para desenvolver o seu novo sistema. Esse banco deseja modernizar suas operações e para isso escolheu Python. Para a primeir versão devemos implementar apenas 3 operações: depósito, saque e extrato.

- **Operação de Depósito**: Deve ser possível depositar valores positivos para a minha conta bancária. A v1 do projeto trabalha apenas com 1 usuário, dessa forma não precisamos nos preocupar em identificar qual é o número da agência e conta bancária. Todos os depósitos devem ser armazenados em uma variável e exibidos na operação de extrato.

- **Operação de Saque**: O sistema deve permitir realizar 3 saques diários com limite máximo de R$ 500,00 por saque. Caso o usuário não tenha saldo em conta, o sistema deve exibir uma mensagem informando que não será possível sacar o dinheiro por falta de saldo. Todos os saques devem ser armazenados em uma variável e exibidos na operação de extrato.

- 🗒️ **Operação de Extrato**: Essa operação deve listar todos os depósitos e saques realizados na conta. No fim da listagem deve ser exibido o saldo atual da conta. Os valores devem ser exibidos utilizando o formato R$ xxx.xx, exemplo: R$ 1500.45