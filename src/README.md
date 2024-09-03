# Sistema de Gestão Bancária

Este projeto é um sistema simples de gestão bancária que permite a criação e gerenciamento de contas bancárias e clientes. O sistema é composto por várias classes que modelam clientes, contas bancárias e a operação do banco em si.

## Estrutura do Projeto

O projeto é dividido em três principais classes:

1. **Cliente**: Representa um cliente do banco.
2. **ContaBancaria**: Representa uma conta bancária que o cliente possui.
3. **Banco**: Representa o banco que gerencia as contas.

### Classes

#### Cliente

- **Atributos**:
  - `nome`: Nome do cliente.
  - `sobrenome`: Sobrenome do cliente.
  - `data_nascimento`: Data de nascimento do cliente.
  - `cpf`: CPF do cliente.
- **Métodos**:
  - `nome_completo()`: Retorna o nome completo do cliente.

#### ContaBancaria

- **Atributos**:
  - `numero_conta`: Número da conta (gerado aleatoriamente).
  - `saldo`: Saldo atual da conta.
  - `numero_saques`: Número de saques realizados no dia.
  - `limite_saques`: Limite de saques permitidos por dia.
  - `agencia`: Código da agência.
  - `transacoes`: Lista de transações realizadas na conta.
  - `cliente`: Referência ao cliente associado à conta.
- **Métodos**:
  - `gerar_numero_conta()`: Gera um número de conta aleatório.
  - `obter_numero_conta()`: Retorna o número da conta.
  - `depositar(valor_depositado)`: Deposita um valor na conta e registra a transação.
  - `sacar(valor_saque)`: Realiza um saque da conta e registra a transação.
  - `obter_extrato()`: Retorna um extrato completo da conta.

#### Banco

- **Atributos**:
  - `contas`: Lista de contas gerenciadas pelo banco.
- **Métodos**:
  - `criar_conta()`: Cria uma nova conta bancária e a adiciona ao banco.
  - `buscar_conta(numero_conta)`: Busca uma conta bancária pelo número.
  - `exibir_usuarios()`: Exibe todos os usuários cadastrados.

## Diagrama UML

O diagrama UML do projeto está disponível na pasta `src`. Você pode visualizar a imagem do diagrama UML clicando no link abaixo:

- [Diagrama UML](src/diagrama_uml.png)

O diagrama UML ajuda a entender a estrutura das classes e os relacionamentos entre elas.
