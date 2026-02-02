# JDBC Study Project

Projeto prático para estudo aprofundado sobre integração entre **Java** e Banco de Dados **MySQL** utilizando **JDBC** puro.

Este repositório documenta a implementação manual de conexões, gerenciamento de transações e boas práticas de manipulação de dados, servindo como base para entender o funcionamento interno de frameworks ORM.

## Funcionalidades e Conceitos Aplicados

* **Conexão Segura:** Implementação de conexão com banco de dados MySQL protegendo credenciais sensíveis via `db.properties`.
* **Connection Factory:** Padrão de projeto para centralizar e gerenciar a abertura/fechamento de conexões.
* **CRUD Completo:**
    * Inserção de dados (INSERT)
    * Leitura e formatação de dados (SELECT)
    * Atualização de registros (UPDATE)
    * Remoção de registros (DELETE)
* **Tratamento de Exceções:** Uso de exceções personalizadas (`DbException`) para encapsular erros de SQL.
* **Transações:** Controle manual de atomicidade (Commit e Rollback).

##  Tecnologias

* **Java 21**
* **JDBC** (MySQL Connector/J 9.6.0)
* **MySQL Server 8.0**
* **IntelliJ IDEA**

## Como executar

1. Clone o repositório.
2. Crie um banco de dados MySQL chamado `coursejdbc`.
3. Na raiz do projeto, crie o arquivo `db.properties` com suas credenciais locais:

```properties
user=seu_usuario
password=sua_senha
dburl=jdbc:mysql://localhost:3306/coursejdbc?useSSL=false&allowPublicKeyRetrieval=true
