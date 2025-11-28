# MeuPet - Sistema de Gestão Veterinária

Sistema web para gerenciamento de animais em uma clínica veterinária, desenvolvido com React 18 + TypeScript no frontend e NestJS no backend.

## 🚀 Tecnologias

### Frontend
- React 18 com TypeScript
- Vite para build e desenvolvimento
- Tailwind CSS para estilização
- Shadcn/ui componentes reutilizáveis
- React Router para navegação

### Backend
- Node.js 20 LTS
- NestJS 10+
- TypeORM com MySQL
- JWT para autenticação
- Swagger para documentação da API

## 📋 Deploy

### Frontend
- **Vercel**: Deploy automático do React
- **GitHub Pages**: Disponível para deploy estático

### Backend
- **Railway**: Deploy da API e banco MySQL

### Documentação
- **GitHub Pages**: Deploy automático da documentação MkDocs

#### Para fazer deploy da documentação no GitHub Pages:

1. Acesse as configurações do repositório no GitHub
2. Vá em `Pages` no menu lateral
3. Em `Source`, selecione `GitHub Actions`
4. Crie o arquivo `.github/workflows/docs.yml`:

```yaml
name: Deploy Documentation

on:
  push:
    branches: [ main ]
  workflow_dispatch:

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Setup Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.x'
      - name: Install dependencies
        run: |
          pip install mkdocs-material
      - name: Build docs
        run: mkdocs build
      - name: Setup Pages
        uses: actions/configure-pages@v3
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v2
        with:
          path: './site'
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v2
```

5. Faça commit e push do arquivo
6. A documentação estará disponível em: `https://[seu-usuario].github.io/[nome-do-repo]`

## 📁 Estrutura da Documentação

- **Início**: Visão geral do projeto
- **Requisitos**: Visão, escopo, atores e elicitação
- **Arquitetura**: Tecnologias utilizadas no projeto

---

Desenvolvido por [Ana Catarina Santos](https://github.com/an4catarina)
