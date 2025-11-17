[README (3).md](https://github.com/user-attachments/files/23571839/README.3.md)
# 📘 Projeto SQL --- DDL, DML e Banco de Dados da Cafeteria

### *Repositório de Estudos em Banco de Dados --- SENAC*

Este repositório reúne estudos e práticas fundamentais sobre **banco de
dados relacional**, com foco nos comandos **DDL** e **DML**, além da
implementação de um **banco de dados simples para uma cafeteria
fictícia**.\
O objetivo é proporcionar uma compreensão clara e prática sobre como
estruturar e manipular dados utilizando SQL.

------------------------------------------------------------------------

## 📌 Objetivos do Projeto

-   Entender a diferença entre **DDL** (Data Definition Language) e
    **DML** (Data Manipulation Language).\
-   Criar e alterar tabelas utilizando comandos DDL.\
-   Manipular dados com comandos DML: inserir, atualizar, deletar e
    consultar registros.\
-   Desenvolver um banco de dados realista como exemplo prático.\
-   Organizar um repositório profissional com boas práticas de
    versionamento.

------------------------------------------------------------------------

## 🧱 1. Conceitos Fundamentais

### 🔹 **O que é DDL?**

**DDL** é a linguagem responsável por definir a **estrutura** do banco
de dados.

Comandos principais: - `CREATE` --- cria tabelas e objetos\
- `ALTER` --- altera estruturas já existentes\
- `DROP` --- exclui tabelas ou objetos

Exemplo:

``` sql
CREATE TABLE clientes (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(50) NOT NULL,
    curso VARCHAR(50)
);
```

------------------------------------------------------------------------

### 🔹 **O que é DML?**

**DML** permite manipular os **dados** que estão dentro da estrutura do
banco.

Comandos principais: - `INSERT` --- insere dados\
- `UPDATE` --- atualiza dados\
- `DELETE` --- remove dados\
- `SELECT` --- consulta dados

Exemplo:

``` sql
INSERT INTO clientes (nome, curso)
VALUES ('Maria', 'Banco de Dados');
```

------------------------------------------------------------------------

## ☕ 2. Banco de Dados --- Cafeteria Senac

Como parte prática do projeto, foi criado um banco de dados simples para
uma cafeteria fictícia.\
Ele inclui:

-   **produtos** (cafés, bebidas e alimentos)\
-   **clientes**\
-   **pedidos**\
-   **itens_pedido**

Trecho do código:

``` sql
CREATE TABLE produtos (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    categoria VARCHAR(50),
    preco DECIMAL(10,2) NOT NULL
);
```

O arquivo completo está disponível na pasta `sql_scripts/cafeteria.sql`.

------------------------------------------------------------------------

## 📂 3. Estrutura do Repositório

    /
    ├── README.md
    └── sql_scripts/
          ├── banco_de_dados.sql
          └── cafeteria.sql

------------------------------------------------------------------------

## 🚀 4. Como Executar o Projeto

1.  Abra seu SGBD (PostgreSQL, MySQL, DBeaver etc.)\
2.  Crie um banco de dados:

``` sql
CREATE DATABASE estudos_sql;
```

3.  Execute algum dos scripts da pasta `sql_scripts/`:
    -   `banco_de_dados.sql` → comandos DDL e DML estudados\
    -   `cafeteria.sql` → banco de dados da cafeteria
4.  Confirme se as tabelas foram criadas usando:

``` sql
SELECT * FROM nome_da_tabela;
```

------------------------------------------------------------------------

## 🎓 5. Sobre o Projeto

Este repositório foi desenvolvido como parte de um estudo introdutório
do módulo de **Banco de Dados** aplicado no SENAC.\
Ele reforça:

-   lógica e estruturação de banco de dados\
-   manipulação de dados\
-   boas práticas de organização de projetos SQL\
-   uso do GitHub como portfólio acadêmico

------------------------------------------------------------------------

## 📎 Arquivos Disponíveis

-   `cafeteria.sql` --- Banco de dados completo da cafeteria\
-   `banco_de_dados.sql` --- Comandos DDL e DML estudados

------------------------------------------------------------------------

Bom estudo! ☕💻
