# Jogo da Velha - Deploy no Vercel

Este repositório contém um site estático (HTML/CSS/JS). Instruções rápidas para publicar no Vercel.

Opção A — Deploy rápido com Vercel CLI

1. Instale o Vercel CLI:

```bash
npm i -g vercel
```

2. No diretório do projeto execute:

```bash
vercel login
vercel              # para deploy de preview
vercel --prod       # para publicar em produção
```

Opção B — Conectar um repositório Git

1. Inicialize git, crie um repositório remoto (GitHub/GitLab/Bitbucket) e envie o código:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <URL-DO-REPO>
git push -u origin main
```

2. No dashboard do Vercel, clique em "New Project" → escolha o repositório → Deploy.

Observações
- O site é estático; não precisa de build por padrão.
- Se quiser que eu faça o deploy automático, forneça autorização (token Vercel) ou conecte o repositório ao Vercel e eu posso orientar.
