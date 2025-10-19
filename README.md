# Workshop Spring Boot + JPA

Este projeto é um workshop desenvolvido com **Spring Boot** + **Spring Data JPA** com o objetivo de demonstrar o uso de persistência de dados, entidades, repositórios e transações em Java.

## 🧱 Tecnologias utilizadas

- Java (versão … — substituir pela versão real)  
- Spring Boot (versão usada no projeto)  

- Spring Data JPA  

- Banco de dados (ex: H2 / MySQL / PostgreSQL) — substituir/conferir conforme configuração  
- Maven (arquivo `pom.xml`)  
- GitHub para controle de versão  

## 📂 Estrutura de pastas
```
├── .mvn/
├── mvnw
├── mvnw.cmd
├── pom.xml
├── src/
│ ├── main/
│ │ ├── java/
│ │ │ └── com/
│ │ │ └── example/
│ │ │ └── projeto/
│ │ └── resources/
│ │ └── application.properties
│ └── test/
│ └── java/
└── .gitignore
```

> A estrutura indica que o projeto está configurado como uma aplicação Spring Boot típica usando Maven.

## 🚀 Como executar o projeto

  1. Clone o repositório:  
     ```bash
     git clone https://github.com/Hugolas-23/workshop-springboot-jpa.git
     ```
  2. Acesse o diretório do projeto:
     ```bash
     cd workshop-springboot-jpa
     ```
  3. Configure o banco de dados em src/main/resources/application.properties (ou application.yml):
     ```properties
     # Exemplo para H2 (modo em memória)
     spring.datasource.url=jdbc:h2:mem:testdb
     spring.datasource.driverClassName=org.h2.Driver
     spring.datasource.username=sa
     spring.datasource.password=
     spring.jpa.hibernate.ddl-auto=update
     spring.h2.console.enabled=true
     ```
  > Ajuste de acordo com o banco que você estiver utilizando.
  
  4. Compile e execute o projeto via Maven:
     ```bash
     ./mvnw spring-boot:run
     Ou, se preferir:
     mvn clean install
     mvn spring-boot:run
     ```
  5. Acesse a aplicação no seu navegador ou via API (dependendo das rotas definidas).
    Por exemplo: http://localhost:8080.

## 🧩 Funcionalidades implementadas

-Definição de entidades JPA (com anotações como @Entity, @Id, etc.).

-Repositórios Spring Data (extends JpaRepository<…>) para operações CRUD.

-Endpoints REST (via @RestController) para manipulação das entidades.

-Exceções e tratamento de erros.

## 🎯 Objetivo do workshop

### Este workshop foi criado para apoiar a compreensão de:

-o ciclo de vida de uma aplicação Spring Boot com acesso a banco de dados via JPA;

-como mapear entidades, relacionamentos, como usar repositórios prontos do Spring Data;

-como configurar corretamente o ambiente;

-como desenvolver endpoints REST simples que persistem e recuperam dados.

## 👨‍💻 Autor

Hugo Martins — @Hugolas-23

LinkedIn - www.linkedin.com/in/hugo-martins23
   

