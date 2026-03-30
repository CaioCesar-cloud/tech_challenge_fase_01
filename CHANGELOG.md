# Changelog

Todas as mudanças notáveis neste projeto serão documentadas aqui.

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/),
e este projeto adota [Versionamento Semântico](https://semver.org/lang/pt-BR/).

---

## [Unreleased]

## [0.1.0] - 2026-03-30

### Adicionado
- Estrutura base do projeto Spring Boot 3.2 com Java 17
- Dependências: Spring Web, Data JPA, Validation, Security (BCrypt), Lombok, DevTools
- PostgreSQL como banco de dados principal; H2 para testes
- Flyway configurado para migrações de banco de dados
- Springdoc OpenAPI (Swagger UI em `/swagger-ui.html`)
- `SecurityConfig` com `BCryptPasswordEncoder` e endpoints liberados
- `OpenApiConfig` com metadados da API
- `application.yml` com configuração via variáveis de ambiente
- `application-test.yml` com H2 in-memory para testes unitários
- Dockerfile multi-stage (build Maven + runtime JRE 17 Alpine)
- `docker-compose.yml` com serviços `app` e `postgres` (healthcheck + volume persistente)
- Estrutura de pacotes: `model`, `repository`, `service`, `controller`, `dto`, `exception`, `config`
- Pasta `db/migration/` preparada para scripts Flyway
- `.gitignore` para Maven, IDEs e variáveis de ambiente
- `README.md` com visão geral, arquitetura, pré-requisitos e endpoints

[Unreleased]: https://github.com/caioc/tech_challenge_fase_01/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/caioc/tech_challenge_fase_01/releases/tag/v0.1.0
