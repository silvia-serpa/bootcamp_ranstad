# Esquema Conceitual – Oficina Mecânica

Este repositório contém o modelo conceitual desenvolvido para representar o sistema de controle e gerenciamento de ordens de serviço em uma oficina mecânica, conforme atividade proposta no bootcamp Randstad – DIO.

## 🎯 Objetivo
Modelar as entidades e relacionamentos necessários para registrar:
- clientes (PF e PJ);
- veículos;
- equipes e mecânicos;
- ordens de serviço;
- serviços executados;
- peças utilizadas.

## 🧩 Visão Geral do Modelo

### Cliente / ClientePF / ClientePJ
Estrutura de generalização/especialização:
- `Cliente` contém dados comuns.
- `ClientePF` e `ClientePJ` especializam o cliente conforme o tipo.

### Veículo
Cada veículo pertence a um cliente e é atendido por uma equipe de mecânicos.

### Equipe e Mecânico
- Uma equipe possui vários mecânicos.
- Cada mecânico possui código, nome e especialidade.

### Ordem de Serviço (OS)
- Associada a um veículo.
- Contém datas de emissão e conclusão.

### Serviço
- Cada OS pode ter vários serviços executados.
- Cada serviço possui tipo e valor de mão de obra (quando aplicável).

### Peças
- Cada OS pode ter várias peças utilizadas.
- Cada peça possui valor unitário, conforme narrativa.

## 📂 Arquivos
- `OS_oficina_V3.pdf` – Diagrama conceitual.
- `README.md` – Documentação do projeto.

