# 🏦 DIO Bank

Um sistema bancário simples desenvolvido em C# .NET como parte do bootcamp da Digital Innovation One (DIO).

## 📋 Sobre o Projeto

O DIO Bank é uma aplicação console que simula as operações básicas de um sistema bancário, permitindo gerenciar contas de pessoas físicas e jurídicas com funcionalidades completas de movimentação financeira.

## ✨ Funcionalidades

- **📊 Listar Contas**: Visualiza todas as contas cadastradas com seus extratos
- **➕ Inserir Nova Conta**: Cadastra novas contas (Pessoa Física ou Jurídica)
- **💸 Transferir**: Realiza transferências entre contas
- **💰 Sacar**: Efetua saques considerando saldo e limite de crédito
- **💳 Depositar**: Realiza depósitos em contas
- **🖥️ Limpar Tela**: Limpa o console para melhor visualização
- **❌ Sair**: Encerra a aplicação

## 🏗️ Estrutura do Projeto

```
DIO.bank/
├── Program.cs              # Arquivo principal com menu e operações
├── Classes/
│   └── Conta.cs            # Classe que representa uma conta bancária
├── Enum/
│   └── TipoConta.cs        # Enumeração para tipos de conta
├── DIO.bank.csproj         # Arquivo de configuração do projeto
├── DIO.bank.sln            # Arquivo de solução
└── README.md               # Este arquivo
```

## 🛠️ Tecnologias Utilizadas

- **C# .NET 9.0**: Linguagem de programação principal
- **Console Application**: Interface de linha de comando
- **Visual Studio Code**: IDE de desenvolvimento recomendada

## 🚀 Como Executar

### Pré-requisitos

- [.NET 9.0 SDK](https://dotnet.microsoft.com/download) instalado
- Editor de código (Visual Studio Code recomendado)

### Passos para execução

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/SavioFagundes/bankdio.git
   cd DIO.bank
   ```

2. **Execute o projeto**:
   ```bash
   dotnet run
   ```

3. **Ou compile e execute**:
   ```bash
   dotnet build
   dotnet run
   ```

## 🎮 Como Usar

Ao executar a aplicação, você verá o menu principal:

```
DIO Bank a seu dispor!!!
Informe a opção desejada:

1- Listar contas
2- Inserir nova conta
3- Transferir
4- Sacar
5- Depositar
C- Limpar Tela
X- Sair
```

### Exemplo de Uso

1. **Criar uma conta**: Escolha a opção `2`
   - Selecione o tipo (1 para Pessoa Física, 2 para Jurídica)
   - Digite o nome do cliente
   - Informe o saldo inicial
   - Defina o limite de crédito

2. **Fazer um depósito**: Escolha a opção `5`
   - Digite o número da conta (índice na lista)
   - Informe o valor a depositar

3. **Realizar um saque**: Escolha a opção `4`
   - Digite o número da conta
   - Informe o valor a sacar (respeitando saldo + crédito)

## 💡 Características Técnicas

### Classe Conta
- **Propriedades**:
  - `TipoConta`: Pessoa Física ou Jurídica
  - `Saldo`: Saldo atual da conta
  - `Credito`: Limite de crédito disponível
  - `Nome`: Nome do titular da conta

- **Métodos**:
  - `Sacar(double valor)`: Realiza saque com validação de saldo
  - `Depositar(double valor)`: Adiciona valor ao saldo
  - `ExibirExtrato()`: Mostra informações completas da conta
  - `ObterSaldo()`: Retorna o saldo atual

### Validações Implementadas
- ✅ Verificação de entrada nula ou inválida
- ✅ Validação de tipos de dados (números, strings)
- ✅ Verificação de saldo suficiente para saques
- ✅ Validação de existência de contas para operações
- ✅ Verificação de tipos de conta válidos

## 🔧 Melhorias Futuras

- [ ] Persistência de dados em arquivo/banco de dados
- [ ] Sistema de autenticação com senha
- [ ] Histórico de transações
- [ ] Interface gráfica (WPF/WinForms)
- [ ] API REST para integração web
- [ ] Juros e taxas bancárias
- [ ] Relatórios financeiros

## 👨‍💻 Desenvolvedor

Desenvolvido como parte do bootcamp da **Digital Innovation One (DIO)**.

## 📄 Licença

Este projeto é parte de um exercício educacional e está disponível para fins de aprendizado.

---

⭐ **Dica**: Use a opção "C" para limpar a tela quando o console ficar poluído com muitas informações!
