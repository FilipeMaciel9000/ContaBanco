# Sistema Bancário em Java

Este projeto é uma aplicação de terminal simples que simula um sistema bancário utilizando **Programação Orientada a Objetos (POO)** em Java. O código é dividido em múltiplas classes, respeitando os quatro pilares da POO: **abstração**, **encapsulamento**, **herança** e **polimorfismo**.

---

## Conceitos aplicados

- Abstração: Classe `Conta` representa o conceito genérico de uma conta bancária.
- Encapsulamento: Atributos privados com acesso controlado por métodos públicos.
- Herança: `ContaCorrente` e `ContaPoupanca` estendem a classe `Conta`.
- Polimorfismo: Cada tipo de conta pode sobrescrever comportamentos, como o saque com taxa.

---

## Funcionalidades

- Criar conta corrente e conta poupança com entrada via `Scanner`
- Realizar depósito
- Realizar saque (com taxa para conta corrente)
- Transferir entre contas
- Exibir extrato

---

## Estrutura de diretórios

```

ContaBanco/
├── Main.java
├── models/
│   ├── Conta.java
│   ├── ContaCorrente.java
│   └── ContaPoupanca.java
├── services/
│   └── BancoService.java
└── utils/
└── ContaFactory.java

````

---

## Como executar

### Pré-requisitos

- Java 11 ou superior
- IDE como IntelliJ IDEA, Eclipse ou terminal com `javac`

### Passos para execução:

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/sistema-bancario-java.git
   cd sistema-bancario-java
````

2. Compile e execute com sua IDE favorita **ou** via terminal:

   ```bash
   javac Main.java models/*.java services/*.java utils/*.java
   java Main
   ```

---

## 📷 Demonstração (exemplo de uso)

```
Criando Conta Corrente:
Número da conta: 123
Agência: 001
Titular: João
Saldo inicial: 1000

Criando Conta Poupança:
Número da conta: 456
Agência: 002
Titular: Maria
Saldo inicial: 500

Depósito de R$500.00 realizado.
Saque com taxa de R$1.00.
Saque de R$101.00 realizado.
Transferência de R$200.00 para Maria realizada.

=== Extrato ===
Titular: João
Agência: 001
Conta: 123
Saldo: R$1199.00

=== Extrato ===
Titular: Maria
Agência: 002
Conta: 456
Saldo: R$700.00
```
