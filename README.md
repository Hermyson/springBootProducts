# Spring Boot Product
Este é um projeto Spring Boot para a gestão de produtos. O projeto inclui funcionalidades básicas de CRUD (Create, Read, Update, Delete) para produtos.

## Tecnologias Utilizadas
Java 21
Spring Boot 3.30
Spring Data JPA
PostgreSQL
Maven

## Requisitos
Java 21
Maven 3.6.3 ou superior
PostgreSQL
Configuração do Projeto
Clone o repositório

## Configuração do Banco de Dados
Crie um banco de dados PostgreSQL e configure o application.properties com as suas credenciais do banco de dados.

spring.datasource.url=jdbc:postgresql://localhost:5432/seubancodedados
spring.datasource.username=seuusuario
spring.datasource.password=suasenha
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.hibernate.ddl-auto=update

## Construir o projeto

mvn clean install

## Executar o projeto

mvn spring-boot:run

## Endpoints
### Produto

-  GET /api/products - Lista todos os produtos
  GET /api/products/{id} - Busca um produto pelo ID
  POST /api/products - Cria um novo produto
  PUT /api/products/{id} - Atualiza um produto existente
  DELETE /api/products/{id} - Deleta um produto
