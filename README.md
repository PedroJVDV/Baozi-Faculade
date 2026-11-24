# Baozi Store - API REST

Atividade Prática da disciplina de Desenvolvimento Web Back-End  
Centro Universitário Internacional UNINTER  

Aluno: Pedro Henrique Duques De Souza  
RU: 5579908  
Ano: 2026  

---

## Descrição do Projeto

API REST desenvolvida para gerenciamento de clientes, produtos e controle de pedidos da loja fictícia Baozi Store. O sistema implementa operações completas de CRUD (Create, Read, Update, Delete) utilizando a arquitetura MVC com camada de serviço e persistência em banco relacional.

---

## Tecnologias Utilizadas

- Java 17
- Spring Boot 3
- Spring Data JPA / Hibernate
- Banco de dados H2 (em memória com sintaxe compatível com MySQL)
- Maven
- Lombok
- Postman (para testes e validação das requisições)

---

## Estrutura de Pacotes

- com.baozistore.controller: Camada responsável pelos endpoints REST da aplicação.
- com.baozistore.service: Camada responsável pela lógica de negócios da aplicação.
- com.baozistore.repository: Interfaces Spring Data JPA para comunicação com a base de dados.
- com.baozistore.model: Classes de entidade mapeadas para tabelas relacionais.

---
---

## Endpoints Disponíveis

Módulo de Clientes:
- POST /clientes : Cadastra um novo cliente (retorna 201 Created).
- GET /clientes : Lista todos os clientes cadastrados (retorna 200 OK).
- GET /clientes/{id} : Consulta cliente por ID (retorna 200 OK ou 404 Not Found).
- DELETE /clientes/{id} : Exclui cliente por ID (retorna 204 No Content ou 404 Not Found).

Módulo de Produtos:
- POST /produtos : Cadastra um novo produto (retorna 201 Created).
- GET /produtos : Lista todos os produtos cadastrados (retorna 200 OK).
- GET /produtos/{id} : Consulta produto por ID (retorna 200 OK ou 404 Not Found).
- DELETE /produtos/{id} : Exclui produto por ID (retorna 204 No Content ou 404 Not Found).

Módulo de Pedidos:
- POST /pedidos : Registra um novo pedido (retorna 201 Created).
- GET /pedidos : Lista todos os pedidos cadastrados (retorna 200 OK).
- GET /pedidos/{id} : Consulta pedido por ID (retorna 200 OK ou 404 Not Found).
- DELETE /pedidos/{id} : Exclui pedido por ID (retorna 204 No Content ou 404 Not Found).

---
