# Spring Boot CRUD API

Este é um projeto de API RESTful simples desenvolvido com **Spring Boot**, que implementa operações básicas de CRUD (Create, Read, Update, Delete) para gerenciamento de produtos.

## Funcionalidades

- **Criar Produto**: Adicione um novo produto com nome e valor.
- **Listar Produtos**: Obtenha uma lista de todos os produtos.
- **Buscar Produto por ID**: Obtenha detalhes de um produto específico.
- **Atualizar Produto**: Atualize os dados de um produto existente.
- **Deletar Produto**: Remova um produto pelo ID.

## Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.3.5**
- **Spring Data JPA**
- **Spring Validation**
- **PostgreSQL**
- **Maven**

## Configuração do Banco de Dados

O projeto utiliza PostgreSQL como banco de dados. Atualize as credenciais no arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/products-api
spring.datasource.username=postgres
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
```

### Endpoints
- **POST /produtos:** Cria um novo produto.
- **GET /produtos:** Retorna todos os produtos.
- **GET /produtos/{id}:** Retorna um produto específico pelo ID.
- **PUT /produtos/{id}:** Atualiza um produto pelo ID.
- **DELETE /produtos/{id}:** Deleta um produto pelo ID.


### Como Executar
Certifique-se de ter o Java 17 e o PostgreSQL instalados.
Clone o repositório:

```bash
git clone https://github.com/CarllosEduardo07/projeto-java-spring-crud.git
```
### Navegue até a pasta do projeto:
```bash
cd projeto-java-spring-crud
```
#### Configure o banco de dados no arquivo `application.properties`.

#### Execute o projeto:
```bash
mvn spring-boot:run
```

### Estrutura do Projeto
- ``controllers:`` Contém os controladores REST.
- ``models:`` Modelos que representam a entidade Produto.
- ``dtos:`` Objetos de transferência de dados para validações.
- ``repositories:`` Interface JPA para interagir com o banco de dados.

### Dependências Principais
As dependências principais estão definidas no pom.xml:

```bash
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
<dependency>
    <groupId>org.postgresql</groupId>
    <artifactId>postgresql</artifactId>
</dependency>
```

Autor <br>
<p>Carlos Eduardo Albuquerque</p>

Se precisar de algo mais no README, é só avisar!
