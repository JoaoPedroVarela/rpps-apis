
# RPPS API

Sistema de gestão de contribuintes, contribuições e benefícios voltado para Regimes Próprios de Previdência Social (RPPS). Essa API RESTful foi desenvolvida para realizar o cadastro, consulta, atualização e desativação de dados relacionados a contribuintes, categorias, salários mínimos e vínculos familiares.

## 🧩 Funcionalidades

- ✅ Cadastro e atualização de contribuintes
- ✅ Cadastro e listagem de contribuições
- ✅ Gestão de categorias de contribuintes
- ✅ Atualização de contribuições com base no salário mínimo
- ✅ Estrutura de parentesco e vínculos familiares
- ✅ Documentação interativa com Swagger

## 🛠️ Tecnologias Utilizadas

- Java 17+
- Spring Boot
- JDBC
- PostgreSQL
- Flyway (versionamento de banco)
- Swagger (documentação da API)

## 🗂️ Estrutura do Projeto

```
src
├── main
│   ├── java
│   │   └── br.com.rpps
│   │       ├── controller
│   │       ├── dto
│   │       ├── model
│   │       ├── repository
│   │       ├── service
│   │       └── util
│   └── resources
│       ├── application.properties
│       └── db/migration (Flyway)
```

## 🚀 Como Executar o Projeto

### Pré-requisitos

- Java 17 ou superior
- PostgreSQL
- Maven

### Passos

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/rpps-api.git
cd rpps-api

# Compile e execute o projeto
./mvnw spring-boot:run
```

## 🧪 Acessar a Documentação da API

Após iniciar o projeto, acesse no navegador:

```
http://localhost:8080/swagger-ui/index.html
```

## 🗃️ Banco de Dados

As tabelas são gerenciadas automaticamente pelo Flyway. Basta configurar o acesso ao seu banco no arquivo `application.properties`.

Exemplo:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/rpps
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

## 📌 Roadmap do Projeto (EAP)

- [x] Levantamento de requisitos
- [x] Modelagem de banco de dados
- [x] Criação de endpoints para contribuintes
- [x] Integração com salário mínimo
- [x] Cadastro de vínculos familiares
- [x] Documentação com Swagger
- [ ] Testes de performance e carga
- [ ] Deploy em ambiente cloud

## 📄 Licença

Este projeto é de uso acadêmico e sem fins lucrativos. Licença a definir.

---

Desenvolvido com 💻 por João Pedro Varela Borges
