# Modelo Conceitual de Banco de Dados – E‑commerce

Este repositório contém o refinamento do modelo conceitual de um banco de dados para um sistema de e‑commerce, desenvolvido como parte do bootcamp Randstad – DIO.

## 🎯 Objetivo da atividade

Refinar o modelo apresentado no lab, acrescentando:

- **Cliente PF e Cliente PJ**  
  Uma conta pode ser Pessoa Física ou Pessoa Jurídica, mas não ambas.

- **Pagamento**  
  Um cliente pode cadastrar mais de uma forma de pagamento.

- **Entrega**  
  Cada pedido possui status de entrega e código de rastreio.

## 🧩 Estrutura do Modelo

### Cliente, ClientePF e ClientePJ
Aplicação de generalização/especialização:
- `Cliente` contém dados comuns.
- `ClientePF` e `ClientePJ` herdam o identificador de `Cliente` via chave estrangeira.

### Pagamento
- Relacionamento 1:N entre **Cliente → Pagamento**.
- Permite múltiplas formas de pagamento cadastradas.

### Entrega
- Relacionamento 1:1 entre **Pedido → Entrega**.
- Armazena status e código de rastreio.

## 📦 Outras entidades do modelo original
- Produto  
- Estoque  
- Fornecedor  
- Terceiro (Vendedor)  
- Pedido  
- Relações Produto/Pedido  
- Disponibilização de Produto  
- Estoque_has_Produto  
- ProdutoPorVendedor  


