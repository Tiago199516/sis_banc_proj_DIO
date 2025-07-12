# :dollar: Sistema Bancário com python

Este projeto é um Sistema bancário com Python proposto pelo bootcamp Santander da DIO. A medida em que formos avançando no curso a complexidade do desafio e do código vai aumentando.

## O desafio:

### Parte 1
Fomos contratados por um banco para desenvolver o seu novo sistema. Esse banco deseja modernizar suas operações e para isso escolheu Python. Para a primeir versão devemos implementar apenas 3 operações: depósito, saque e extrato.

- **Operação de Depósito**: Deve ser possível depositar valores positivos para a minha conta bancária. A v1 do projeto trabalha apenas com 1 usuário, dessa forma não precisamos nos preocupar em identificar qual é o número da agência e conta bancária. Todos os depósitos devem ser armazenados em uma variável e exibidos na operação de extrato.

- **Operação de Saque**: O sistema deve permitir realizar 3 saques diários com limite máximo de R$ 500,00 por saque. Caso o usuário não tenha saldo em conta, o sistema deve exibir uma mensagem informando que não será possível sacar o dinheiro por falta de saldo. Todos os saques devem ser armazenados em uma variável e exibidos na operação de extrato.

- 🗒️ **Operação de Extrato**: Essa operação deve listar todos os depósitos e saques realizados na conta. No fim da listagem deve ser exibido o saldo atual da conta. Os valores devem ser exibidos utilizando o formato R$ xxx.xx, exemplo: R$ 1500.45

### Parte 2
Separar as funções existentes de saque, depósito e extrato em funções. Criar duas novas funções: cadastrar usuário (cliente) e cadastrar conta bancária.

* **Separação em funções**: Devemos criar funções para todas as operações do sistema. Cada função vai ter uma regra na passagem de argumentos. O retorno e a forma como serão chamadas, pode ser definida pelo *dev* da forma que lhe convier.
    1. **Saque**: A função saque deve receber os argumentos apenas por nome.  Sugestão de argumentos: *saldo, valor, extrato, limite, numero_saques e limite_saques*. Sugestão de retorno: *saldo e extrato*.
    2. **Depósito**: A função depósito deve receber argumentos apenas por posição. Sugestão de argumentos: *saldo, valor e extrato*. Sugestão de retorno: *saldo e extrato*.
    3. **Extrato**: A função extrato deve receber os argumentos por posição e nome. Argumento posicional: *saldo*. Argumento nomeado: *extrato*.

* **Novas Funções**: Necessário criar duas novas funções: *criar usuário e criar conta corrente*, mas se quiser, pode adicionar outras como por exemplo uma função para *listar contas*.
    1. **Criar usuário**: O programa deve armazenar os usuários em uma lista, um usuário é composto por nome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nro - bairro - cidade/DF. Deve ser armazenado somente os números do CPF. Não podemos cadastrar 2 usuários com o mesmo CPF.
    2. **Conta corrente**: O programa deve armazenar contas em uma lista, uma conta é composta por: agência, número da conta e usuário. O número da conta é sequencial, iniciando em 1. O número da agência é fixo: "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário.

    ###### ----------Dica----------
        :asterisk: Para vincular um usuário a uma conta, filtre a lista de usuários buscando o número do CPF informado para cada usuário da lista
