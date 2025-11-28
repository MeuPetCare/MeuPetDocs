# Tecnologias do Projeto

## Linguagem & Padrões
- **TypeScript** (full-stack)
- APIs **REST** com **Swagger**
- Autenticação **JWT (Bearer)** e **RBAC** (Administrador, Veterinário)

## Front-end
- **React** 18 com **TypeScript**
- **Vite** para build e desenvolvimento
- **Tailwind CSS** para estilização
- **Shadcn/ui** componentes reutilizáveis
- **React Router** para navegação

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
- CI/CD: GitHub Actions (lint, testes, build)
- Variáveis via **12-factor** (.env por ambiente)

## Deploy
- **Railway** - Deploy da API e banco de dados
- **Vercel** - Deploy do frontend React
- **GitHub Pages** - Documentação (disponível para deploy)

## Segurança (baseline)
- CORS restrito
- Rate limit básico
- Hash de senha **Argon2** (ou bcrypt ≥ 12)
- Validação de payload (DTOs)
- Uploads: checagem de MIME/tamanho
- OWASP Top 10 (injeção, XSS, IDOR, etc.)

---
