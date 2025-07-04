# 📚 Modelagem de Banco de Dados para Livraria

Este repositório contém o script SQL para criação e povoamento de um banco de dados relacional voltado a uma **livraria**, com foco em armazenar informações sobre os produtos (livros) disponíveis e os pedidos realizados por clientes.

## 🗂️ Estrutura do Banco de Dados

O modelo é composto por duas tabelas principais:

### 🔹 `produtos`
Armazena informações sobre os livros à venda.

- `id` (INTEGER, chave primária, auto incremento)
- `nome` (VARCHAR, nome do livro)
- `preco` (DECIMAL, preço do livro)

### 🔹 `pedidos`
Registra as compras feitas pelos clientes.

- `id` (INTEGER, chave primária, auto incremento)
- `produto_id` (INTEGER, chave estrangeira referenciando `produtos`)
- `quantidade` (INTEGER, número de unidades compradas)
- `data_pedido` (DATE, data da compra)

## 💡 Comandos Implementados

O script SQL neste repositório inclui:

- Criação das tabelas com suas chaves primária e estrangeira.
- Inserção de **quatro produtos** (livros) de exemplo.
- Inserção de **quatro pedidos** simulando compras em diferentes datas.
- Consultas `SELECT` para visualização dos dados inseridos.

## ✅ Exemplo de Produtos Inseridos

| ID | Nome                     | Preço   |
|----|--------------------------|---------|
| 1  | Livro de SQL             | 59.90   |
| 2  | HTML e CSS na Prática    | 44.50   |
| 3  | JavaScript Essencial     | 69.00   |
| 4  | Python para Iniciantes   | 75.20   |

## 🚀 Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/Dyogo199/ProjetoIntegradorII_Unidade03.git
2. Acesse a pasta:
   cd ProjetoIntegradorII_Unidade03

Importe o arquivo modelagem_livraria.sql para seu banco de dados compatível com SQL (ex: MySQL, MariaDB, SQLite, etc.).
Ajustes de sintaxe podem ser necessários conforme o SGDB utilizado.

Execute os comandos em um cliente SQL (como MySQL Workbench, DBeaver ou phpMyAdmin) para criar e popular o banco.

🔄 Versionamento
Este projeto utiliza Git para controle de versão.
Você pode consultar todo o histórico de commits clicando aqui.

🎓 Créditos
Desenvolvido por Dyogo Mondego para a disciplina Projeto Integrador em Tecnologia da Informação II — UFMS, 2025.



