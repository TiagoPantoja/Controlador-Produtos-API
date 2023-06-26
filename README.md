# Spring Boot Product API

Este é um exemplo de uma API de produtos desenvolvida utilizando o framework Spring Boot.

A API permite a manipulação de registros de produtos, fornecendo endpoints para listar todos os produtos, obter um produto específico, cadastrar um novo produto, atualizar um produto existente e excluir um produto.

## Tecnologias utilizadas

- Java
- Spring Boot
- Spring Data JPA
- HATEOAS

## Requisitos

- Java 8 ou superior
- Maven

## Executando a aplicação

Para executar a aplicação, siga as etapas abaixo:

1. Certifique-se de ter o Java e o Maven instalados em sua máquina.
2. Faça o download ou clone este repositório.
3. Navegue até o diretório raiz do projeto.
4. Execute o seguinte comando no terminal para compilar o projeto:

`mvn clean install`

5. Após a conclusão da compilação, execute o seguinte comando para iniciar a aplicação:

`mvn spring-boot:run`

6. A aplicação estará em execução e você poderá acessar os endpoints da API.

## Endpoints

A API expõe os seguintes endpoints:

### Listar todos os produtos

`GET /products`

Retorna uma lista de todos os produtos cadastrados.

### Obter um produto

`GET /products/{id}`

Retorna um produto com base no ID fornecido.

### Cadastrar um produto

`POST /products`

Cria um novo produto com base nos dados fornecidos no corpo da requisição.

### Atualizar um produto

`PUT /products/{id}`

Atualiza um produto existente com base no ID fornecido e nos dados fornecidos no corpo da requisição.

### Excluir um produto

`DELETE /products/{id}`

Exclui um produto com base no ID fornecido.

## Modelo de Dados

### ProductModel

O modelo `ProductModel` representa um produto e possui os seguintes atributos:

- `idProduct` (UUID): O identificador único do produto.
- `name` (String): O nome do produto.
- `value` (BigDecimal): O valor do produto.

## DTO

### ProductRecordDto

O DTO `ProductRecordDto` é usado para receber os dados de entrada do usuário ao criar ou atualizar um produto e possui os seguintes atributos:

- `name` (String): O nome do produto.
- `value` (BigDecimal): O valor do produto.

## Repositório

### ProductRepository

O repositório `ProductRepository` é responsável pela comunicação com o banco de dados e fornece métodos para realizar operações de CRUD nos produtos.

## Contribuindo

Se você encontrar algum problema ou tiver sugestões de melhoria, sinta-se à vontade para abrir uma _issue_ ou enviar uma solicitação de _pull request_.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
