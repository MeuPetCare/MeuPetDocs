# Tecnologias do Projeto

## Linguagem & Padrões
- **TypeScript** (full-stack)
- APIs **REST** com **Swagger**
- Autenticação **JWT (Bearer)** e **RBAC** (Administrador, Veterinário)

## Front-end
- **Angular** 17+ (Angular CLI)
- **TypeScript**
- **Angular Router**
- Formulários: **Reactive Forms**
- UI: **Tailwind CSS**

## Back-end (API)
- **Node.js** 20 LTS
- **NestJS** 10+
- **Swagger** (nest/swagger) para documentação da API
- ORM: **TypeORM** 5+ (provider **MySQL**)  
- Validação DTO: **class-validator** / **class-transformer**

## Banco de Dados
- **MySQL** 8.x

## Qualidade de Código
- **ESLint** + **Prettier**
  
## DevOps / Ambientes
- **Docker** + **docker-compose** (dev)
- Serviços no compose: **MySQL**, **MinIO**, **MailHog**
- CI/CD (quando der): GitHub Actions (lint, testes, build)
- Variáveis via **12-factor** (.env por ambiente)

## Segurança (baseline)
- CORS restrito
- Rate limit básico
- Hash de senha **Argon2** (ou bcrypt ≥ 12)
- Validação de payload (DTOs)
- Uploads: checagem de MIME/tamanho
- OWASP Top 10 (injeção, XSS, IDOR, etc.)

---
